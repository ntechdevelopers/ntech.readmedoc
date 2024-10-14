Middleware in .NET
===================================

**Middleware in .NET**

Middleware is software assembled into an app pipeline to handle requests and responses. 
Each component:

- Chooses whether to pass the request to the next component in the pipeline.
- Can perform work before and after the next component in the pipeline.

Here are some common types of middleware that might be used in a .NET API program:

1. **Routing middleware**:  

This middleware is responsible for determining which endpoint should handle a particular request based on the request's path and method.

2. **Exception handling middleware**:  

This middleware is responsible for catching and handling exceptions that occur during the processing of a request.

3. **Authentication and authorization middleware**:  

This middleware is responsible for verifying a request from an authenticated and authorized user.

4. **CORS (Cross-Origin Resource Sharing) middleware**:  

This middleware adds the necessary headers to allow a browser to make cross-origin requests to the API.

5. **Response compression middleware**:  

This middleware is responsible for compressing the response payload to reduce the size of the response and improve performance.

6. **Request validation middleware**:  

This middleware is responsible for validating incoming requests to ensure that they conform to the expected format.

7. **Response caching middleware**:  

This middleware is responsible for caching responses to reduce the load on the server and improve performance.

8. **Static file serving middleware**:  

This middleware is responsible for serving static files, such as HTML, CSS, and JavaScript files, from the file system.

It’s important to note that the order in which middleware is added to the pipeline can be important, as the middleware will be executed in the order in which it is added.  
For example, if the authentication middleware is added before the routing middleware, the routing middleware will not be executed until the authentication middleware has been completed.


**Order of Middlewares in DotNet**

What should be the order of the middlewares in the .NET pipeline?
The recommended order of middlewares in the pipeline is as follows:

1. **UseExceptionHandler**:  

This middleware is used for global exception handling. It catches any unhandled exceptions during request processing and generates an appropriate error response.
   
2. **UseHsts**:  

This middleware is used to enforce HTTPS. It adds the HTTP Strict Transport Security (HSTS) header to the response, instructing the client always to use HTTPS.

3. **UseHttpsRedirection**:  

This middleware causes an automatic redirection to the HTTPS URL when an HTTP URL is received, forcing a secure connection.

4. **UseStaticFiles**:  

This middleware serves static files from the `wwwroot` folder.

5. **UseRouting**:  

This middleware enables routing in the application. It examines the incoming request and maps it to the appropriate endpoint handler.

6. **UseCors**:  

This middleware enables cross-origin resource sharing (CORS). It allows cross-domain requests from the browser.

7. **UseAuthentication**:  

This middleware enables authentication. It authenticates the user making the request.

8. **UseAuthorization**:  

This middleware enables authorization. It checks if the incoming request is authorized to access the requested resource.

9. **UseResponseCompression**:  

This middleware enables response compression. It compresses the response body using Gzip or Deflate to reduce network transfer time and improve application performance.

10. **UseEndpoints**:  

This middleware maps HTTP requests to endpoint handlers. It is used to configure the routing for the application and maps controller actions to the appropriate endpoints.

It is important to note that the order of the middlewares can affect the behavior of your application.  
For example, if the `UseAuthorization` middleware is placed before the `UseAuthentication` middleware, the authentication system won't be able to authenticate the user, and the authorization system won't be able to authorize the user as the user's identity won't be established yet.  
Therefore, the order of the middlewares should be carefully considered while building an application.

.. image:: ./imgs/order_middleware_pipeline_dotnet.svg
  :width: 600
  :alt: Roadmap DotNet Developers