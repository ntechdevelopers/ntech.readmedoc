Http Request Methods
===================================

**GET**

Example: ``GET/api/employees/{employee-id}``

Returns a specific employee by Employee ID.
Description: Retrieves data from the server. It should only retrieve data and should have no other effect on the data.

**PATCH**

Example: ``PATCH/api/employees/123 { "name": "Brij" }``

Updates name for employee id 123
Description: Also used to update resources but it only updates the fields that were included in the request.

**OPTIONS**

Example: ``OPTIONS/api/main.html/1.1``

Returns Permitted HTTP Method in this URL
Description:This Method is used to get information about the possible communication options for the given URL or an asterisk to refer to the entire server

**POST**

Example: ``POST/api/employees/department``

Creates a department resource
Description: Used to send data to a server to create a new resource. The data is included in the body of the request.

**DELETE**

Example : ``DELETE/api/employees/235``

Delete employee by Employee ID.
Description: The DELETE method deletes a resource. Regardless of the number of calls, it returns the same result.

**TRACE**

Example: ``TRACE/api/main.html``

Responds the exact request that client sent.
Description: The TRACE Method is for diagnosis purposes. It echoes the received request so that a client can see what changes or additions have been made by intermediate servers.

**PUT**

Example: ``PUT/api/employees/123``

Update employee by employee ID
Description: Similar to POST, but it's used to update an existing resource. The entire resource is updated at once.

**HEAD**

Example: ``HEAD/api/employees``

Similar to GET, but it does not return the list of employees
Description: Typically this is used to check if a resource is available and to get the metadata.

**CONNECT**

Example: ``CONNECT www.example.com:443 HTTP/1.1``

Connects to the URL Provided
Description: The Connect Method is for making end to end connections between a client and a server. It makes a two way connection like a tunnel between them.