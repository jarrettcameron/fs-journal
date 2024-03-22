# Intro to JavaScript
01. Which keywords are used to declare a variable in JavaScript?

    > var, let, const. Pretty self explanatory, let and var are quite similar but have differences in scope functionality and ability to re-declaration. Const is unique as the immediate value (important when it comes to reference types as that can be confusing) cannot be changed or re-declared. The object itself can be changed but the value of the const variable cannot.

02. What is the definition of a function?

    > Readings defined it as 'a subprogram designed to perform a particular task', I like to think of it as a versatile code snippet of sorts, something that is used frequently throughout a program.

03. What are the `SOLID` principles?

    > Couldn't find anything about this in the readings nor was it mentioned in class but I did some research to get the answer. SOLID is an acronym for S (Single Responsibility Principle) O (Open-Closed Principle) L (Liskov Substitution Principle) I (Interface Segregation Principle) D (Dependency Inversion Principle).

04. Given this array: How could you remove the `pineapple`?

    ```js
    let fruit = ['apple', 'banana', 'pineapple', 'orange', 'strawberry']
    ```

    > I personally like to use the splice function with the first arg being the value you want to remove and the second arg being the amount of items to remove. In this case it would look something like fruit.splice('pineapple', 1).

05. Given these two objects: How could you add each to the others friends arrays?

    ```js
    let you = {
        name: "You",
        hair: true,
        friends: []
    }
    let them = {
        name: "Them",
        hair: false,
        friends: []
    }
    ```

    > them.friends.push(you.name)
    > you.friends.push(them.name)

06. Give an example of a JavaScript `Conditional`:

    > if (x > y) { console.log("do something"); }

07. What is the main difference between `parameters` and `arguments`?

    > They both basically refer to the same concept but in different places. Parameters are local/internal to the function, it's what is being used in the function where its defined. function test(param1, param2) { } whereas arguments are plugged into a function when the function is being called test(arg1, arg2).

08. Instead of writing everything to the console, what is a better way to debug your code?

    > While console logging can be extremely helpful, overuse of logging can make things more confusing. Apart from that side effect, there's many other tools to use for debugging. Breakpoints are very helpful for better understanding what your code is doing and what functions and variables states are. Chrome Dev Tools in general are super helpful for debugging.

09. What is the difference between a `primitive` value and a `reference` value?

    > This one is a bit tricky to explain in words. Primitive data types are simple and direct values (num, bool, string). If you set a variable to a primitive data type and set another variable to that variable and change the second variable, the values will be different. They can be set independently from each other. Reference data types reference primitive data types, they point back to the same definition, when you change a reference object you are changing that data anywhere else that it is referenced through that definition.

10. Demonstrate a loop that prints the numbers between -100 and 100?

    > for (let i = -100; i <= 100; i++) console.log(i)
    > This should print out numbers from -100 to 100. The <= makes the loop inclusive with 100 instead of < which would have stopped the loop at 99.
