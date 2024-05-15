# Working in a Professional Environment
01. What is Inheritance?

> Inheritance is an idea in Object-Oriented Programming that allows classes to inherit behavior, methods and structure from another class. A prime example of a time we use this in class would be working with the express template we create controllers by extending from a util 'BaseController'. This allows the newly created controller to inherit behavior from that util class (registering the controller with express).

02. What is the `Singleton` design pattern?

> The singleton design pattern is a pattern that restricts a class to only have one instance of itself. This is done to keep things more organized and to prevent possible conflicts of multiple instances accessing the same resources at once. A time that we've used something similar would be with MVC services, when we create a service class we don't export the class but instead export an instance of the class. This effectively limits the instances of the class to one instance.

03. What is the `Observer` design pattern?

> The observer design pattern is used to efficiently communicate between objects. This is done through events, one object subscribes to be notified of an event through the other, this object will then notify it when changes are made. We used a similar structure with the mvc starter with AppState.on().

04. What is the `Strategy` design pattern?

> Strategy design pattern is used when a class all have a basic structure and function to them but need to be altered slightly across multiple algorithms. Strategy pattern allows an algorithm to be applied to the basic class instance.

05. What is the `Factory` design pattern?

> The factory design pattern allows objects to be created in a superclass but allows subclasses to alter the type of the object. It's handy for when you need flexibility in creating objects without directly specifying their classes.

06. What is test driven development?

> Test driven development is a development process where specific tests are used to mark progression and planning in development. The process starts by making a test for a specific piece of functionality that's going to be added. Then that test is ran to make sure it fails on unexpected output and passes on expected output. The next step is writing the actual base functionality to pass the initial test. After the basic test is passed, a new test can be drawn to add any checks or more complex pieces to the function and the process repeats.

07. In Scrum/Agile what is the DoD?

> The DoD stands for definition of done, it's the standard for measuring when a task is truly completed in development. It's a checklist that covers everything from basic functionality to polishing, testing and documentation.

08. Give two examples of a user story:

> As a user, I should be able to receive notifications when someone interacts with my threads and posts.
> As a user, I should be able to edit and delete previous posts and threads that I've made.

09. During which ceremony is your Sprint Backlog created?

> The sprint backlog is created during the sprint planning phase.

10. In which of these ceremonies are Tasks assigned to you?

> Tasks are usually assigned during the sprint planning in the form of sprint backlogs.
