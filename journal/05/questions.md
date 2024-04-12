# Intro to Server side concerns with JavaScript
01. What do the letters of the acronym `CRUD` stand for?

  > CRUD is an acryonym for the types of requests that can be sent to an API. C for Create, R for Read, U for Update and D for Delete.

02. Each action that `CRUD` represents maps to an HTTP request. What HTTP request does each `CRUD` action correspond to?

  > C stands for create (POST method), R stands for read (GET method), U stands for Update (PUT method) and D stands for delete (DELETE method).

03. What does `ORM` stand for? Which `ORM` do we use when interacting with MongoDB

  > We use mongoose for interacting with MongoDB. ORM stands for Object Relational Mapper.

04. Which two `HTTP` request types include a body?

  > POST and PUT requests both contain a body to send the data that needs to be changed or created to the API.

05. In a/an _______ coding model, when you call a function, it returns only when the action has finished and stops your program for the time the action takes. Likewise in a/an _______ coding model, multiple things are allowed to happen at one time. When you perform an action, your program continues to run.  Fill in the blanks.

  > Synchronous. Asynchronous.

06. What are the three types of data relationships? Provide an example of each.

  > One to Many such as an Account to Posts it can make, Many to Many such as a Book that was written by multiple authors. One to one like an account to it's address.

07. What is middleware?

  > Middleware is basically a block of code that runs before a 'gateway' in an API. A prime example of this being Auth0Provider. This piece of middleware protects everything behind it by verifying a user is authenticated, if they are not they receive a 401.

08. The ______ pipeline delivers information from the client while the ______ pipeline returns it. Fill in the blanks.

  > request & response? Not sure what answer is being looked for here.

09. Demonstrate the pattern that is used to include a request query with the client's `HTTP` request providing the property `tag` and the value `winter`.

  > ?tag=winter

10. What is a ***virtual property***?

  > A virtual property is a property that is not directly stored in the database. Instead is generated when the database converts a query to JSON, during this process the virtual property is attached (may need to be populated).
