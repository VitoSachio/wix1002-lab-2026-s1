# Tutorial 3 -Answers
## Q1
```java
    import java.util.Scanner;

    public class answers {
    public static void main(String[] args) {
    
        Scanner input = new Scanner(System.in);
        
        System.out.print("Enter the first Integer: ");
        int num1 = input.nextInt();
        System.out.print("Enter the second Integer: ");
        int num2 = input.nextInt();
        System.out.print("Enter an operator (+, -, *, /, %): ");
        char operator = input.next().charAt(0);
        
        if (operator == '+') {
            System.out.println(num1 + num2);
        } else if (operator == '-') {
            System.out.println(num1 - num2);
        } else if (operator == '*') {
            System.out.println(num1 * num2);
        } else if (operator == '/') {
            System.out.println(num1 / num2);
        } else if (operator == '%') {
            System.out.println(num1 % num2);
        } else {
            System.out.println("Invalid operator");
        }
      }
    }
```
## Q2
```
    import java.util.Random;

    public class answers {
    public static void main(String[] args) {
        Random random = new Random();
        int number = random.nextInt(6);

        String word;
        switch (number) {
            case 0:
                word = "Zero";
                break;
            case 1:
                word = "One";
                break;
            case 2:
                word = "Two";
                break;
            case 3:
                word = "Three";
                break;
            case 4:
                word = "Four";
                break;
            default:
                word = "Five";
                break;
           }
          System.out.println(number +" is "+ word);
        }
    }
```
## Q3
```
    import java.util.Scanner;

    public class Jawaban {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.print("Enter the sales volume: ");
        double sales = input.nextDouble();

        double commission;

        if (sales <= 100) {
            commission = sales * 0.05;
        } else if (sales <= 500) {
            commission = sales * 0.075;
        } else if (sales <= 1000) {
            commission = sales * 0.10;
        } else {
            commission = sales * 0.125;
        }

        System.out.printf("Commission: %.2f%n", commission);
        }
    }
```
## Q4
```
    import java.util.Random;

    public class answers {
    public static void main(String[] args) {
        Random random = new Random();

        int player1 = (random.nextInt(6) + 1) + (random.nextInt(6) + 1);
        int player2 = (random.nextInt(6) + 1) + (random.nextInt(6) + 1);

        System.out.println("Player 1: " + player1);
        System.out.println("Player 2: " + player2);

        if (player1 > player2) {
            System.out.println("Player 1 wins");
        } else if (player2 > player1) {
            System.out.println("Player 2 wins");
        } else {
            System.out.println("Draw");
        }
        }
    }
```
## Q5
```
    import java.util.Scanner;

    public class answers {
    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        double a = in.nextDouble(), b = in.nextDouble(), c = in.nextDouble();
        double d = in.nextDouble(), e = in.nextDouble(), f = in.nextDouble();

        double k = a * d - b * c;

        if (k == 0)
            System.out.println("The equation has no solution");
        else
            System.out.println("x = " + (e * d - b * f) / k + ", y = " + (a * f - e * c) / k);
      }
    }
```
## Q6
```
    import java.util.Scanner;

    public class answers {
    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        double r = in.nextDouble(), x = in.nextDouble(), y = in.nextDouble();

        System.out.println(x * x + y * y <= r * r ? "inside" : "outside");
      }
    }
```
