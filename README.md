# Java Classes and Objects - Simple Classes

## Introduction

In this exercise, you will use simple java classes to create an improved StudentManager called `BetterStudentManager`.
You will need to create a `Student` class to represent a student, and you will need to complete the methods in the
`BetterStudentManager` class to manage a list of students.

> [!NOTE]
> You may notice that the build is broken when you open the project and there are errors showing. This is because the
> `Student` class is not yet created and implemented.  Once you have implemented the `Student` class, the errors will
> disappear.

## Implementing the Student Class

To implement the `Student` class, you will need to create a new class called `Student` in the `src/main/java/org/example`
directory. The `Student` class should have the following public (non-static) fields:

| Field Name | Type   | Description              |
|------------|--------|--------------------------|
| name       | String | The name of the student  |
| grade      | double | The grade of the student |

Once you have implemented this class, you will see the errors in this project disappear.

## Implementing the BetterStudentManager Class

To implement the `BetterStudentManager` class, you will need to complete the methods in the `BetterStudentManager` class

### `addStudent(String name, double grade)`

The `addStudent` method should add a student to the list of students. The methood takes a name and a grade as
parameters, and should create a new `Student` object with the given name and grade, and add it to the list of students.

### `removeStudent(String name)`

The `removeStudent` method should remove a student from the list of students. The method takes a name as a parameter,
and should remove the student with the given name from the list of students.

You will need to loop through the list of students to find the student with the given name, store the index of the
found student, and then **after** the loop, remove the student at the stored index using the `remove` method of the
`ArrayList` class.

### `getStudentList()`

The `getStudentList` method should return a String representation of the list of students. The method should loop through
the list of students and build a String representation of the list of students, with each student on a new line, and 
each line containing the name and grade of the student separated by a space

For example:

```
Alice 90.0
Bob 85.0
Charlie 95.0
```

## Verifying Your Solution

Once you have completed the exercises, run the tests in the `src/test/java/org/example/BetterStudentManagerTests.java`
to verify that your solutions are correct.

You should also manually verify that your solution is correct by running the `Main` class and interacting with the
`BetterStudentManager` class to add and remove students and print the list of students.

