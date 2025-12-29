# Learning-Javascript
A code repo for Learning JavaScript 



# Overview

Everything in **C#** is associated with **classes** and **objects**, along with their **attributes** and **methods**.

**Example (Real Life Analogy):**  
A **car** is an object.  
- **Attributes:** weight, color  
- **Methods:** drive, brake  

A **Class** is like an object constructor or a **blueprint** for creating objects.

---

## Purpose of Classes

- Organize code in a structured way  
- Represent real-world entities in programming  
- Reuse code and reduce duplication  

---

## Importance in Object-Oriented Programming (OOP)

Classes form the foundation of OOP concepts such as:

- Encapsulation  
- Inheritance  
- Polymorphism  
- Abstraction  

> Without classes, object-oriented design is not possible in C#.

---

## Components of a Class

### 1. Fields / Variables
Store data about the object.

```csharp
public string Name;
public int Age;
Methods / Functions
Define the behavior of the object.
public void ShowDetails()
{
    Console.WriteLine("Name: " + Name);
    Console.WriteLine("Age: " + Age);
}
``` 
### 2. Constructors
A special method used to initialize objects.

```csharp
public Student(string name, int age)
{
    Name = name;
    Age = age;
}
```
### 3. Access Modifiers
Control access to class members.
- public
- private
- protected
- internal

### Access Modifiers Explained
#### 1. Private Modifier
Accessible only within the same class.
```csharp
class Car
{
    private string model = "Mustang";

    static void Main(string[] args)
    {
        Car myObj = new Car();
        Console.WriteLine(myObj.model);
    }
}
```
#### Output:
Mustang
Accessing it outside the class will cause an error.

#### 2. Public Modifier
Accessible from all classes.
```csharp
class Car
{
    public string model = "Mustang";
}

class Program
{
    static void Main(string[] args)
    {
        Car myObj = new Car();
        Console.WriteLine(myObj.model);
    }
}
```
#### Output:

Mustang
By default, all members of a class are private if no access modifier is specified.

#### 3. Protected Modifier
Accessible within the same class or in a derived (inherited) class.

#### 4. Internal Modifier
Accessible only within the same assembly, not from another assembly.
--- 
## Creating a Class
Use the class keyword to create a class.
```csharp
class Car

{
    string color = "red";
}
Using Multiple Classes
Classes can be separated into different files for better organization.
class Car
{
    public string color = "red";
}
class Program
{
    static void Main(string[] args)
    {
        Car myObj = new Car();
        Console.WriteLine(myObj.color);
    }
}
```

---
## Constructors

A constructor:

- Has the same name as the class
- Is called automatically when an object is created
- Is used to initialize fields
- Class and Object Relationship
- A class is a blueprint
- An object is an instance of that class
- Multiple objects can be created from one class, each with its own data
- Practical Usage of Classes
- Classes are commonly used to model real-world entities such as:
     - Students in educational systems
     - Employees in organizations
     - Accounts in banking applications
- Each entity is represented as a class with relevant data and operations.