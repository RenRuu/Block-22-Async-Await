
Asynchronous = means "happening at disconnected times".

Also called 'Async Code' in JS. Will run at an arbitrary (unknown) future time, and other JS code can run in the meantime. 

Asynchronous programming = enable your program to start a potentially long running task while still responding to other events rather than having to wait until one task has finished to respond to the other.

Asynchronous Code:
- Callbacks 
    (self review on this.....)
or
- Promises
    What is it? 
        is a JS object that represent the eventual result of an asynchronous operation.
        Object with value and status
        
        ASYNC/AWAIT(promises)
        (added thunderclient to VScode)

        `await` keyword must ALWAYS happen inside a function marked as `async`.
        `async` keyword with regular functions and arrow functions.

    EX)
        async function getNumber() {
            const num = await readFileAsync('/luckyNumber.txt')
        }
        getNumber();
    

APIs = Application Programming Interface 
    Set of functions and procedures that allow for the creation of applications.
    Access the data and features of other applications, services, or operating systems.

    Client > Rest API > Database > Rest API > Client

    RESTful APIs
        Representational State Transfer (REST)
        Created as a guideline to manage communication on a complex network (network)
        Used to support high performing and reliable communication at scale. 
        
        Resource: 
        https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/PATCH 

        Method: GET
        Action: retrieve info about an existing resource 
        Ex) http://example.com/api/orders/123(get order 123)

        Method: POST
        Action: create a new resource 
        Ex) http://example.com/api/orders

        Method: PUT
        Action: update a resource
        Ex) http://example.com/api/orders/123(updateorder123)

        Method: DELETE
        Action: delete a resource 
        Ex) http://example.com/api/orders/123(deleteorder123)

    Fetching Data
        "Fetch" is a web API that the browser makes available to JavaScript to access data. The fetch() method accesses this Fetch API.

        It sends a request to sources outsides of the local process, like your computer's files system, or a remote database.

        It also receives a response, which we can unravel using Async/await 

    HTTP Methods
        HyperText Transfer Protocol

        Internet protocol for sending and receiving information 
        In a wed application, a client requests information, and a server provides the responses.

        CRUD Operations 
            Create | Read | Update | Delete
            These are the four basic operations a software application should be able to perform.

            Users must be able to create data, have access to the data in the UI by reading the data, update or edit the data, and delete the data.

            HTTP Method:
                Method: GET
                CRUD Action: Retrieve a resource 

                Method: POST
                CRUD Action: Create a Resource 

                Method: PUT
                CRUD Action: Update a resource 

                Method: DELETE
                CRUD Action: Delete a resource 

*Stopping point in class*
- asked to mess around with API's 


