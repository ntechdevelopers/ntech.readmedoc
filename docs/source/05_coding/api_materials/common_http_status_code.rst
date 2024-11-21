Common Http Status Code
===================================

**What are HTTP status codes?**

HTTP status codes are three-digit responses from the server to the browser-side request. Everyone has probably gotten the classic 404 page-not-found error. That is an HTTP client error status code and there are a lot more of them.
These status codes (also called response status codes) serve as a means of communication between the server and the internet browser and there are multiple code classes based on the type of information they are communicating. The differences in classes are indicated through the first digit of the error code, for example: just like a 404, any other 4xx will mean that in some way the page or website could not be reached, while a 2xx means that your request was successfully completed.

**How are HTTP status codes categorized?**

HTTP status codes are split into 5 different categories. Each category will give you hints as to what the response was, even if you don't know the specific response code.
For an explanation of each category - and each individual status code - click on the corresponding link below or go to our complete list of HTTP status codes.

- 1xx - Informational: The server has received the request and is continuing the process 
- 2xx - Successful: The request was successful and the browser has received the expected information 
- 3xx (Redirection): You have been redirected and the completion of the request requires further action
- 4xx (Client Error): The website or the page could not be reached, either the page is unavailable or the request contains bad syntax 
- 5xx (Server Error): While the request appears to be valid, the server could not complete the request


**What does a 1xx Informational status code mean?**

A 1xx Informational status code means that the server has received the request and is continuing the process. A 1xx status code is purely temporary and is given while the request processing continues. For most tasks you won't encounter these much, as it's not the final response to the request.

- 100 Continue
- 101 Switching protocols
- 102 Processing
- 103 Early Hints

What does 100 Continue mean?
The 100 Continue status code means that the initial part of the request has been received by the server and that the client should proceed with the request or ignore the response if the request has already finished.

What does 101 Switching protocols mean?
The 101 Switching protocols status code means that the server understands the Upgrade header field request and indicates which protocol it is switching to.

What does 102 Processing mean?
The 102 Processing status code means that the server has accepted the full request but has not yet completed it and no response is available as of yet.

What does 103 Early Hints mean?
The 103 Early hints status code is intended to be used to allow the user agent to preload resources, while the server prepares a response. It is intended to be primarily used with the Link Header.

**What does a 2xx Succesful status code mean?**

A 2xx Succesful status code means that the request was successful and the browser has received the expected information. This is generally the one you want to see, as it means that the request was a success and has been received, understood and accepted it. As a website owner you should make sure that all pages and resources (images, videos, etc.) all return a 2xx status code. This means that browsers can reach it successfully and that your website visitors can see and use your website.

- 200 OK
- 201 Created
- 202 Accepted
- 203 Non-Authoritative Information
- 204 No Content
- 205 Reset Content
- 206 Partial Content
- 207 Multi-Status
- 208 Already Reported
- 226 IM Used

What does 200 OK mean?
The 200 OK status code means that the request was successful, but the meaning of success depends on the request method used:

    + GET: The requested resource has been fetched and transmitted to the message body.
    + HEAD: The header fields from the requested resource are sent in without the message body. 
    + POST or PUT: A description of the result of the action is transmitted to the message body.
    + TRACE: The request messages, as received by the server, will be included in the message body

When looking at things SEO-wise the 200 OK response code is the perfect status code for a functioning page, all the linked pages are working as they should. A 200 will mean that search engine crawlers can successfully crawl the page and it will be put into their search index.

What does 201 Created mean?
The 201 Created status code means that the request was successfully fulfilled and resulted in one or possibly multiple new resources being created.

What does 202 Accepted mean?
The 202 Accepted status code means that the request has been accepted for processing, but the processing has not been finished yet. The request may or may not be completed when the processing eventually takes place.

What does 203 Non-Authoritative Information mean?
The 203 Non-Authoritative Information status code means that the request was successful. However, the meta-information that has been received is different from the one on the origin server and has instead been collected from a 3rd party or local copy. When not used for backups or mirrors of another resource a 200 OK response is preferable.

What does 204 No Content mean?
The 204 No Content status code means that while the server has successfully fulfilled the request, there is no available content for this request. But the user agent might want to update its currently cached headers for this resource, for the new one. 

