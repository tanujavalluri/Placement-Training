a) Program to Print Whether a Number is Even or Odd

CODE : 
  import java.util.Scanner;

public class EvenOdd {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter a number: ");
        int num = sc.nextInt();

        if (num % 2 == 0) {
            System.out.println(num + " is Even");
        } else {
            System.out.println(num + " is Odd");
        }

        sc.close();
    }
}

OUTPUT : 
Enter a number: 18
18 is Even

b) Take Name as Input and Print a Greeting Message

CODE : 

  import java.util.Scanner;

public class Greeting {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter your name: ");
        String name = sc.nextLine();

        System.out.println("Hello, " + name + "! Welcome.");

        sc.close();
    }
}


OUTPUT : 
Enter your name: Thanuja
Hello, Thanuja! Welcome.


c) Take Two Numbers and an Operator (+, -, *, /) and Calculate the Value

CODE : 

  import java.util.Scanner;

public class Calculator {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter first number: ");
        double a = sc.nextDouble();

        System.out.print("Enter second number: ");
        double b = sc.nextDouble();

        System.out.print("Enter operator (+, -, *, /): ");
        char op = sc.next().charAt(0);

        if (op == '+') {
            System.out.println("Result = " + (a + b));
        } else if (op == '-') {
            System.out.println("Result = " + (a - b));
        } else if (op == '*') {
            System.out.println("Result = " + (a * b));
        } else if (op == '/') {
            if (b != 0) {
                System.out.println("Result = " + (a / b));
            } else {
                System.out.println("Division by zero is not allowed.");
            }
        } else {
            System.out.println("Invalid Operator");
        }

        sc.close();
    }
} 


OUTPUT :
Enter first number: 15
Enter second number: 5
Enter operator (+, -, *, /): *
Result = 75.0

  
