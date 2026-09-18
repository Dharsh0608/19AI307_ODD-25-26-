# Ex.No:5(C)  FILE HANDLING USING JAVA
## QUESTION:
Write a Java program to create a new file named example.txt.

## AIM:
To write a Java program that creates a new file named example.txt using the File class and handles any possible I/O exceptions.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a File object pointing to "example.txt".

4.Call the createNewFile() method to attempt creating the file.

5.If the method returns true, print that the file was created.

6.If it returns false, print that the file already exists.

7.Surround the file-creation logic with a try–catch block to handle IOException.





## PROGRAM:
 ```
/*
Program to implement a File Handling using Java
Developed by: DHARSHANA A S
RegisterNumber: 212224220022 
*/
```

## SOURCE CODE:
```
import java.io.File;
import java.io.IOException;

public class CreateNewFileExample {
    public static void main(String[] args) {
        try {
            File file = new File("example.txt");
            if (file.createNewFile()) {
                System.out.println("File created: " + file.getName());
            } else {
                System.out.println("File already exists.");
            }
        } catch (IOException e) {
            System.out.println("An error occurred: " + e.getMessage());
        }
    }
}
```

## OUTPUT:

<img width="768" height="255" alt="image" src="https://github.com/user-attachments/assets/fb4c5016-7ebf-4102-a2ec-66b948e787a2" />


## RESULT:
Therefore the program successfully creates a new file named example.txt if it does not already exist.
