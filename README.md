### Java Weekly Assessment

## 1 ) WRITE A JAVA PROGRAM TO PRINT THE SUM,MULTIPLY,SUBTRACT,DIVIDE AND REMAINDER OD TWO NUMBERS

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

## INPUT:
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
