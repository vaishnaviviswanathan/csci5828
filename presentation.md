####**PROGRAMMING PARADIGMS**
				
<b>What is a Programming Paradigm?</b>

<p>
Programming paradigm is a style of programming a language.
The word paradigm is from the Greek word “paradeigma” which means a group sharing a characteristic.
Paradigm depicts a thought pattern followed to achieve a specification given.
Programming Paradigm indicates the style or the way a programmer thinks to solve a programming problem. 
This style is a notational form that can be read by both the machine and the human. 
Hence, it is nothing but a standard programming procedure followed to achieve a task.
</p>

Some of the programming paradigms which were developed over time are,

* Imperative
* Declarative
* Functional
* Object-Oriented
* Procedural
*  Logic
 
<p>
There are many programming languages which supports either a single paradigm 
or multiple paradigms.In this presentation we discuss about the most used paradigms;
Logical,Imperative,Functional,Procedural,Object-Oriented. 
</p>

<p style="text-align:center"><b>HISTORY</b></p>

<p>
The Machine code was the first programming paradigm which was introduced in
the earlier days. Assembly language (mnemonics and symbolic labels were used
to represent machine instruction and memory addresses)
was used for coding. These languages are also called the first and 
second generation languages.
</p>

<p>
Then came the Procedural languages. They had routines, subroutines, methods
and functions. One of the commonly known programming language,C, is a procedural 
language. These are also called the second generation programming language.
The procedural programming uses procedures to operate on data structures.
</p>

<p>
Object Oriented language was the next paradigm which was introduced. It involved 
creating objects which interacted in defined ways. Programming language C++, Java ,
C# are examples of an Object Oriented language.
</p>

<p>
Then came the declarative programming paradigms. Ex:SQL. They are also called the 
fourth generation languages. They tell the computer WHAT the program 
should do instead of specifying HOW the program should do it i.e they describe
their desired results without listing the commands required to achieve it.
</p>

<p>
Imperative works in contrast to the declarative programming language. Procedural
Programming is an imperative programming paradigm.  
</p>

<p>
FUNCTIONAL and LOGICAL PROGRAMMING PARADIGMS fall under DECLARATIVE 
PROGRAMMING paradigm.
<p>

<p style="text-align:center;font-weight:bold"><b>LOGICAL PROGRAMMING PARADIGM</b></p>
			
<p>								
Logic programming is a programming paradigm based on formal logic. 
A logic program is a set of instructions that model facts and rules about the problem. 
It is analogous to translation of problems in terms of digital logic. 
Logic programming works well in exhaustive searches since it involves automatic backtracking for problems
</p>


Some languages which can be programmed in Logical Paradigm:

> Prolog

> ASP

>Datalog

>ROOP
 
<p>
Algorithms in logic programming are a combination of logic(determines solutions) and control
(determines alternate ways of execution)
</p>
 
<b>Example in Prolog to calculate fibonacci series:</b>

<pre><code>
fib(1, 1).
fib(2, 1).
fib(X, Y):-
       X > 1,
       X1 is X - 1,
       X2 is X - 2,
       fib(X1, Z),
       fib(X2, W),
       Y is W + Z.
main :-
  fib(6,X), write(X), nl.

</pre></code>
						

<p style="text-align:center;font-weight:bold"><b>IMPERATIVE PROGRAMMING PARADIGM</b></p>
			
<p>
In Imperative Programming, the programmer knows the formula or the steps to be followed to
solve a problem. He instructs the program to follow those steps to get what he wants in return. 
</p>

Languages :
Machine level languages

>Fortran

>ALGOL

>COBOL

>BASIC

>Pascal

<p>
<b>Example in Javascript to multiply elements of an array by 2</b>
</p>

<pre><code>
var numbers = [1,2,3,4,5]
var doubled = []

for(var i = 0; i < numbers.length; i++) 
{
  var newNumber = numbers[i] * 2
  doubled.push(newNumber)
}
console.log(doubled) //=> [2,4,6,8,10]
</code></pre>


