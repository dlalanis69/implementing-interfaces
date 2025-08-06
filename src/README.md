# Implementing Interfaces in Java

This project demonstrates how Java handles **multiple inheritance** using **interfaces**, by combining an abstract class with multiple interfaces. It models real-world roles such as students and employees, each with their specific behaviors.

## 📌 Description

The project defines:
- An abstract class `Person`, extended by the concrete classes `Student` and `Employee`.
- Two interfaces: `StudentInterface` and `EmployeeInterface`, each declaring methods related to their role.
- The `Student` and `Employee` classes implement their respective interfaces and override required methods.
- The `Main` class instantiates and displays information about a student and an employee, including salary and fee details.

## 📂 Structure

| Class/Interface        | Type             | Inherits/Implements                                 | Key Fields / Methods                                     |
|------------------------|------------------|------------------------------------------------------|----------------------------------------------------------|
| `Person`               | Abstract Class    | –                                                    | `name: String`, `age: int`; `getDetails()` *(abstract)*  |
| `StudentInterface`     | Interface         | –                                                    | `subject: String`, `marks: int`, `fee: boolean`; `getGrade()`, `hasPaidFee()` |
| `EmployeeInterface`    | Interface         | –                                                    | `basicPay: double`; `calculateSalary()`, `calculateTax()` |
| `Student`              | Concrete Class    | Extends `Person`, Implements `StudentInterface`      | `subject`, `marks`, `fee`; overrides methods             |
| `Employee`             | Concrete Class    | Extends `Person`, Implements `EmployeeInterface`     | `basicPay`; overrides methods                            |
| `Main`                 | Entry Point       | –                                                    | Creates and displays a `Student` and an `Employee`       |

## ▶️ How to Run

### Using IntelliJ IDEA
1. Open the project in IntelliJ.
2. Ensure JDK 17+ is configured.
3. Run the `Main` class.

### Using Terminal
```bash
javac *.java
java Main
```

## 🧪 Sample Output
```
Name: Charlie
Age: 20
Subject: Electronics
Marks: 75
Pass!
The student has paid the specified fee.
Name: Steve
Age: 35
Basic Pay: 50000.0
Salary: 75000.0
Tax: 5000.0
```

> Output may vary depending on the values used in `Main.java`.

## 🎓 Developed as a lab assignment for the Coursera Java Programming course.

## ✅ Requirements

- Java 17 or higher (tested with OpenJDK 24)
- IntelliJ IDEA or any Java-compatible IDE

## 💡 Key Concepts Practiced

- Combining abstract classes with interfaces
- Simulating multiple inheritance using Java interfaces
- Encapsulation and object-oriented design principles
- Calculating values based on object state (salary, tax, grades)
