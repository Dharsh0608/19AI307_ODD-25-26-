# Ex.No:2(D) VARIABLE SCOPE AND CONSTRUCTOR

## QUESTION:
Write a class that uses a constructor to initialize variables and overrides toString() method.

## AIM:
To write a Java program that initializes object variables using a constructor and overrides the toString() method to display object details in a readable format.


## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Define a class Student with two instance variables:

  String name

  int age

4.Create a parameterized constructor to initialize these variables.

5.Override the toString() method to return the student details in a formatted string.

6.In the main() method:

7.Read the name and age from the user.

8.Create a Student object using the constructor.

9.Print the object, which automatically calls the overridden toString() method.

10.End the program.





## PROGRAM:
 ```
/*
Program to implement a Variable scope and Constructor using Java
Developed by: DHARSHANA A S
RegisterNumber: 212224220022
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class Student {
    String name;
    int age;

    public Student(String name, int age) {
        this.name = name;
        this.age = age;
    }

    @Override
    public String toString() {
        return "Student{name='" + name + "', age=" + age + "}";
    }
}

public class StudentDemo {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        String name = scanner.nextLine();
        int age = scanner.nextInt();

        Student student = new Student(name, age);
        System.out.println(student.toString());
    }
}

```



## OUTPUT:

<img width="896" height="395" alt="image" src="https://github.com/user-attachments/assets/406e18bf-a1c9-4ba5-ad3e-7fcf19a561c0" />



## RESULT:
Therefore the program successfully creates a student object using the constructor.
