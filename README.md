# Vehicle Registry System

## Introduction

The Vehicle Registry System is a console-based application developed in C++ using Object Oriented Programming concepts.  
This project is designed to manage different types of vehicles such as Sedan, SUV, Sports Car, and Flying Car.

The system allows users to:
- Add vehicles
- Display all vehicle details
- Search vehicles by ID
- Count total vehicles created

This project demonstrates important OOP concepts like:
- Encapsulation
- Inheritance
- Multilevel Inheritance
- Multiple Inheritance
- Polymorphism
- Constructor Overloading
- Static Members
- Virtual Functions

Source Code Reference: :contentReference[oaicite:0]{index=0}

---

# Objectives

- To understand Object Oriented Programming concepts.
- To implement inheritance and polymorphism in C++.
- To create a vehicle management system using classes and objects.
- To practice runtime polymorphism using virtual functions.
- To understand multilevel and multiple inheritance.

---

# Features

- Add Sedan Vehicle
- Add SUV Vehicle
- Add Sports Car
- Add Flying Car
- Display All Vehicles
- Search Vehicle by ID
- Store Multiple Vehicles
- Count Total Vehicles

---

# Technologies Used

| Technology | Purpose |
|---|---|
| C++ | Programming Language |
| OOP Concepts | Program Structure |
| Console Application | User Interface |

---

# OOP Concepts Used

## 1. Encapsulation

Encapsulation means binding data and functions together inside a class.

Example:
```cpp
class Vehicle
{
protected:
   int Vehicle_id;
   string Vehicle_manufacturer;
};


2. Inheritance

Inheritance allows one class to acquire properties of another class.

Single Inheritance
class Car : public Vehicle
Multilevel Inheritance
Vehicle -> Car -> ElectricCar -> SportsCar
Multiple Inheritance
class FlyingCar : public Car, public Aircraft
3. Polymorphism

Polymorphism allows functions to behave differently.

Virtual function used:

virtual void display() const

Function overriding is implemented in derived classes.

4. Constructor Overloading

Different constructors are created for different initialization methods.

Example:

Vehicle()
Vehicle(int id, string Manufacturer, string model, int yer)
5. Static Data Member

Static member used to count total vehicles.

static int totalVehicles;
Classes Description
1. Vehicle Class

Base class for all vehicles.

Data Members
Vehicle ID
Manufacturer
Model
Year
Functions
setVehicleID()
getVehicleID()
setManufacturer()
getManufacturer()
display()
2. Car Class

Derived class from Vehicle.

Additional Data Member
Fuel Type
Function
display()
3. ElectricCar Class

Derived from Car class.

Additional Data Member
Battery Capacity
Function
display()
4. SportsCar Class

Derived from ElectricCar.

Additional Data Member
Top Speed
Function
display()
5. Sedan Class

Derived from Car.

Function
display()
6. SUV Class

Derived from Car.

Function
display()
7. Aircraft Class

Independent class for flight range.

Data Member
Flight Range
8. FlyingCar Class

Derived using Multiple Inheritance.

Parent Classes
Car
Aircraft
Function
display()
9. VehicleRegistry Class

Stores all vehicles.

Functions
addVehicle()
displayAll()
searchByID()
Program Flow
User selects menu option.
User enters vehicle details.
Vehicle object is created dynamically.
Object is stored in VehicleRegistry.
User can display or search vehicles.
Menu Driven Program
--- Vehicle Registry System ---

1. Add Sedan
2. Add SUV
3. Add Sports Car
4. Add Flying Car
5. View All Vehicles
6. Search by ID
7. Exit
Sample Output
Add Sedan
Enter Vehicle ID : 101
Enter Manufacturer : Honda
Enter Model : City
Enter Year : 2024
Enter Fuel Type : Petrol

Vehicle added successfully!
Display Vehicles
[Sedan]
ID             : 101
Manufacturer   : Honda
Model          : City
Year           : 2024
Fuel Type      : Petrol
Search Vehicle
Enter ID to search : 101
Vehicle Found
Advantages
Easy to understand
Demonstrates advanced OOP concepts
User-friendly system
Reusable code
Dynamic object handling
Limitations
Data is not stored permanently
Maximum 50 vehicles only
Console-based interface
Future Enhancements
Add file handling
Add database connectivity
Add graphical user interface
Add delete and update options
Add login system
Conclusion

The Vehicle Registry System is an excellent project for understanding Object Oriented Programming concepts in C++.
The project successfully demonstrates:

Inheritance
Polymorphism
Encapsulation
Constructor Overloading
Multiple Inheritance

This project helps students understand real-world implementation of vehicle management systems using C++.
