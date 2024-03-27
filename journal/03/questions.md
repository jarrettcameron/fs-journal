# Application Architecture, MVC Design Pattern
01. What are the Pillars of Object Oriented Programming (`OOP`)?

  > There are four pillars of OOP, the four pillars are: abstraction, encapsulation, inheritance and polymorphism. Abstraction and encapsulation are pretty similar as they both revolve around simplification and organization of code to make projects more extendable and readable. We haven't really gotten to subclasses or inheritance yet but I look forward to it.

02. How does `export` differ from `export default`?

  > Export is for exporting multiple values with set names while export default is better when exporting single values or renaming imports. Structure and context are huge factors in which to use.

03. What is Encapsulation?

  > Encapsulation is used to hide or obfuscate methods that deal with an app's data (prime example being the export for service classes). It's done this way to make it more difficult from a client view to reverse the process while also making it easier to find certain methods that may change data. This makes debugging way easier and not just by the developer but by anyone else picking up the project.

04. What are some of the benefits of the `Proxy` object that we are using in our structure for applications?

  > It allows us to see modification to the object that's being proxied. This makes it possible to create event handlers to detect when an object or value is changed. This makes it super helpful for controllers to keep drawn data up-to-date.

05. What the difference between a `class` and an instance of a `class`?

  > Classes are like the blueprint of the structure but an instance of a class includes all the relevant data. An instance of a class also has the methods included in the class which make accessing certain functions way faster and accessible.

06. What is a computed Property?

  > Computed properties are really cool as they allow you to set dynamic object keys/property names which can be extremely useful for making code more versatile. There's honestly a few more uses of computer properties but they are kind of confusing without a better understanding of the specific conditions in which they'd be useful.

07. What is the purpose of the `MVC` pattern?

  > There's a few reasons but one of the main benefits is readability. MVC allows a project to be way more organized and structured compared to how we were working before. This makes code much easier to edit and debug. If there's a certain part that's not working, it's a lot easier to find the specific point of failure by recognizing which layer the error was caused in.

08. What is the job of the `Controller` in the `MVC` Pattern?

  > The controller is responsible for drawing data to the page. The controller is also responsible for communicating with the Service to pass view-interactions to it.

09. What is the job of the `Service` in `MVC`?

  > The service layer is responsible for two main things. The first is logic and the second is data modification.

10. What is the job of the `Model` in `MVC`?

  > The model is the blueprint of the data, it's how the data is structured. It's then registered in the AppState which is used by the Controller (read) and the Service (read/write) to access the data in that way.
