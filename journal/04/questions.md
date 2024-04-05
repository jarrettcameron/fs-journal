# Understanding Asynchronous Code, and API's
01. What is the difference between `asynchronous` code and `synchronous` code?

  > Async code runs on a different thread from the main thread so it can run parallel with the main thread. This means that tasks that might take longer to execute (such as Network Requests) can run and be handled without stopping any functionality in the main thread. Synchronous code runs in the main thread which means it will always run in order one at a time.

02. What is an event listener?

  > An event listener is a piece of code that handles changes or events of an object. This week we used AppState.on() to attach an event listener to run code when a variable in our AppState was changed or emit was called.

03. What does *REST* stand for, and in simple terms what does it mean??

  > REST stands for representational state transfer. To put it *very* simple, it's an architecture/format that dictates how applications and APIs should interact with each other.

04. What is a callback / higher order function?

  > A callback function is a piece of code that is ran when an event is triggered or a task has finished. They can be used in specific situations to prevent race-conditions and avoid registering event listeners for single-use situations.

05. What is a `promise`? How do you capture an error from a `promise`?

  > A promise is kind of like a wrapper for a task. It's basically a *promise* to run a task. You can access the status and handle if the task was successful or if it threw an error. You can handle an error from a promise using .catch().

06. Name three processes used to make requests over `HTTP`?

  > This is worded poorly so I'm gonna assume the question is what are some steps to making HTTP requests. And it depends on a lot. The first step is usually to identify what HTTP method needs to be used in the request. The next would be to setup async functions to properly handle the request. Third would be to perform the request through either fetch() or axios.

07. What does the `API` acronym stand for?

  > API stands for Application Programming Interface. APIs allow applications to interact with data stored on other applications through a convenient and *hopefully* well-documented format.

08. What must you do in order to `await` a promise inside of a function?

  > The function must have the async modifier for await to be used. If the function is not async, it cannot await as it's on the main thread.

09. What is the purpose of encapsulation in programming?

  > Encapsulation is helpful for two main things, the first being restricting access to certain functions and data of an object. The second being better organization, structure and control over the data.

10. What is `HTTP` response code for a successful request?

  > The HTTP response code for a successful request is 200 / OK.

11. What is a 400 error?

  > HTTP Status Code 400 means Bad Request. In the past week I've noticed this error is extremely common with malformed payload/query data. It's a pretty vague error though so the possibilities for receiving a 400 error are endless.
