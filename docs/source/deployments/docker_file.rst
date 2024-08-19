Docker File
===================================


**Docker File**

An image contains all the dependencies and configurations that required to run an application.  Example like, A cut-down OS, Third-party Libraries, Application files, Environment Variables. 
Once we have an image we can start container from it.  A container is just like a virtual machine it provides an isolated environment for executing an application. 
We are considering a static web application developed in react. 

To run an node application we need to follow some steps: 

``
# Install Node 
npm install 
npm start
``

Based on your application development you choose the dependencies.

**Docker File Instructions**

A Docker file contains instructions for building an image. 

- FROM - it specifies the base image, which contains files and directories were we can built on top of it. 
- WORKDIR - it specifies the working directory. Once we use this command all the commands will execute in this directory. 
- COPY/ADD - used to copy files 
- RUN - it used for executing the operating system commands. ENV - It is used for setting up the environment variables. 
- EXPOSE - to tell the container start at the given port. 
- USER - specifies the user that run the application. 
- CMD - to execute a command 
- ENTRYPOINT - specify the command where the container start. 

**Choosing the Right Base Image**

FROM is for choosing base image. Base image can be an Operating System(OS) like windows or Linux or It can be an OS + Runtime application. for example if you are an javascript developer you start with node or if you are python developer you start with python image. 

FROM node by default docker assumes that it chooses the latest, never use latest for building an application it causes conflicts with version compatibility issues. By using TAG we can avoid it in tag we specify the node version and the Linux distribution. 

``FROM node:14.16.0-alpine3.13``

Here alpine is an Linux distribution cut-down OS. 

**Copying Files and Directories**

After choosing the base image next step is copying the application files into the image. 
COPY and ADD both do the same process but ADD has some additional features. 

By using the copy command we copy the files in current directory to the image. during docker build docker engine it can’t access beyond the directory. 

``COPY app.js /app/`` it means copying the app.js file into the /app/ folder in the image. if /app is not there it will create a new one. 
``COPY . /app/`` it means all the source code including directories copy to the image. /app/ is an absolute path. We can use an relative path if we set the  WORKDIR. 

Instead of specifying directory explicitly in copy we can use the WORKDIR it will make sure every operations is being done on that directory. 

``WORKDIR /app`` now we can use COPY . . it mans the relative path in this case  /app/ .  

If the file name has spaces it will cause syntax errors. for example hello world.txt we need to make an entry like array of strings. Like ``COPY [”hello world.txt”, “.”] ``. 

ADD is like COPY but by using ADD we can copy files using the URL as well. Example: ``ADD http://…/file.json ``. 

The another advantage of ADD is if we copy the compressed file it will automatically un-compress the files. 

**Excluding Files and Directories**

For excluding flies & directories like in git docker uses ``.dockerignore`` file to ignore. In that file we can mention files and directories. for example ``node_modules/ ``, Here we are excluding the node third-party libraries in node application development. By using it we can reduce the transferring context.  

**Running Commands**

RUN is used to execute the commands for installing dependencies of our application. 

``RUN npm install`` to install node dependency third-party libraries. 

**Setting Environment Variables**

The environment variables is used to change the values in your application for example if you want to update the api link in the front end application we use ``ENV API_URL=http://api-myapp.com/ ``, Here API_URL is the environment variable and  the URL is it is value. 
ENV is used to work with environment variables. With out equal sign also it works but it is prefer to use. 

**Exposing Ports**

EXPOSE command used to list in which port our container is listening.
Example: ``EXPOSE 3000`` it means our container is listening on port 3000. The EXPOSE command does not automatically publish the port in the host OS, it is just for documentation purpose to tell us eventually this container listens on that port. 

**Setting the User**

By default Docker run the application by using root privileges. To root privileges are the highest privileges, to reduce it we use regular user to start the application with lowest privileges. Linux commands to create group and user and assign to it. 

``
addgroup app 
adduser -S -G app user01 
# we can combine these two commands into a sing line addgroup app && adduser -S -G app user01 
``

In Docker file we use RUN to execute this command 
``RUN addgroup app && adduser -S -G app app ``, here app is the user name and the group name as well. Once we set that the we use USER command to set the user USER app after that all the following commands will be executed using this user. 

If we run our application using root user the hacker might re-write the application if we run it by using system user it has only the read privileges no write privileges.  
If you are defining users you should need to define them immediately after the  FORM after choosing the base image. 

**Defining Entrypoints**

By using CMD command we can instruct default command to execute. for example running the node application 
CMD npm start by using this we don not need to run our application explicitly. If you have multiple CMD instructions it will consider the last CMD . 
The difference between the RUN and the CMD instructions is: 

- The RUN instruction is the build time instruction, it is executed at the time of building the image. 
- The CMD instruction is an run-time instruction, it is executed when starting a container. 
- The CMD instruction has two forms 1. Shell form, 2. Execute form which takes array of strings. 

``
#shell form  
CMD npm start 
#Exec form 
CMD ["npm", "start"] 
``

The difference is if you use shell form the docker will execute the command inside a different shell. The common best form to use is Execute form. Because by using Exec form we can directly execute the commands with out spinning up the new process.  
ENTRYPOINT is also similar to the CMD instruction it also has two forms SHELL form and Exec form. 

Example: ``ENTRYPOINT npm start or ENTRYPOINT [”npm”, “start”] ``. 

The difference is we can overwrite the CMD during the starting of our container. we can not easily overwrite the ENTRYOINT command. If you want to change the entry point command we need to use ``--entrypoint`` attribute during the running of a container. 
The both CMD and ENTRYPOINT is used for supply the default instruction or command. 

Complete Docker File example for react-app:

``
FROM node:14.16.0-alpine3.13 
RUN addgroup app && adduser -S -G app app USER app 
WORKDIR /app 
COPY . . 
RUN npm install 
ENV API_URL=http://api.myapp.com/ EXPOSE 3000 
CMD ["npm", "start"]
``


