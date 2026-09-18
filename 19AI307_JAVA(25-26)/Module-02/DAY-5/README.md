# Ex.No:2(E) ACCESS MODIFIERS

## QUESTION:
Create a class Employee with method display(). Inside display(), return the current object using this. Create another method that calls display().printName()


## AIM:
To create an Employee class where the display() method returns the current object using this, and demonstrate calling display().printName() from another method.


## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a class Employee with a variable name.

4. Write a method setName() to assign value to name.

5. Write a method display() that returns the current object using return this;.

6. Write a method printName() to print the employee name.

7.Add another method show() that internally calls display().printName().

8.In the main() method, read the employee name from the user.

9.Create an Employee object and set the name.

10.Call both display().printName() and show() to demonstrate method chaining.





## PROGRAM:
 ```
/*
Program to implement a Access Modifiers using Java
Developed by: DHARSHANA A S
RegisterNumber: 212224220022
*/
```


## SOURCE CODE:
```
import java.util.Scanner;

class Employee {
    String name;

    void setName(String name) {
        this.name = name;  
    }

    Employee display() {
        return this;  
    }

    void printName() {
        System.out.println("Employee Name: " + name);
    }
}

class prog {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        String inputName = scanner.nextLine();

        Employee emp = new Employee();
        emp.setName(inputName);
        emp.display().printName();  
    }
}
```






## OUTPUT:
<img width="686" height="326" alt="image" src="https://github.com/user-attachments/assets/16eac874-7afc-42a2-bc6f-86da23f99f13" />



## RESULT:
Therefore the program successfully returns the current object using this inside the display() method.