What does 205 Reset Content mean?
The 205 Reset Content status code means that the user should reset the document that sent this request.

What does 206 Partial Content mean?
The 206 Partial Content response code is a response to a Range header sent from the client when requesting only a part of the resource.

What does 207 Multi-Status mean?
The 207 Multi-Status status code conveys information about multiple resources, in situation when multiple status codes are appropriate.

What does 208 Already Reported mean?
The 208 Already Reported status code is used inside the response element DAV: propstat, in order to avoid enumerating the internal members of multiple bindings to the same collection repeatedly.

What does 226 IM Used mean?
The 226 IM response code means that the server has successfully fulfilled a GET request for the resource, and the response is a representation of the result of one or multiple instance-manipulations applied to the current instance.

**What does a 3xx Redirection code mean?**

A 3xx Redirection status code means that you have been redirected and the completion of the request requires further action. Redirects are a natural part of the internet and you shouldn't be scared to have 3xx redirect status codes on your website. A redirect means that the request was received successfully, but that the resource was found elsewhere. If a webpage has changed path and you try to access it through the old path, your CMS will often redirect the user to the new path. Ultimately the request will end in a 2xx success, but first it must go through the 3xx redirection.

- 300 Multiple Choices
- 301 Moved Permanently
- 302 Found (Previously "Moved temporarily")
- 303 See Other
- 304 Not Modified
- 305 Use Proxy
- 306 Switch Proxy
- 307 Temporary Redirect
- 308 Permanent Redirect
 

What does 300 Multiple Choices mean?
The 300 Multiple Choices status code means that the request has multiple possible responses and the user/user agent should choose one.

What does 301 Moved Permanently mean?
The 301 Moved Permanently response code means that the target resource has been assigned a new permanent URL and any references to this resources in the future should use one of the URLs included in the response.
When looking at things SEO-wise the 301 Permanent Redirect should be used every time a URL is moved permanently. This redirect passes your current link equity from your content to the new URL. Links that result in a status code 301 does give slightly less link equity than 200. So if you have a lot of links going through a 301 Permanent Redirect it is advised to fix these, if possible.

What does 302 Found (Previously “Moved temporarily”) mean?
The 302 Found status code, previously known as “Moved temporarily”, means that the URI of the request has been changed temporarily, and since changes can be made to the URI in the future, the effective request URI should be used for future requests.
When looking at things SEO-wise the 302 Found should only be used when making temporary changes as it does not pass the link equity the same way as a 301. If the page is not going to come back you should always use 301.

What does 303 See Other mean?
The 303 See Other response code is sent by the server in order to direct the client to get the requested resource at another URI with a GET request.

What does 304 Not Modified mean?
The 304 Not Modified response code informs the client that the response has not been modified. This means that the client can continue to use the already present, cached version of the response.

What does 305 Use Proxy mean?
The 305 Use Proxy status code instructs a client that it should connect to a proxy and then repeat the same request there. This response code is deprecated due to security concerns.

What does 306 Switch Proxy mean?
The 306 Switch proxy status code is no longer in use. It was used to inform the client that the subsequent requests should use the specified proxy.

What does 307 Temporary Redirect mean?
The 307 Temporary Redirect status code gets sent by the server in order to direct the client to the requested resource at another URI. The request method, however, must not be changed.

What does 308 Permanent Redirect mean?
The 308 Permanent Redirect status code means that the requested resource has been permanently assigned a new URI and future references to the resource should be made by using one of the enclosed URIs.

**What does a 4xx Client Error mean?**

A 4xx Client Error status code means that the website or the page could not be reached and either the page is unavailable or the request contains bad syntax. As a website owner you should do your best to avoid these, as it means your users will not find what they're looking for. This can be either pages that are no longer found and are either temporarily or permanently gone. Besides giving a bad user experience, it can also hurt your SEO efforts.

