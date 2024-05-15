# CSharp and SQL Fundamentals
01. What is the purpose of a `namespace`?

  > Namespaces are used primarily organization but also makes importing easier. Namespaces are broken down by application and then class type. For instance in the dotnet templates the first part of the namespace signifies the specific project we are working on `csharp_project_name` or something similar, it's followed by the type of files we are working with. If you're creating a model it could be `namespace csharp_project_name.Models`. This makes it very easy to import all models or sort through the project faster.

02. What is the difference between a `class` and an `interface`?

  > An interface is used with inheritance to define what objects a class should have. A class can then pull from an interface and inherit those objects.

03. What is the method that returns an instance of a class, yet it has no return type?

  > Void methods.

05. In the Car example what is the access modifier of the `Start()` method?

  ```c#
  abstract class Car
  {
    public string Start()
    {

      return "Vroooom";

    }
  }
  ```

  > The access modifier of the `Start()` method is public. This means that it can be accessed externally. Although the method can be accessed externally, it's important to note that the class is abstract which prevents it from being initialized. The method and all other members of the `Car` class can only be accessed through inheritance.

06. In the Car example what is `string` an indication of?

  > In this example `string` is the return type from the `Start()` method. This means that when the code is ran a string result can be expected.

07. In the Car example what is `abstract` preventing?

  > `abstract` prevents classes from being initialized, this means that accessing members of the class is only possible through inheritence.

08. In a SQL table, what is the difference between information in a row and information in a column?

  > A column is comparable to a field/property, it defines what exactly is being stored and how. A column could be a `username` field with the datatype varchar/string. A row is individual entries of columns. For example, rows could look like ("username1", "username2" ...) while columns look like username VARCHAR(255) NOT NULL etc. A table is a collection of columns (fields) and rows (values).

09. Demonstrate the necessary SQL for creating a table called `characters` with the values `name, age, description` as strings, and an `int` id.

  > `CREATE TABLE characters(id INT NOT NULL AUTO_INCREMENT, name VARCHAR(255) NOT NULL, age TINYINT UNSIGNED NOT NULL,description VARCHAR(500));` I changed the age datatype because strings aren't quite appropriate for an age.

10. In SQL how can you query more than a single table? Provide an example.

  > `SELECT * FROM posts JOIN accounts ON posts.creatorId = accounts.id;` This would return posts and accounts where posts creatorId matches an account Id.
