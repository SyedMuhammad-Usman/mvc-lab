
# Student Management System in Java

This repository demonstrates the application of the **MVC (Model-View-Controller)** architecture in Java. It showcases how to design software with proper separation of concerns and reusable components.

---

## **Task: MVC Architecture (Student Management)**

### Overview:
This project implements the **MVC (Model-View-Controller)** architecture, separating concerns into:
- **Model**: Manages the data and business logic.
- **View**: Handles the user interface and displays information to the user.
- **Controller**: Acts as the intermediary, processing user inputs, updating the model, and refreshing the view.

### Code Details:
1. **Model**:
   - Represents the `Student` entity storing student data such as name, age, and GPA.
2. **View**:
   - Displays the student details to the console.
3. **Controller**:
   - Coordinates between the `Model` and `View` to process data.

---

### Key Concepts:

#### **Aggregation**:
- **Aggregation** is used between the `Controller` and both the `Model` and `View`.
- The `Controller` **has-a** relationship with the `Model` (`Student`) and the `View`.
- The lifecycle of the `Student` and `View` is independent of the `Controller`.

#### **How Aggregation is Used**:
- The `Controller` class holds references to the `Student` (Model) and `StudentView` (View).
- These references allow the `Controller` to manipulate the model data and update the view without owning their lifecycle.

---

### Execution:
To run the code:
1. Clone this repository.
2. Open the project in any Java IDE (e.g., IntelliJ IDEA).
3. Navigate to `MVC_pkg.Main`.
4. Run the `Main` class.

---

### Output:
When the program runs, it displays all students' details, demonstrating the coordination between Model, View, and Controller.

Example:
```
Student Name: Usman, Age: 20, GPA: 3.6
Student Name: Ali, Age: 20, GPA: 4.0
Student Name: Hadi, Age: 20, GPA: 3.7
Student Name: Umer, Age: 20, GPA: 3.3
```

---

## **File Structure**
```
src/
└── MVC_pkg/
    ├── Student.java
    ├── StudentView.java
    ├── Controller.java
    └── Main.java
```

---

## **Technologies Used**
- Java
- IntelliJ IDEA
