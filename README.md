# Occurrence-of-a-digit-in-a-given-number-using-Java

Occurrence of a digit in a given number using Java
In this page we will discuss the program to find the occurrence of a digit in a given number using java programming language. We are given with a number and a digit and need to count the number of occurrence of that digit in the given number.

Method Discussed :
Method 1 : Using loops.
Method 2 : Using string.
Method 1 :
Declare variable count that will count the required number of occurrences
Take a while loop.
Declare a variable rem to store every digit of the number to be compared.
Compare rem with the digit
if rem equals digit increment count.
n=n/10
Print the value of count.
Method 1 : Code in java
Run
//Write a program to print the Occurrence of a Digit in a given Number in Java
import java.io.*;
import java.util.*;

class Main{

    public static void main (String[] args) 

    {
 
        int n = 898989, count = 0;

        int d = 9;

        while(n>0){
            int rem = n%10;
            if(rem == d)
                count++;
            n /= 10;
        }
        System.out.println(count);

    }

}
Output:
3
Related Pages
Convert digit/number to words

Counting number of days in a given month of a year
 
Finding number of integers which has exactly x divisors

Finding Roots of a quadratic equation

Power of a Number 

Method 2 :
 Declare a variable count = 0, to count the required occurrence.
Take a for loop.
Declare a variable i to iterate over every character of string.
Compare each character with the digit
if  character equals digit increment count.
Print the value of count.
End
Method 2 : Code in java
Run
//Write a program to print the Occurrence of a Digit in a given Number in Java
import java.io.*;
import java.util.*;

class Main{

    public static void main (String[] args) 

    {
 
        int x = 898989, c = 0;

        char b = '9';

        String s = Integer.toString(x);

        for(int i=0;i<s.length();i++){

            if(s.charAt(i)==b)
                c=c+1;
        }
        System.out.println(c);

    }

}
Output:
3
