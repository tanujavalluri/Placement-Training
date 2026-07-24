A) Write a program to print whether a number is even or odd, also take input from the user.

CODE : 

import java.util.Scanner;
public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter a number: ");
        int num = sc.nextInt();

        if (num % 2 == 0) {
            System.out.println(num + " is Even");
        } else {
            System.out.println(num + " is Odd");
        }

OUTPUT :

Enter a number: 1
1 is Odd


B) Take in two numbers and an operator (+, -, *, /) and calculate the value. (Use if conditions)

CODE : 

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter first number: ");
        double num1 = sc.nextDouble();

        System.out.print("Enter second number: ");
        double num2 = sc.nextDouble();

        System.out.print("Enter operator (+, -, *, /): ");
        char op = sc.next().charAt(0);

        if (op == '+') {
            System.out.println("Result = " + (num1 + num2));
        } 
        else if (op == '-') {
            System.out.println("Result = " + (num1 - num2));
        } 
        else if (op == '*') {
            System.out.println("Result = " + (num1 * num2));
        } 
        else if (op == '/') {
            if (num2 != 0) {
                System.out.println("Result = " + (num1 / num2));
            } else {
                System.out.println("Division by zero is not allowed.");
            }
        } 
        else {
            System.out.println("Invalid Operator");
        }

        sc.close();
    }
}


  OUTPUT : 

  Enter first number: 3
  Enter second number: 6
  Enter operator (+, -, *, /): -
  Result = -3.0


  C) Take 2 numbers as input and print the largest number.

  CODE : 

  import java.util.Scanner;

public class LargestNumber {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter first number: ");
        int num1 = sc.nextInt();

        System.out.print("Enter second number: ");
        int num2 = sc.nextInt();

        if (num1 > num2) {
            System.out.println("Largest number = " + num1);
        } else if (num2 > num1) {
            System.out.println("Largest number = " + num2);
        } else {
            System.out.println("Both numbers are equal.");
        }

        sc.close();
    }
}



OUTPUT :

Enter first number: 2
Enter second number: 6
Largest number = 6

  
