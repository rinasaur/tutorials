# Classes

## Introduction
In this tutorial we will design, develop, and use some very basic custom classes. Complete the following exercises in small groups.

## The Circle class
1. Define a new class named `Circle`.

2. Define a **parameterized constructor** (`__init__` method) to initialize a `Circle` with a specified **radius** (a `float`). Your radius should be assigned to an **instance variable** (data attribute)

3. Within the `__init__`  method, assign a second data attribute called `area` that stores the circle's area (computed from the radius)

## The Rectangle class
1. Define a new class named `Rectangle`.

2. Define a **parameterized constructor** (`__init__` method) to initialize a `Rectangle` with a specified **length** and **width** (both `float`). Your parameters should be assigned to **instance variables** (data attributes)

3. Within the `__init__`  method, assign a second data attribute called `area` that stores the rectangle's area (computed from the length and width)

## Using classes
Use your Circle and Rectangle classes in the following programs:
1. In a given park, a circular running track is being built. Write a program that will allow the user to enter the **outer** radius of the track and the **inner** radius, then display the total track **area**.

2. You want to create a poster that is rectangular in shape. Write a program that will allow the user to enter the **dimensions of the poster** and the **cost per square foot** for materials and print out the **cost of producing the poster**.

## Creating multiple instances of a class
In this exercise you will read student data from [students.txt](/img/students.txt) and create an instance of an object to represent each student.
1. Write a class named `Student`. It's `__init__` method should accept arguments for **last_name** (string), **first_name** (string), and **gpa** (float), and assign these values to data attributes.
    - Alternatively, `__init__` could accept a single string argument - a string line from the students.txt file. The parsing and assignment of the individual values to data attributes could then happen inside `__init__`

3. Write code to read the student data from [students.txt](/img/students.txt). Create a `Student` object for each student (each row of the file). Add the `Student` objects to a list.

4. Write a loop that checks each of the `Student` objects and prints the names of students with a GPA higher than 3.9.
