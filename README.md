

# C++ Constructors and Destructors

This repository contains explanations and logic for different types of constructors and destructors in C++.

---

## 1. Default Constructor (Inside Class)

**Aim:**  
To implement a default constructor inside the class.

**Theory:**  
- A default constructor is automatically called when an object is created.  
- It takes no arguments and assigns default values to data members.  

**Syntax:**  
```cpp
ClassName() {
   // initialization
}

Logic:

Define constructor inside the class.

Assign default values to members.

Create an object → constructor is executed.



---

2. Default Constructor (Outside Class)

Aim:
To implement a default constructor outside the class.

Theory:

A constructor can be declared inside the class but defined outside using the scope resolution operator ::.


Syntax:

ClassName::ClassName() {
   // initialization
}

Logic:

Declare constructor in the class.

Define it outside with ClassName::.

Initialize members with default values.



---

3. Parameterized Constructor

Aim:
To implement a parameterized constructor.

Theory:

A parameterized constructor takes arguments.

It allows initializing data members with custom values at object creation.


Syntax:

ClassName(type arg1, type arg2) {
   // initialization
}

Logic:

Pass values while creating object.

Constructor assigns these values to data members.

Different objects can be initialized with different values.



---

4. Copy Constructor

Aim:
To implement a copy constructor.

Theory:

A copy constructor initializes a new object as a copy of an existing object.

Takes a reference to another object of the same class.


Syntax:

ClassName(const ClassName &obj) {
   // copy values
}

Logic:

Copy constructor receives another object as input.

Copies the values of its members into the new object.

Used when creating duplicate objects.



---

5. Copy Constructor (Q2 – Multiple Attributes)

Aim:
To implement a copy constructor for objects having multiple attributes (e.g., name, price, author).

Logic:

Define a parameterized constructor to initialize multiple values.

Create a copy constructor that takes a reference object.

Copy each attribute (like name, price, author) into the new object.

Demonstrates deep/shallow copy behavior.



---

6. Destructor

Aim:
To implement a destructor in C++.

Theory:

Destructor is a special function called automatically when an object goes out of scope.

It has the same name as the class with a ~ prefix.

Used for cleanup tasks like freeing memory or closing files.


Syntax:

~ClassName() {
   // cleanup
}

Logic:

Define destructor inside the class.

Destructor is automatically called when object is destroyed.

Useful for memory management and resource cleanup.



---

📌 Summary

Default Constructor → Initializes objects with default values.

Parameterized Constructor → Initializes objects with specific values.

Copy Constructor → Creates a new object as a copy of another.

Destructor → Performs cleanup when an object is destroyed.


---



