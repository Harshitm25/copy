1) Write a JAVA Program to demonstrate Constructor Overloading and Method Overloading.

class A
{
A(int a,int b)
{
System.out.println("addition of integers:"+(a+b));
}
A(double a,double b)
{
System.out.println("addition of double numbers:"+(a+b));
}
void add(int a,int b)
{
System.out.println("addition of integers:"+(a+b));
}
void add(double a,double b)
{
System.out.println("addition of double numbers:"+(a+b));
}
}
class Main
{
public static void main(String args[])
{
System.out.println("constructor overloading:");
A a=new A(2,3);
A b=new A(2.4f,5.6f);
System.out.println("method overloading");
a.add(3,5);
b.add(5.6f,3.5f);
}
}

2) Write a JAVA Program to implement Inner class and demonstrate its 
                                                  Access protection.
class Outer
{
int outer_x=100;
class Inner
{
int inner_y=10;
void display()
{
System.out.println("inner_y:"+inner_y);
System.out.println("outer_x:"+outer_x);
}
}
void test()
{
Inner in=new Inner();
in.display();
//System.out.println("inner_y"+inner_y);
}
}
class Demo
{
public static void main(String args[])
{
Outer out=new Outer();
out.test();
}
}

3) string handling

import java.util.*;
import java.util.Scanner;
public class Main{
    public static void main (String[] args) {
    Scanner sc=new Scanner(System.in);
    System.out.println("enter a string");
    StringBuffer ph=new StringBuffer(sc.next());
    System.out.println("string buffer size is "+ph.capacity());
    System.out.println("reverse=:"+ph.reverse());
    System.out.println("uppercase=:"+ph.toString().toUpperCase());
        System.out.println("enter second sting:");
        String ph1=sc.next();
        sc.close();
        System.out.println("append=:"+ph.append(ph1));
    
    }
}

4) a) Write a JAVA Program to demonstrate Inheritance.

class Employee{  
 float salary=40000;  
}  
class Programmer extends Employee{  
 int bonus=10000;  
 public static void main(String args[]){  
   Programmer p=new Programmer();  
   System.out.println("Programmer salary is:"+p.salary);  
   System.out.println("Bonus of Programmer is:"+p.bonus);  
}  
}  

4) b) Program on Java for the implementation of Multiple inheritance using interfaces to calculate the area of a rectangle and triangle
import java.io.*;
import java.util.*;
interface rectangle
{
public void arearect(double length,double breadth);
}
interface triangle
{
public void areatri(double base,double height);
}
class shape implements rectangle,triangle
{
public void arearect(double length,double breadth)
{
double area=length*breadth;
System.out.println("Area of Rectangle:"+area);
}
public void areatri(double base,double height)
{
double area=(0.5*base*height);
System.out.println("Area of Triangle:"+area);
}
}
class Main
{
public static void main(String a[])
{
 Scanner sc=new Scanner(System.in);
int length,breadth,height,base;
System.out.println("Enter length and breadth of rectangle");
 length=sc.nextInt();
 breadth=sc.nextInt();
shape s=new shape();
s.arearect(length,breadth);
System.out.println("Enter base and height of triangle");
 base=sc.nextInt();
 height=sc.nextInt();
s.areatri(base,height);
}
}

5) bank acc problem

import java.io.*;
import java.util.*;
class LessBalanceException extends Exception
{
 private int wd;
 LessBalanceException(int a)
 {
 wd=a;
 }
 public String toString(){
 return "LessBalanceException"+wd+"rs is not valid";
 }
}
class Account
{
 int bal,acno;
 Account(int acno,int b)
 { acno=acno;
 bal=b;
 }
 void deposit(int d)
 {
 System.out.println("Deposit amount is:"+d);
 bal=bal+d;
 System.out.println("Now the balance of account is:"+bal);
 }
 void withdraw(int w) throws LessBalanceException
 {
 System.out.println("Called withdraw:"+w);
 int temp;
 temp=bal-w;
 if(temp<500)
 throw new LessBalanceException(w);
 else
 {
 bal=bal-w;
 System.out.println("balance is:"+bal);
 }
 }
}
class P4
{
 public static void main(String args[])
 {
 int ch,acno,amt;
 Account a1=new Account(123,500);
 Account a2=new Account(124,1000);
 do{
 System.out.println("1.Deposit\n2.Withdraw\n3.exit\n");
 
 Scanner in=new Scanner(System.in);
 System.out.println("Ur choice\n");
 ch=in.nextInt();
 switch(ch)
 {
 case 1: System.out.println("Enter acno:");
 acno=in.nextInt();
 System.out.println("Enter amount to deposit:");
 amt=in.nextInt();
 if(acno==123)a1.deposit(amt);
 else if(acno==124)a2.deposit(amt);
 else
 System.out.println("Invalid\n");
break;
 case 2: System.out.println("Enter acno:");
 acno=in.nextInt();
 System.out.println("Enter amount to widraw:");
 amt=in.nextInt();
 try{
 if(acno==123)a1.withdraw(amt);
 else if(acno==124)a2.withdraw(amt);
 else
 System.out.println("Invalid\n");
 }
 catch(LessBalanceException e)
 {
 System.out.println("Caught:"+e);
 }
break;
 case 3:System.exit(0) ; break; }
 }while(ch!=3);
 }
}

