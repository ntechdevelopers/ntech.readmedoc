CORS and How to Enable them in .NET
===================================

CORS stands for Cross-Origin Resource Sharing, so what exactly is cross-origin?

These two URLs have the same origin:
``https://ntechdevelopers.com/Get/Ntech``  
``https://ntechdevelopers.com/Get/AllIsWell``

These URLs have different origins:
``https://ntechdevelopers.com/Get/Ntech``  
``http://ntechdevelopers.net/Get/AllIsWell``

To facilitate requests from different origins, you need to enable CORS in .NET.

In .NET 6+, by using the combination of these methods, you can enable CORS as per your requirement.

- **AllowAnyOrigin**: This policy allows requests from any origin.
- **WithOrigins**: This policy allows requests from specific origins. You can specify one or more origins as arguments to this method.
- **AllowAnyHeader**: This policy allows requests with any header.
- **WithHeaders**: This policy allows requests with specific headers. You can specify one or more headers as arguments to this method.
- **AllowAnyMethod**: This policy allows requests with any HTTP method (e.g., GET, POST, PUT, DELETE).
- **WithMethods**: This policy allows requests with specific HTTP methods. You can specify one or more methods as arguments to this method.

A few things to keep in mind:

- CORS is not a security feature. CORS is a W3C standard that allows a server to relax the same-origin policy.
- An API isn't safer by allowing CORS.
- It's a way for a server to allow browsers to execute a cross-origin request that otherwise would be forbidden.
- Browsers without CORS can't do cross-origin requests.
