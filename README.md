# Switchcase
import java.util.Scanner;

public class SwitchCaseExample {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

// Input: two numbers and an operator
System.out.print("Enter the first number: ");
double num1 = scanner.nextDouble();
System.out.print("Enter the second number: ");
double num2 = scanner.nextDouble();
System.out.println("Choose an operation: +, -, *, /");
char operator = scanner.next().charAt(0);
double result;

// Switch case to perform operations
switch (operator) {
        case '+':
        result = num1 + num2;
              System.out.println("Result: " + result);
break;

case '-':
    result = num1 - num2;               System.out.println("Result: " +result);
    break;
    case '*':
      result = num1 * num2;
      System.out.println("Result: " + result);
      break;
      case '/':
        if (num2 != 0) {
        result = num1 / num2;
        System.out.println("Result: " + result);
         } else {
         System.out.println("Error: Division by zero is not allowed.");
                }
                break;
                default:          System.out.println("Invalid operation! Please choose +, -, *, or /.");
        }
        scanner.close();
    }
}

output-
Enter the first number: 10
Enter the second number: 5
Choose an operation: +, -, *, /
+
Result: 15.0
