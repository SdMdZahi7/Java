# Java Weekly Assessment

## 1 ) WRITE A JAVA PROGRAM TO PRINT THE SUM,MULTIPLY,SUBTRACT,DIVIDE AND REMAINDER OF TWO NUMBERS
## INPUT CODE:
~~~
import java.util.Scanner;
public class calculator
{
    public static void main(String[]args)
    {
        Scanner sc=new Scanner(System.in);
        System.out.println("ENTER THE VALUE OF A");
        int a=sc.nextInt();
        System.out.println("ENTER THE VALUE OF B");
        int b=sc.nextInt();
        int sum=a+b;
        int subtract=a-b;
        int multiply=a*b;
        int divide=a/b;
        int remainder=a%b;
        System.out.println("THE ADDITION OF TWO NUMBERS IS:");
        System.out.println(sum);
        System.out.println("THE SUBTRACTION OF TWO NUMBERS IS:");
        System.out.println(subtract);
        System.out.println("THE MULTIPLICATION OF TWO NUMBERS IS:");
        System.out.println(multiply);
        System.out.println("THE DIVISION OF TWO NUMBERS IS:");
        System.out.println(divide);
        System.out.println("THE REMAINDER OF TWO NUMBERS IS:");
        System.out.println(remainder);
    }
}
~~~

