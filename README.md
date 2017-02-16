a. Write a Java code with the class name, “acad,” and a method called “main.”Hard code the program with two integers and print the sum of those two integers.

import java.util.Scanner;
public class acad {
public static void main(String args[]){
	Scanner sc=new Scanner(System.in);
	int sum;
	int a = 5;int b = 10;//input intialized in the program
	sum=a+b;
	System.out.println(sum);//display sum as 15
	
}
}



b. Rewrite the above code, where in the inputs are provided by the user at runtime and the output is printed.

import java.util.*;
public class acad {
public static void main(String args[]){
	Scanner sc=new Scanner(System.in);
	int a=sc.nextInt();//input from user
	int b=sc.nextInt();//input from user
	int sum;
	sum=a+b;
	System.out.println(sum);//display sum of two number
	
}
}


c. Write a program with the method name, “sum()” that accepts two parameters from the user and print the sum of those two numbers. The
output format should be:
First number is:
Second number is:
Sum is:

import java.util.*;
 public class acad {
 public static void main(String arg[]){//method name main
 Scanner sc=new Scanner(System.in);
int a=sc.nextInt();//getting input from user
int b=sc.nextInt();//getting input from user
sum(a,b);
 }
public static void sum(int x,int y) { //method name sum
	
int sum =x+y;
	
System.out.println(sum);//display the sum of values of(x and y)
}

}


d. Write a program to accept two numbers from “stdin” and find all the odd as well as even numbers present in between them.


import java.util.*;
public class Main {
	public static void main(String args[])
	{
		Scanner s=new Scanner(System.in);
		int a =s.nextInt(); //getting first number from user
		int b=s.nextInt(); //getting second number from user
		System.out.println("The even numbers are:");
for(int i=a;i<=b;i++)
{
	if(i%2==0)
		System.out.println(i);//display even numbers from input
}
System.out.println("The odd numbers are:");
for(int i=a;i<=b;i++)
{
	if(i%2!=0)
		System.out.println(i);//display odd numbers from input
}
	}

}
e. Joe is scared to go to school. When her dad asked for the reason, Joe said that she was unable to complete the task given to her by her teacher. The task was to find the “first 10 multiples” of the number entered from “stdin”.
Example:
Input: 3

import java.util.Scanner;


public class Main {
public static void main(String args[]){
	Scanner s=new Scanner(System.in);
	int a=s.nextInt();//getting from user
	for(int i=1;i<=10;i++)//defining loop
	{
		System.out.println(a+"*"+i+"="+(a*i));//printing multiplication values(output)
	}
}
}


f. Write a program consisting the method “sum()” and demonstrate the concept of method overloading using this method.

import java.util.Scanner;


public class Main {
public static void main(String args[])
{
	Scanner s=new Scanner(System.in);
System.out.println("1.Sum of two numbers \n2.Sum of three numbers");  
int i =s.nextInt();
if(i==1){
System.out.println("Enter two numbers");
int x=s.nextInt();
int y=s.nextInt();
sum(x,y);  //calling the method sum which accepts two integers
}
if(i==2){ System.out.println("Enter three numbers");
int b=s.nextInt();
int c=s.nextInt();
int d=s.nextInt();
sum(b,c,d);  //calling the method sum which accepts three integers
}
}
public static void sum(int a,int b)  //creating a method sum which accepts two integers
{
	System.out.println("Sum of two numbers are "+(a+b));
}
public static void sum(int a,int b,int c) //creating a method sum which accepts three integers
{
	System.out.println("Sum of three numbers are "+(a+b+c));
}
}


g. Can you overload a method with the same return type? Explain your answer with proper logic.
import java.util.Scanner;


public class Main {
public static void main(String args[])
{
	Scanner s=new Scanner(System.in);
System.out.println("1.Sum of two numbers \n2.Sum of three numbers");  
int i =s.nextInt();
if(i==1){
System.out.println("Enter two numbers");
int x=s.nextInt();
int y=s.nextInt();
sum(x,y);  //calling the method sum which accepts two integers
}
if(i==2){ System.out.println("Enter three numbers");
int b=s.nextInt();
int c=s.nextInt();
int d=s.nextInt();

int r=sum(b,c,d);  //calling the method sum which accepts three integers
}

}
public static int sum(int a,int b)  //creating a method sum which accepts two integers
{
	return (a+b);
}
public static int sum(int a,int b,int c) //creating a method sum which accepts three integers
{
	return (a+b+c);
}
}

h. Write a program in Java using Arrays, that sorts the element in a descending order.



import java.util.Arrays;
import java.util.Scanner;
public class acad {
public static void main(String args[])
{
	Scanner s=new Scanner(System.in);
System.out.println("Enter the number of elements in array ");
int n=s.nextInt(); //getting the size of the array
System.out.println("Enter the elements in array");
int[] a=new int[n];  //defining an integer array of size n
for(int i=0;i<n;i++)
{
 	a[i]=s.nextInt();   //getting the value from user for the array
}
Arrays.sort(a);  //sort the elements present in the array in ascending order
System.out.println("Array in descending order");
for(int i=n-1;i>=0;i--)     //loop which is used to print it in a reverse order
{
	System.out.println(a[i]);
}
}
}
