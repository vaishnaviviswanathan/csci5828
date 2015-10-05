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


<p style="text-align:center;font-weight:bold">FUNCTIONAL PROGRAMMING PARADIGM</p>

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


<p>Programming Languages that use Procedural Paradigm are:
</p>
> Go

> Pascal

> Bliss 

> Blue

<b>Example in Pascal - calculating Fibonacci series;</b>

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


