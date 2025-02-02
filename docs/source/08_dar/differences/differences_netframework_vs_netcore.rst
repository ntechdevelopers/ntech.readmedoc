.NET Framework vs .NET Core
===================================

Now we understand that .NET Framework and .NET Core are two different .NET implementations, therefore, both can be compared.

**.NET Framework**
    1. The .NET Framework is the first implementation of .NET which works on Windows only
    2. Its source code is public but Microsoft doesn’t accept third party contributions for it
    3. It has a very rich desktop top development framework for windows which include Windows Forms and WPF
    4. A huge third-party packages library is also available for it
    5. It doesn’t support the in-app deployment model
    6. Although it can be used with a docker container, its image size is large and can only be deployed on Windows containers

**.NET Core**
1. .NET Core is the latest implementation of .NET which runs on Windows, Linux, and macOS
2. Its open-source and Microsoft accepts third party contribution to .NET Core
3. It supports desktop frameworks like Windows Forms and WPF from version 3.0
4. The .NET Core also has support for a large number of third party packages as well but still, it doesn’t compete with .NET Framework in this area
5. It does support in-app deployment model
6. It is the best choice to work with docker containers

**.NET Framework and .NET Core vs .NET Standard**

Because .NET Framework and .NET Core are .NET implementations, therefore, we can compare them together against the .NET Standard.

**.NET Framework and .NET Core**
    1. The .NET Framework and .NET Core are implementations of .NET
    2. Both frameworks have runtime which manages the execution of applications
    3. The base class library is also a part of both frameworks
    4. We can create different types of projects in either framework

**.NET Standard**
    1. The .NET Standard is a specification and not a .NET implementation
    2. It specifies a set of APIs that all the .NET implementations have to implement
    3. We can create only class library type projects with it

**Deciding Target Platform and Version**
Let’s discuss what point should we keep in mind while choosing the target platform and their versions.
We should use the .NET Core:
    1. While developing applications for cross-platform
    2. For the development of microservices
    3. When we want to use Docker containers
    4. To develop high-performance and scalable systems

Use the .NET Framework when:
    1. We want to target only Windows
    2. Our application uses some third party packages which are not supported by .NET Core
    3. The application uses .NET technologies that are not available for .NET Core

.NET Standard should be the choice when:
    1. We want to share our common code across different .NET implementations

Once we choose the right platform and project type for our application, the next step is to use the correct version. Let’s suppose that we have to target both, the .NET Framework and .NET Core and we also want to share the common code across both of these platforms.