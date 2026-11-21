# OOP-LAB-TASK-3

Employee and Manager (Java)

A small Java program I wrote to practice method overriding along with inheritance. It's a console program with two classes, Employee and Manager, and a main class that creates one of each and prints their details.

An employee has a name and a salary. A manager is also an employee, but with a department added on top. So instead of rewriting everything, Manager extends Employee.

How it's set up

Employee is the parent class. It has name and salary, and a displayDetails() method that prints both.

Manager extends Employee and adds a department field. It also has its own version of displayDetails(). That's the overriding part: same method name as the parent, but it does a bit more. Inside it I call super.displayDetails() to print the name and salary using the parent's code, and then print the department after that.

Detail is the main class. It creates an Employee and a Manager and calls displayDetails() on each one. Since the two objects have different classes, the same method call gives different output.

Running it

What it prints
Name = Alam
Salary = 95000.0
Name = Mahmood
Salary = 150000.0
Department = CS