<p style="text-align:center;font-weight:bold"><b>FUNCTIONAL PROGRAMMING PARADIGM</b></p>

<p>
In this paradigm, a problem is divided into functions. 
Functions are nothing but blocks of code with a name. 
They are capable of performing a particular task when invoked. 
They just compute what they are told to and are not bothered with the steps around them.
</p>

<p>
Functional programming languages can be either pure or impure. 
Pure functional languages are the ones which do not have any other way to program paradigm
mixed with functional style.Impure functional programming languages can have some influences
from other programming paradigms.
</p>

<p>
Some pure functional programming languages are :
</p>

>Haskell

>Hope

>Mercury

>Miranda

Some impure functional programming languages are :

>C#

>Curve

>Groovy

>Erlang
 
<b>Example - python</b>

<pre>
<code>

def fizbuz(n):
'''
Print FizzBuzz when n is a multiple of 3 and 5
Print Fizz when n is a multiple of only 3 and not 5
Print Buzz when n is a multiple of 5 and not 3
'''
    i = 0
    while(i < n+1) :
        if i%3==0 or i%5==0:
            if i%3 ==0 and i%5!=0:
                print "Fizz"
            elif i%3 !=0 and i%5==0:
                print "Buzz"

            elif i%3==0 and i%5==0:
                print "FizzBuzz"
        i+=1

def main():
    n = 100
    fizbuz(n)

main()

</pre></code>



<p style="text-align:center;font-weight:bold"><b>PROCEDUARAL PROGRAMMING PARADIGM</b></p>

<p>
In Procedure Oriented Programming paradigm, the problems are solved by concentrating on how to do things.
They are based on procedures, which are also known as routines. We instruct the program how to operate 
on the data, but the data is given lesser importance. Hence, the data is said to be decoupled from the 
functions which operate on it. In Procedural Programming, data moves freely throughout the program. 
Hence, every modification reflects throughout the program. The problem here is not modelled in terms of 
a real world problem.
</p>


Programming Languages that use Procedural Paradigm are:

<p>Go</p>

<p>Pascal</p>

<p>Bliss </p>

<p>Blue</p>

<b>Example in Pascal - Calculating Fibonacci series:</b>

<pre><code>
function fib(n: Integer): Integer;
var a: Integer = 1;
    b: Integer = 1;
    f: Integer;
    i: Integer;
begin
  if (n = 1) or (n = 2) then
     fib := 1
  else
    begin
      for i := 3 to n do
      begin
         f := a + b;
         b := a;
         a := f;
      end;
      fib := f;
    end;
end;

begin
  WriteLn(fib(6));
end.

</code></pre>

<b>Object Oriented Programming Paradigm</b>
<p>
In Object Oriented Programming, all the behavior that we want a program to display is present in under a Class.</p> 

<p>Some languages which can be programmed in Object Oriented Paradigm :</p>
<p>
<p>1.Java</p>

<p>2.Python</p>

<p>3.C++</p>

<p>4.Ruby</p>
</p>
<p><b>Example program - python to print time</p>
<pre><code>
def print_time(time) :
    print '(%.2d:%.2d:%.2d)' %(time.hour, time.minute, time.second)


class Time(object) :
    '''
    Time of the day
    The attributes are hour, minute and seconds
    '''

time = Time()
time.hour = raw_input("Enter the hour:")
time.hour = int(time.hour)
time.minute = raw_input("Enter minutes:")
time.minute = int(time.minute)
time.second = raw_input("Enter seconds:")
time.second = int(time.second)
print_time(time)

</pre></code>


<b>Object - oriented sample program in JAVA </b>

                   EXAMPLE PROGRAM 
<pre><code>
REDUCING THE RATIONAL NUMBERS AND TO PERFORMS ARITHMETIC OPERATIONS WITH TWO RATIONAL NUMBERS

import java.util.*;

