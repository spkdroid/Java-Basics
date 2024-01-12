# Java-Basics

Below is a simple tutorial that covers basic programs in Java to demonstrate input and output, control structures, and exception handling. 

### Program 1: Input and Output

```java
import java.util.Scanner;

public class InputOutputDemo {
    public static void main(String[] args) {
        // Input using Scanner
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter your name: ");
        String name = scanner.nextLine();

        System.out.print("Enter your age: ");
        int age = scanner.nextInt();

        // Output using System.out.println
        System.out.println("Hello, " + name + "! You are " + age + " years old.");

        // Close the scanner
        scanner.close();
    }
}
```

### Program 2: Control Structures

```java
import java.util.Scanner;

public class ControlStructuresDemo {
    public static void main(String[] args) {
        // Input using Scanner
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter a number: ");
        int number = scanner.nextInt();

        // Control Structure (Finding Odd or Even)
        if (number % 2 == 0) {
            System.out.println(number + " is an even number.");
        } else {
            System.out.println(number + " is an odd number.");
        }

        // Close the scanner
        scanner.close();
    }
}
```

### Program 3: Exception Handling

```java
import java.util.Scanner;

public class ExceptionHandlingDemo {
    public static void main(String[] args) {
        // Input using Scanner
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter a number: ");

        try {
            int number = scanner.nextInt();

            // Output
            System.out.println("You entered: " + number);
        } catch (Exception e) {
            // Exception Handling
            System.out.println("Error: Invalid input. Please enter a valid number.");
        } finally {
            // Close the scanner
            scanner.close();
        }
    }
}
```

### Program 4: Conversion - Kilograms to Pounds

```java
import java.util.Scanner;

public class KilogramsToPoundsConverter {
    public static void main(String[] args) {
        // Input using Scanner
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter weight in kilograms: ");
        double weightInKilograms = scanner.nextDouble();

        // Conversion
        double weightInPounds = weightInKilograms * 2.20462;

        // Output
        System.out.println(weightInKilograms + " kilograms is equal to " + weightInPounds + " pounds.");

        // Close the scanner
        scanner.close();
    }
}
```

### Program 5: Simple Arithmetic

```java
import java.util.Scanner;

public class ArithmeticOperations {
    public static void main(String[] args) {
        // Input using Scanner
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter the first number: ");
        double num1 = scanner.nextDouble();

        System.out.print("Enter the second number: ");
        double num2 = scanner.nextDouble();

        // Arithmetic Operations
        double sum = num1 + num2;
        double difference = num1 - num2;
        double product = num1 * num2;
        double quotient = num1 / num2;

        // Output
        System.out.println("Sum: " + sum);
        System.out.println("Difference: " + difference);
        System.out.println("Product: " + product);
        System.out.println("Quotient: " + quotient);

        // Close the scanner
        scanner.close();
    }
}
```

### Program 6: Loops

```java
import java.util.Scanner;

public class LoopDemo {
    public static void main(String[] args) {
        // Input using Scanner
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter the number of times to print 'Hello': ");
        int count = scanner.nextInt();

        // Loop to print 'Hello'
        for (int i = 0; i < count; i++) {
            System.out.println("Hello");
        }

        // Close the scanner
        scanner.close();
    }
}
```

### Program 7: Complex Exception Handling

```java
import java.util.Scanner;

public class ComplexExceptionHandling {
    public static void main(String[] args) {
        // Input using Scanner
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter the numerator: ");
        int numerator = scanner.nextInt();

        System.out.print("Enter the denominator: ");
        int denominator = scanner.nextInt();

        // Complex Exception Handling
        try {
            double result = divide(numerator, denominator);
            System.out.println("Result of division: " + result);
        } catch (ArithmeticException ae) {
            System.out.println("Error: " + ae.getMessage());
        } catch (Exception e) {
            System.out.println("Unexpected error: " + e.getMessage());
        } finally {
            // Close the scanner
            scanner.close();
        }
    }

    // Custom method for division
    private static double divide(int numerator, int denominator) {
        if (denominator == 0) {
            throw new ArithmeticException("Cannot divide by zero.");
        }
        return (double) numerator / denominator;
    }
}
```
