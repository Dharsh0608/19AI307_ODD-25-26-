# Ex.No:3(b) POLYMORPHISM

## QUESTION:
Write a Java program to create a class Vehicle with a method called speedUp(). Create two subclasses Car and Bicycle. Override the speedUp() method in each subclass to increase the vehicle's speed differently.


## AIM:
To create a Java program demonstrating method overriding by defining a base class Vehicle with a speedUp() method and overriding it in subclasses Car and Bicycle to increase speed differently.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a parent class Vehicle with an integer variable speed and a method speedUp(int increment) that increases speed normally.

4.Create a subclass Car that overrides speedUp() to increase speed by double the increment.

5.Create a subclass Bicycle that overrides speedUp() to increase speed normally (same as parent but customized message).

6.Read vehicle type and increment value from user.

7.Based on the type, create an object of Car, Bicycle, or Vehicle.

8.Call the speedUp(increment) method to show polymorphic behavior.





## PROGRAM:
 ```
/*
Program to implement a Polymorphism using Java
Developed by: DHARSHANA A S
RegisterNumber: 212224220022  
*/
```

## SOURCE CODE:

```
import java.util.Scanner;

// Parent class
class Vehicle {
    int speed = 0;

    void speedUp(int increment) {
        speed += increment;
        System.out.println("Vehicle speed increased to: " + speed + " km/h");
    }
}


class Car extends Vehicle {
    @Override
    void speedUp(int increment) {
        speed += increment * 2;
        System.out.println("Car speed increased to: " + speed + " km/h");
    }
}


class Bicycle extends Vehicle {
    @Override
    void speedUp(int increment) {
        speed += increment;
        System.out.println("Bicycle speed increased to: " + speed + " km/h");
    }
}


public class TestVehicles {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String type = sc.nextLine().toLowerCase();
        int increment = sc.nextInt();

        Vehicle vehicle;
        if (type.equals("car")) {
            vehicle = new Car();
        } else if (type.equals("bicycle")) {
            vehicle = new Bicycle();
        } else {
            vehicle = new Vehicle();
        }

        vehicle.speedUp(increment);
    }
}
```





## OUTPUT:
<img width="921" height="437" alt="image" src="https://github.com/user-attachments/assets/3dec864e-a5e2-4af5-9115-0ccef271f50d" />




## RESULT:
Therefore the program successfully demonstrates method overriding by applying different speed increase behaviors for car and bicycle.