- 400 Bad Request
- 401 Unauthorized
- 402 Payment Required
- 403 Forbidden
- 404 Not Found
- 405 Method Not Allowed
- 406 Not Acceptable
- 407 Proxy Authentication Required
- 408 Request Timeout
- 409 Conflict
- 410 Gone
- 411 Length Required
- 412 Precondition Failed
- 413 Payload Too Large
- 414 URI Too Long
- 415 Unsupported Media Type
- 416 Range Not Satisfiable
- 417 Expectation Failed
- 418 I'm a Teapot
- 421 Misdirected Request
- 422 Unprocessable Entity
- 423 Locked
- 424 Failed Dependency
- 425 Too Early
- 426 Upgrade Required
- 428 Precondition Required
- 429 Too Many Requests
- 431 Request Header Fields Too Large
- 451 Unavailable For Legal Reasons

What does 400 Bad Request mean?
The 400 Bad Request status code means that the server could not understand the request because of invalid syntax.

What does 401 Unauthorized mean?
The 401 Unauthorized status code means that the request has not been applied because the server requires user authentication.

What does 402 Payment Required mean?
The 402 Payment Required status code is a response reserved for future use. It was originally created to be implemented in digital payment systems, however, it is rarely used and a standard convention of using it does not exist.

What does 403 Forbidden mean?
The 403 Forbidden status code means that the client request has been rejected because the client does not have rights to access the content. Unlike a 401 error, the client's identity is known to the server, but since they are not authorized to view the content, giving the proper response is rejected by the server.

What does error 404 mean?
The 404 Not Found status code means that the server either did not find a current representation for the requested resource or is trying to hide its existence from an unauthorized client.

When looking at things SEO-wise the 404 Not Found status code pages with a high volume of traffic should be redirected using a 301 to the most relevant page possible. For some pages, however, a 404 might be necessary, for example, if the product is out of stock for an extended period of time. If you have external links pointing to a page that returns 404, you will lose the link equity those links would otherwise give.

If you need to fix 404 errors, jump to this section.

What does 405 Method Not Allowed mean?
The 405 Method Not Allowed status code means that while the server knows the request method, the method has been disabled and can not be used.

What does 406 Not Acceptable mean?
The 406 Not Acceptable status code is sent by the server when it does not find any content following the criteria given by the user agent.

What does 407 Proxy Authentication Required mean?
The 407 Proxy Authentication Required status code means that the client must first be authenticated by a proxy (similar to a 401).

What does 408 Request Timeout mean?
The 408 Request Timeout status code means that the server did not receive a complete request in the time that it prepared to wait.

What does 409 Conflict mean?
The 409 Conflict status code means that the request could not be fulfilled due to a conflict with the current state of the target resource and is used in situations where the user might be able to resubmit the request after resolving the conflict.

What does 410 Gone mean?
The 410 Gone status code means that the target resource has been deleted and the condition seems to be permanent. 
When looking at things SEO-wise the 410 Gone status code is a more permanent version a 404. The page will no longer be available from the server and has no forwarding address available. If you want to completely remove a page from Googles search index, then using 410 on a page is the proper way of doing it (instead of simply 404). 

What does 411 Length Required mean?
The 411 Length Required status code means that the server has rejected the request because it requires the Content-Length header field to be defined.

What does 412 Precondition Failed mean?
The 412 Precondition Failed status code means the server does not meet one or multiple preconditions that were indicated in the request header fields.

What does 413 Payload Too Large mean?
The 413 Payload Too Large status code means the server refuses to process the request because the request payload is larger than the server is able or willing to process. While the server may close the connection to prevent the client from continuing the request, it should generate a Retry-After header field and after how long can the client retry.

What does 414 URI Too Long mean?
The 414 URI Too Long status code means that the server is refusing to service the request because the request-target was longer than the server was willing to interpret.

What does 415 Unsupported Media Type mean?
The 415 Unsupported Media Type status code means that the server is rejecting the request because it does not support the media format of the requested data.

What does 416 Range Not Satisfiable mean?
The 416 Range Not Satisfiable status code means that the range specified in the Range header field of the request can't be fulfilled. The reason might be that the given range is outside the size of the target URI's data.

What does 417 Expectation Failed mean?
The 417 Expectation Failed status code means that the Expectation indicated by the Expect request-header field could not be met by the server.

What does 418 I am a Teapot mean?
The 418 I'm a Teapot status code means that the server refuses to brew coffee because it is, in fact, a teapot. (It is a reference to a 1998 April Fools' joke called ''Hyper Text Coffee Pot Control Protocol'').