class operation
{
int a,b;

/** CONSTRUCTOR TO INITIALISE THE VALUES PASSED TO THE CLASS VARIABLES
@param x -numerator
@param y -denominator
*/

public operation(int x,int y)
{
a=x;
b=y;
}

/** DISPLAY METHOD IS TO DISPLAY THE ENTERED RATIONAL NUMBERS */
public void display()
{
System.out.println("the rational number is "+a+"/"+b);
}

/** GCD METHOD IS TO FIND THE GCD OF THE TWO NUMBERS ENTERED 
@param number1 -numerator
@param number2 -denominator
@return -returns the gcd of the two numbers

*/

public int gcd(int number1,int number2)
{
if(number2==0)
{
return number1;
}
return gcd(number2,number1%number2);
}


/** REDUCE METHOD IS TO REDUCE THE RATIONAL NUMBER TO ITS LEAST FORM
@param number1 -numerator
@param number2 -denominator
@param c -it is the gcd of the two numbers(numerator and denominator)
*/

public void reduce(int number1,int number2,int c)
{
if(number2==0)
System.out.println("\n invalid rational number");
else
{
number1=number1/c;
number2=number2/c;
System.out.println("the reduced rational number is..."+number1+"/"+number2);
}//else close
}

/** PERFORMS ADDITION OF TWO RATIONAL NUMBERS
@param a numerator of the first rational number
@param b denominator of the first rational number
@param c numerator of the second rational number
@param d denominator of the second rational number
*/

public void add(int a,int b,int c,int d)
{
int deno=b*d;
int num=a*d+b*c;
System.out.println("the rational number is "+num+"/"+deno);
int cd1=gcd(num,deno);
System.out.println("the gcd of the two numbers is"+cd1);
reduce(num,deno,cd1);
}

/** PERFORMS SUBTRACTION OF TWO RATIONAL NUMBERS
@param a numerator of the first rational number
@param b denominator of the first rational number
@param c numerator of the second rational number
@param d denominator of the second rational number
*/

public void sub(int a,int b,int c,int d)
{
int deno=b*d;
int num=(a*d)-(b*c);
System.out.println("the rational number is "+num+"/"+deno);
int cd1=gcd(num,deno);
System.out.println("the gcd of the two numbers is"+cd1);
reduce(num,deno,cd1);
}

/** PERFORMS MULTIPLICATION OF TWO RATIONAL NUMBERS
@param a numerator of the first rational number
@param b denominator of the first rational number
@param c numerator of the second rational number
@param d denominator of the second rational number
*/

public void mul(int a,int b,int c,int d)
{
int deno=(b*d);
int num=(a*c);
System.out.println("the rational number is "+num+"/"+deno);
int cd1=gcd(num,deno);
System.out.println("the gcd of the two numbers is"+cd1);
reduce(num,deno,cd1);
}

/** PERFORMS DIVISION OF TWO RATIONAL NUMBERS
@param a numerator of the first rational number
@param b denominator of the first rational number
@param c numerator of the second rational number
@param d denominator of the second rational number
*/

public void div(int a,int b,int c,int d)
{
int deno=(b*c);
int num=(a*d);
System.out.println("the rational number is "+num+"/"+deno);
int cd1=gcd(num,deno);
System.out.println("the gcd of the two numbers is"+cd1);
reduce(num,deno,cd1);
}
}

