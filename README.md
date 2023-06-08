SPA = Single Page Application

Interaction with API's gives you data for your front end other wise it would need to be hard coded (takes forevvver).

asynchronous / async = means "happening at disconnected times". 
    Will run at an arbitrary (unknown) future time, and other JS code can run in the meantime. 

EX  *Note: JS waits for no one*

Order)
    1) say hello user = sayHello()
    2) get weather information = getWeatherData() 
        > calls an "API" takes 
            - 2-3 sec to get info
                const weatherData = getWeatherData() > will get "undefined"
            This is where an "async" would come in handy to request the order to wait for step 2 to populate the data from the API call before continuing to step 3.
    3) giver user a prompt = givePrompt()
        If you use the weatherData above to show the prompt results will be "undefined".


Asynchronous programming = 
        enable your program to start a potentially long running task while still responding to other events rather than having to wait until one task has finished to respond to the other.

A: 1 / 3 / 2

Old way with "Asynchronous" code was used with "callbacks" functions.
    - callbacks is a function that gets called within another function so your passing the function along to get called back later.
    - callback hell or or pyramid of doom = so many callbacks that it gets hard to read
    - your work can get weird side effects where it doesn't always resolve so your code won't work every time when you use callbacks. 
    - Hard to de-bug

Instead we use "Promises"

What is it? 
    - is a JS object that represent the eventual result of an asynchronous operation.
    - Object with value and status

    EX    const tryGetRich = async () => (
            let num = await
            readFileAsync('/luckyNumber.txt);
            let success = await bookmarker.bet(num);
            if(success) {
                console.log("I'm rich!)
            }
        )

    `await` keyword must ALWAYS happen inside a function marked as `async`.
    `async` keyword with regular functions and arrow functions.

*can use the `async` keyword with regular functions and arrow functions.*

APIs = Application Programming Interface 

    Set of functions and procedures that allow for the creation of applications.
    Access the data and features of other applications, services, or operating systems.

    Client > Rest API > Database > Rest API > Client


-Installed "Thunder Client" within VS Code-

Public API's https://swapi.dev/ 

Resource: https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/PATCH

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

- asked to mess around with API's through thunder client