## OUTPUT:
![wt1 2](https://user-images.githubusercontent.com/94187572/224473042-cc639cef-f316-4ccb-9ea9-d6da423623f9.png)

## 2)WRITE A JAVA PROGRAM TO COMPARE TWO NUMBERS
## INPUT CODE:
~~~
import java.util.Scanner;
public class compare
{
    public static void main(String[]args)
    {
        Scanner sc=new Scanner(System.in);
        System.out.println("ENTER THE FIRST NUMBER:");
        int a=sc.nextInt();
        System.out.println("ENTER THE SECOND NUMBER:");
        int b=sc.nextInt();
        if(a>b)
        {
            System.out.println(a+">"+b);
        }
        else if(a<b)
        {
            System.out.println(a+"<"+b);
        }
        else if(a==b)
        {
            System.out.println(a+"=="+b);
        }
        else
        {
            System.out.println(a+" is not equal to"+b);
        }

    }
}
~~~
## OUTPUT:
![WT 2 21](https://user-images.githubusercontent.com/94187572/224473213-5171c24c-e2c5-4710-bebb-86bc9739c31c.png)

## 3)WRITE A JAVA PROGRAM TO CONVERT A STRING TO AN INTEGER
## INPUT CODE:
~~~
import java.util.Scanner;
public class convert
{
    public static void main(String[]args)
    {
        int n=Integer.valueOf("-7");
        System.out.println("Number is ="+n);

    }
}
~~~
## OUTPUT:
![wt3 2](https://user-images.githubusercontent.com/94187572/224473409-e81507b6-6182-4f00-8d62-e9acff32c1b6.png)

## 4) WRITE A JAVA PROGRAM TO FIND THE AREA OF A RHOMBUS
## INPUT CODE:
~~~
import java.util.Scanner;
public class rhombus
{
    public static void main(String[]args)
    {
        Scanner sc=new Scanner(System.in);
        System.out.println("ENTER THE LENGTH OF DIAGONAL 1");
        float d1= sc.nextFloat();
        System.out.println("ENTER THE LENGTH OF DIAGONAL 2");
        float d2= sc.nextFloat();
        float area=(d1*d2)/2;
        System.out.println("THE AREA OF THE RHOMBUS IS ");
        System.out.println(area);
    }
}
~~~
## OUTPUT:
![wt4 2](https://user-images.githubusercontent.com/94187572/224473554-2e0b302c-d4a8-4f9c-b1e9-b3f6610b43a8.png)

## 5) WRITE A JAVA PROGRAM TO FIND THE NO OF DAYS IN A MONTH
## INPUT CODE:
~~~

import java.util.Scanner;

public class days{

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
      int year = scanner.nextInt();
        int month = scanner.nextInt();
        System.out.println(day(year,month));
    }
    private static int day(int year, int month) {
        int no_of_days=0;
        if(month==1){
            no_of_days = 31;
        }
        else if(month==2){
            if((year%400==0) || ((year%100!=0) && (year%4==0))){
                no_of_days= 29;
            }
            else {
                no_of_days= 28;
            }
        }
        else if(month==3){
            no_of_days = 31;
        }
        else if(month==4){
            no_of_days = 30;
        }
        else if(month==5){
            no_of_days = 31;
        }
        else if(month==6){
            no_of_days = 30;
        }
        else if(month==7){
            no_of_days = 31;
        }
        else if(month==8){
            no_of_days = 31;
        }
        else if(month==9){
            no_of_days = 30;
        }
        else if(month==10){
            no_of_days = 31;
        }
        else if(month==11){
            no_of_days = 30;
        }
        else if(month==12){
            no_of_days = 31;
        }
        System.out.println("THE NUMBER OF DAYS IS:");
        return no_of_days;
    }
}
~~~
## OUTPUT:
![wt5 3](https://user-images.githubusercontent.com/94187572/224473616-5ef4cfce-fead-4f3c-bae7-5c3b2645402a.png)
 
 ## 6 ) WRITE A JAVA PROGRAM TO PRINT THE EVEN NUMBERS FROM 1 TO 20
 ## INPUT CODE:
 ~~~
 import java.util.Scanner;
public class even
{
    public static void main(String[]args)
    {
        System.out.println(" THE EVEN NUMBERS BETWEEN 1 TO 20 ARE:");
        for(int i=1;i<=20;i++)
        {
            if(i%2==0)
            {
                System.out.println(i);
            }
        }
    }
}
~~~
## OUTPUT:
![wt6 2](https://user-images.githubusercontent.com/94187572/224473729-6aa06ff8-43e1-47c9-8a8d-c0ee29feb4e3.png)

## 7 ) WRITE A JAVA PROGRAM TO CREATE A SIMPLE CALCULATOR
## INPUT CODE:
~~~
import java.util.Scanner;
public class calculator
{
    private static Scanner sc;
    public static void main(String[] args)
    {
        sc = new Scanner(System.in);
        double a, b, result;
        System.out.print("Please Enter any Two Numbers = ");
        a = sc.nextDouble();
        b = sc.nextDouble();
        System.out.print("Enter any Operator from +, - , /, *, % = ");
        char operator = sc.next().charAt(0);
        switch(operator)
        {
            case '+':
                result = a + b;
                break;
            case '-':
                result = a - b;
                break;
            case '*':
                result = a * b;
                break;
            case '/':
                result = a / b;
                break;
            case '%':
                result = a % b;
                break;
            default:
                System.out.println("You have entered incorrect operator");
                return;
        }
        System.out.printf("%.2f %c %.2f = %.2f", a, operator, b, result);
    }
}
~~~

## OUTPUT:
![wt7 3](https://user-images.githubusercontent.com/94187572/224473811-4dcc2757-29ea-4fd0-853d-e9eec36bcbf9.png)

## 8 ) WRITE A JAVA PROGRAM TO PRINT THE MULTIPLICATION OF A GIVEN NUMBER
## INPUT CODE:
~~~
import java.util.Scanner;

public class multiplication_table
{
    public static void main(String[] args)
    {
        Scanner sc=new Scanner(System.in);
        int num=sc.nextInt();
        System.out.println("THE MULTIPLICATION TABLE OF GIVEN NUMBER IS:");
        for(int i = 1; i <= 12; ++i)
        {
            System.out.printf("%d * %d = %d \n", num, i, num * i);
        }
    }
}
~~~
## OUTPUT:
![wt8 2](https://user-images.githubusercontent.com/94187572/224473868-fa2b9f9d-10ae-429b-95d1-654900e8445c.png)