public class Rationalnum1
{
public static void main(String l[])
{
Scanner s1=new Scanner(System.in);
System.out.println("Enter the first number to find GCD");
int number1=s1.nextInt();
System.out.println("Enter the second number to find GCD");
int number2=s1.nextInt();
operation op=new operation(number1,number2);
op.display();
int cd=op.gcd(number1,number2);
System.out.println("the gcd of the two numbers is"+cd);
op.reduce(number1,number2,cd);
do{
System.out.println("\n\n1.ARITHMETIC OPERATIONS 2.EXIT\n\n");
System.out.println("enter the choice");
int choice=s1.nextInt();
switch(choice)
{
case 1:
{
//first fraction
System.out.println("Enter the first number");
int a=s1.nextInt();
System.out.println("Enter the second number");
int b=s1.nextInt();
System.out.println("the first rational number is "+a+"/"+b);
//second fraction
System.out.println("Enter the third number");
int c=s1.nextInt();
System.out.println("Enter the fourth number");
int d=s1.nextInt();
System.out.println("the second rational number is "+c+"/"+d);
System.out.println("Enter the option\n1.add\n2.sub\n3.mul\n4.div\n");
int e=s1.nextInt();
//perform addition
if(e==1)
{
op.add(a,b,c,d);
}
//perform subtraction
if(e==2)
{
op.sub(a,b,c,d);
}
//perform multiplication
if(e==3)
{
op.mul(a,b,c,d);
}
//perform division
if(e==4)
{
op.div(a,b,c,d);
}
break;
}
default:
{
System.out.println("\nerror!");
System.exit(1);
break;
}
}//switch close
}while(true);
}//method close
}//class close
</pre></code>


<p><b> Some of the most important concepts in OOP are : </b></p>
<b>(I) Classes: </b>
<p>
Classes are the key component in OOP. It is a blueprint for the object. Classes describe what an object should be like. They have three fundamental aspects : 
</p>

>1.Type(what the class is)

>2.Attributes (describes the data fields used in the class)

>3.Methods (describes the functions and subroutines that constitute the class behavior)

<p>Several languages include predefined classes for convenience.</p>

<b>Example in  Java:</b>
<pre><code>
public class Rectangle -------> CLASS TYPE/NAME                                         
{
public static void main(String args[])
{
      		int length, breadth,b; -------> CLASS ATTRIBUTES
Scanner s1 = new Scanner(System.in);
System.out.println(“Enter length”);
Length=s1.nextInt();
System.out.println(“Enter breadth”);
Breadth=s1.nextInt();
b=Area();
System.out.println(b);
}
Area() -------> CLASS BEHAVIOR/METHOD
{
return (length*breadth);
}}}

</pre></code>

 
<p>(II) Abstraction:</p>

<p>Abstraction involves managing complexity in computer systems. It enables the user to interact with a class or a function at a higher level and suppresses unnecessary details. Essentially, the user has an interface with which he interacts with the elements and is not concerned with representation and implementation details below that interface.</p>

<b>Example:</b>

<p>Consider the Area method in the previous example. We can just call Rectangle.area and do not need to know the exact formula for the area. Area acts as a black box that takes in the length and the breadth and outputs the rectangle area.</p>

<p><b> (III) Encapsulation:</b></p>
<p>Encapsulation enables combining data and functions into a single entity. Additionally, it involves access restriction to the inner working of the class. It is roughly similar to abstraction in information hiding. It reduces dependencies and collisions between pieces of code.</p>

<b>Example:</b>
<pre><code>
int x,y
d = distance(x,y)
</pre></code>

<p><b> (IV) Inheritance:</b></p>
<p>Inheritance is a means of avoiding repetition when we have several classes sharing similar behaviors. Suppose we have class p. We want to create a class c which has all the behaviors of class p and some additional ones. Then, p is called the parent class and c is called the child class. Inheritance is generally defined by “is a” relationship. A Mercedes Class inherits from a Car Class because a Mercedes is a Car. </p>

<p><b> (V) Polymorphism:</b></p>
<p>Polymorphism implies “many forms”. It is a feature by which a single interface can be used for different purposes. Essentially, it lets us do the right thing at the right time. It is of two types: </p> 

>1.Compile time polymorphism

>2.Run time polymorphism
 
<p><b>Compile time polymorphism:</b></p>
<p>It involves early binding, static binding or static linking. The object is bound to the function call at compile time. It is implemented through function and operator overloading.</p>
 
<p><b>Run time polymorphism:</b></p>
<p>It involves dynamic binding or late binding. Objects of the derived class are treated as if they are the objects of base class. The function and the object are not linked till run time. It is achieved through virtual functions.</p>

