# Checking-Whether-the-Number-is-Harshad-or-not-using-Python



Checking Whether the Number is Harshad or not using Python
Check Whether or Not a Number is a Harshad Number in Python
Given an integer input the objective is to check whether or not the given number is a Harshad Number or not. To do so we’ll check if the sum of the digits can perfectly divide the number or not. We’ll write a Program to Check Whether or Not a Number is a Harshad Number in Python Language.

Example
Input : 21
Output : Yes It's a Harshad Number
Check Whether or Not a Number is a Harshad Number in Python Language
Given an integer number as the input, the objective is to check whether or not the number is a Harshad Number by checking if the number is divisible by the sum of it’s digits or not. For a Number to be a Harshad Number, it’s must be divisible by the sum of it’s digits. Check out the below mentioned example for better understanding.

Harshad Number
A Number that is divisible by the sum of it's digits is known as a Harshad number.
Let's try and understand it even better using an example,

Example
Input : 21
Output : Yes ' It's a Harshad Number.
Explanation : The sum of the digits of 21 is 3 i.e 2 + 1. As the number 21 is divisible by 3, It's a Harshad Number.
Therefore, for any number to be a Harshad number, it must be divisible by the sum of it’s digits. Mentioned below are the working and the code to Check Whether or Not a Number is a Harshad Number in Python Language. We’ll use to following methods,

Method 1: Using Iteration I
Method 2: Using Iteration II
Let’s discuss the above mentioned methods in detail in the upcoming sections.


Method 1: Using Iteration I
Working
In this method we’ll use the while loop to extract the digits and sum them up. Once we get the sum we’ll divide the number with sum and check for divisibility.

For a given integer input,we’ll perform the following operations

Duplicate the number using a p variable.
Create an empty list for collecting all the digits.
Run a while loop until the duplicate is 0.
Extract the digits using Modulo operator “%”.
Append the digit to the list.
Shorten the number using divide operator “/”.
Get the sum of all the elements in the list.
Check if the number is divisible by sum.
Let’s implement the above mentioned Logic in Python Language.

Python Code
Run
n = 21
p=n
l=[]
sum1=0
while(n>0):
    x=n%10
    l.append(x)
    n=n//10
sum1=sum(l)
if(p%sum1==0):
    print("Harshad number")
else:
    print("Not harshad number")
Output
It's a Harshad Number
Method 2: Using Iteration II
Working
This method is the improvised version of method 1. In this method we’ll use while loop to extract the digits but instead of appending the digits to a list, we’ll directly add them to the sum variable.

For a given integer input as number, we perform the following operations

Duplicate the number using a p variable.
Run a while loop until the duplicate is 0.
Extract the digits using Modulo operator “%”.
Append the digit to the sum variable.
Shorten the number using divide operator “/”.
Check if the number is divisible by sum.
Let’s implement the above mentioned logic in Python Language.

Python Code
Run
n = 21
p=n
sum1=0
while(n>0):
    sum1+=n%10
    n=n//10
if(p%sum1==0):
    print("Harshad number")
else:
    print("Not harshad number")
Output
It's a Harshad Number