6)JAVA program using Synchronized Threads, which demonstrates 
Producer Consumer concept.

class Q
{
int n;
boolean valueset=false;
synchronized int get()
{
if(!valueset)
try
{
wait();
}
catch(InterruptedException e)
{
System.out.println("InterruptedException caught");
}
System.out.println("got:"+n);
valueset=false;
notify();
return n;
}
synchronized void put(int n)
{
if(valueset)
{
try
{
wait();
}
catch(InterruptedException e)
{
System.out.println("InterruptedException caught");
}
}
this.n=n;
valueset=true;
System.out.println("put:"+n);
notify();
}
}
class Producer implements Runnable
{
Q q;
Producer(Q q)
{
this.q=q;
new Thread(this,"Producer").start();
}
public void run()
{
int i=0;
while(true)
{
q.put(i++);
}
}
}
class Consumer implements Runnable
{
Q q;
Consumer(Q q)
{
this.q=q;
new Thread(this,"Consumer").start();
}
public void run()
{
while(true)
{
q.get();
}
}
}
class PCFixed
{
public static void main(String args[])
{
Q q=new Q();
new Producer(q);
new Consumer(q);
System.out.println("press control-c to stop.");
}
}

7)a)  queue implementation

import java.util.Scanner;
class QueueOutOfBoundException extends Exception
{
private String msg;
QueueOutOfBoundException(String m)
{
msg=m;
}
public String toString()
{
return msg;
}
}
class Queue
{
int front,rear;
int q[]=new int[3];
Queue()
{
rear=-1;
front=0;
}
void insert(int ele) throws QueueOutOfBoundException
{
if(rear==2)
throw new QueueOutOfBoundException("Queueis Full");
q[++rear]=ele;
System.out.println("the element successfully inserted\n");
}
void delete() throws QueueOutOfBoundException
{
if(rear<front)
throw new QueueOutOfBoundException("queue is empty");
System.out.println("the element deleted is \n"+q[front++]);
}
void display() throws QueueOutOfBoundException
{
int i;
if(rear<front)
throw new QueueOutOfBoundException("Queue is empty");
System.out.println("the queue elements are \n:");
for(i=front;i<=rear;i++)
{
System.out.println(q[i]+"\n");
}
}
}
class useQueue{
public static void main(String args[])
{
Queue a= new Queue();
int ch,ele;
System.out.println("Queue operations \n");
System.out.println("Enter the choice \n");
while(true)
{
System.out.println("1.insertion \n 2.Deletion \n 3.Display \n 4.Exit \n");
Scanner sin=new Scanner(System.in);
ch=sin.nextInt();
switch(ch)
{
case 1: System.out.println("Enter element to be inserted\n");
 ele=sin.nextInt();
 try {
 a.insert(ele);
 }
 catch(QueueOutOfBoundException e)
 {
 System.out.println(e);
 }
 break;
case 2: try {
 a.delete();
 }
 catch(QueueOutOfBoundException e)
 {
 System.out.println(e);
 }
 break;
case 3: try{
a.display(); 
}
catch(QueueOutOfBoundException e)
{
System.out.println(e);
}
 break;
case 4:System.exit(1);
default:System.exit(0);
}
}
}
}

7) b)  package with queue

package shape;
public class Circle
 {
 private double r,PI=3.14;
 public Circle(double radius)
 {
 r=radius;
 }
 public void area()
 {
System.out.println("area of circle"+(PI*r*r));
 }
}
package shape;
public class Square
 {
 private double a;
 public Square(double size)
 {
 a=size;
 }
 
 public void area()
 {
 System.out.println("area of square"+(4*a));
 }
}
package shape;
public class Triangle {
 private double b,h;
 public Triangle(double base,double height)
 {
 b=base;
 h=height;
 }
 
 public void area()
 {
System.out.println("area of triangle"+(b*h/2));
 }
 }
import shape.*;
public class Lab7
{
 public static void main(String args[])
 {
 Circle c=new Circle(20);
 c.area();
 Square s=new Square(15);
 s.area();
 Triangle t=new Triangle(12,6);
 t.area();
 }
} 

8) enumeration