What does 421 Misdirected Request mean?
The 421 Misdirected Request status code means that the client request was directed at a server that is not configured to produce a response.

What does 422 Unprocessable Entity mean?
The 422 Unprocessable Entity status code means that while the request was well-formed, the server was unable to follow it, due to semantic errors.

What does 423 Locked mean?
The 423 Locked status code means that the resource that is being accessed is locked.

What does 424 Failed Dependency mean?
The 424 Failed Dependency status code means that the request failed due to the failure of a previous request.

What does 425 Too Early mean?
The 425 Too Early status code means that the server is not willing to risk processing a request that might be replayed.

What does 426 Upgrade Required mean?
The 426 Upgrade Required status code means that while the server refuses to perform the given request using the current protocol, it might be willing to do so after the client has been upgraded to a different protocol.

What does 428 Precondition Required mean?
The 428 Precondition Required status code means that the origin server requires the request to be conditional.

What does 429 Too Many Requests mean?
The 429 Too Many Requests response code means that in the given time, the user has sent too many requests.

What does 431 Request Header Fields Too Large mean?
The 431 Request Header Fields Too Large means that the server is not willing to process the request because its header fields are indeed too large, however, the request may be submitted again once the size of the request header fields is reduced.

What does 451 Unavailable For Legal Reasons mean?
The 451 Unavailable For Legal Reasons response code means that the user has requested an illegal resource (such as pages and sites blocked by the government).

**What does a 5xx Server error mean?**

A 5xx Server error status code means that while the request appears to be valid, the server could not complete the request. If you're experiencing 5xx server errors for your website, you should immediately look at your server. If you're hosting your own server you'll need to start debugging to figure out why it is not responding properly. If you're using an external hosting provider you'll need to reach out to them, so they can look at it.

- 500 Internal Server Error
- 501 Not Implemented
- 502 Bad Gateway
- 503 Service Unavailable
- 504 Gateway Timeout
- 505 HTTP Version Not Supported
- 506 Variant Also Negotiates
- 507 Insufficient Storage
- 508 Loop Detected
- 510 Not Extended
- 511 Network Authentication Required

What does 500 Internal Server Error mean?
The 500 Internal Server Error status code means that the server has encountered a situation that it does not know how to handle.
When looking at things SEO-wise the 500 Internal Server Error indicates a problem with the server, not the actual availability of the content. Since bots and users will both be lost, the link equity will go down fast.

What does 501 Not Implemented mean?
The 501 Not Implemented response code means that the request can not be handled because it is not supported by the server.

What does 502 Bad Gateway mean?
The 502 Bad Gateway response code means that the server received an invalid response while working as a gateway to handle the response.

What does 503 Service Unavailable mean?
The 503 Service Unavailable response code means that the server is currently not ready to handle the request. This is a common occurrence when the server is down for maintenance or is overloaded.
When looking at things SEO-wise the 503 Service Unavailable status code means that the server is unavailable and the visitor, bot or human, is asked to return again at a later time. This could be because of either server maintenance or server overload and search engines know to come back and check the availability later.
If you want to fix 503 errors, jump to this section.

What does 504 Gateway Timeout mean?
The 504 Gateway Timeout response code means that the server acting as a gateway could not get a response time.

What does 505 HTTP Version Not Supported mean?
The 505 HTTP Version Not Supported response code means that the version of HTTP used in the request is not supported by the server.

What does 506 Variant Also Negotiates mean?
The 506 Variant Also Negotiates response code means that the server has the following internal configuration error: The chosen variant resource is configured to engage in transparent negotiation itself, therefore it cannot be a proper endpoint in the negotiation process.

What does 507 Insufficient Storage mean?
The 507 Insufficient Storage status code means that the method could not be performed on the resource because the server is not able to store the representation that would be needed to complete the request successfully.

What does 508 Loop Detected mean?
The 508 Loop Detected response code means that the server has detected an infinite loop while processing the request.

What does 510 Not Extended mean?
The 510 Not Extended response code means that further extensions are required for the server to be able to fulfil the request.

What does 511 Network Authentication Required mean?
The 511 Network Authentication Required response code indicates that the client needs to authenticate to gain network access. 