# A bit more CSharp and SQL
1. What does ***inheritance*** accomplish for us in C#?

  > Inheritance allows classes to inherit members from another, this saves us a lot of time when creating classes that share similar properties. An example of this being used in our C# projects would be with models, the RepoItem class creates Id, CreatedAt and UpdatedAt members for the other models through inheritance.

2. How does ***member inheritance*** work in C#? Does a `Class` inherit all members of the base `Class`?

  > A class does NOT inherit *all* members of the base class. If a member is private, it cannot be accessed through inheritance.

3. How does ***accessibility*** affect inheritance?

  > As mentioned above, access modifiers directly affect which members can be accessed through inheritance. Public modifiers are accessible, private modifiers are not, protected are accessible, internal is accessible within the assembly.

4. What is the difference between a `PRIMARY KEY` and a `FOREIGN KEY`

  > Primary key is how a column is sorted, its the unique identifier for a column. A foreign key is creating a relationship between one internal column and a foreign column on another table.

5. What is an ***alias***?

  > An alias is used in SQL as an alternative name to simplify a result from a more complex query. An example of this is the COUNT(..) as ALIAS being used to condense that data down into a 'virtual' column.

6. Demonstrate how you would query a join statement that would get all of a doctors patients from the following collections:

  ```SQL
  CREATE TABLE doctors (
    id INT NOT NULL AUTO_INCREMENT,
    -- CODE OMITTED
    PRIMARY KEY (id)
  )

  CREATE TABLE patients (
    id INT NOT NULL AUTO_INCREMENT,
    -- CODE OMITTED
    PRIMARY KEY (id)
  )

  CREATE TABLE patient_doctors (
    id INT NOT NULL AUTO_INCREMENT,
    doctorId INT NOT NULL,
    patientId INT NOT NULL,

    FOREIGN KEY (doctorId)
      REFERENCES doctors(id),
    FOREIGN KEY (patientId)
      REFERENCES patients(id),
  )

  ```

  > SELECT patients.* FROM patients JOIN patient_doctors ON patients.id = patient_doctors.patientId JOIN doctors ON patient_doctors.doctorId = doctors.id WHERE doctors.id = @DoctorId;
