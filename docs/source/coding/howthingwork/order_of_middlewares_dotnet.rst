Order of Middlewares in DotNet
===================================

**What should be the other of the middlewares in the .Net pipeline?**

The recommended order of middlewares in the pipeline is as follows:

1. 𝐔𝐬𝐞𝐄𝐱𝐜𝐞𝐩𝐭𝐢𝐨𝐧𝐇𝐚𝐧𝐝𝐥𝐞𝐫 - This middleware is used for global exception handling. It catches any unhandled exceptions during request processing and generates an appropriate error response.
2. 𝐔𝐬𝐞𝐇𝐬𝐭𝐬 - This middleware is used to enforce HTTPS. It adds the HTTP Strict Transport Security (HSTS) header to the response, instructing the client always to use HTTPS.
3. 𝐔𝐬𝐞𝐇𝐭𝐭𝐩𝐬𝐑𝐞𝐝𝐢𝐫𝐞𝐜𝐭𝐢𝐨𝐧- This middleware causes an automatic redirection to HTTPS URL when an HTTP URL is received, in a way that forces a secure connection.
4. 𝐔𝐬𝐞𝐒𝐭𝐚𝐭𝐢𝐜𝐅𝐢𝐥𝐞𝐬 - This middleware serves static files from the wwwroot folder.
5. 𝐔𝐬𝐞𝐑𝐨𝐮𝐭𝐢𝐧𝐠- This middleware enables routing in the application. It examines the incoming request and maps it to the appropriate endpoint handler.
6. 𝐔𝐬𝐞𝐂𝐨𝐫𝐬 - This middleware enables cross-origin resource sharing (CORS). It allows cross-domain requests from the browser.
7. 𝐔𝐬𝐞𝐀𝐮𝐭𝐡𝐞𝐧𝐭𝐢𝐜𝐚𝐭𝐢𝐨𝐧- This middleware enables authentication. It authenticates the user making the request.
8. 𝐔𝐬𝐞𝐀𝐮𝐭𝐡𝐨𝐫𝐢𝐳𝐚𝐭𝐢𝐨𝐧 - This middleware enables authorization. It checks if the incoming request is authorized to access the requested resource.
9. 𝐔𝐬𝐞𝐑𝐞𝐬𝐩𝐨𝐧𝐬𝐞𝐂𝐨𝐦𝐩𝐫𝐞𝐬𝐬𝐢𝐨𝐧 - This middleware enables response compression. It compresses the response body using Gzip or Deflate to reduce the network transfer time and improve the performance of the application.
10. 𝐔𝐬𝐞𝐄𝐧𝐝𝐩𝐨𝐢𝐧𝐭𝐬 - This middleware maps HTTP requests to endpoint handlers. It's used to configure the routing for the application. It maps controller actions to the appropriate endpoints.

It is important to note that the order of the middlewares can affect the behavior of your application. For example, if UseAuthorization middleware is placed before UseAuthentication middleware, the authentication system won't be able to authenticate the user and the authorization system won't be able to authorize the user as the user's identity won't be established yet. So, the order of the middlewares should be carefully considered while building an application.

.. image:: ./imgs/order_middleware_pipeline_dotnet.svg
  :width: 600
  :alt: Roadmap DotNet Developers