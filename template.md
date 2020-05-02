# Elixir

## - History of the language:    
  José Valim was created Elixir programming language 9 years ago. Elixir is highly influenced by ERLANG and RUBY. So, he took the best features of Erlang and Ruby for the language that he wants to create. Also, other programming language creators were influenced by the elixir, like Lisp Flavored Erland(LFE). Elixir is a dynamic, concurrent, functional language works on Erlan VM(BEAM). Elixir use of everything the Erlang VM provides and enables higher extensibility with macros and polymorphism.  
## - Why was it invented  
  Before José Valim created elixir, he's job was to improve the RUBY on Rails framework performance.It means jose valim know the week sides of the RUBY. The real problem of RUBY was the RUBY was not designed good enough to solve concurerency Problem. So he developed language with high-concurrency and low-latency language. 
## - When/why shall we use it   
  Banks need reliable, efficient, and fast data operations and data transfer. And also data that store in the bank systems has a large volume. Functional programming is a good tool for complex data operations. Elixir is a functional programming language. So, you can choose ELIXIR for your data operations. Also, elixir is highly reliable. The number of user does not affect the elixir. Because elixir works regardless of user number.  
  
  Elixir has got some features which are flexibility, scalability, and speed, maintaining the web applications. Elixir built on top of Erlang and it has already used by many corporations. Web applications have the benefit of programming with elixir like memory management and the ability to scale linearly. Elixir web applications are efficient by making the best use multicore systems. Phoenix framework is the most popular framework for Elixir. Elixir with Phoenix combinations allows real-time processing on the server-side and javascript on the client-side to helps increase the efficiency and speed of applications for better user experience. Elixir will be a good choice for developing web applications which have many users.  
    
  Netflix, Pinterest, and Whatsapp using Elixir for their applications.
  

## -**How to setup an environment to use it in different platforms**    
#### Windows  
-Download and run [Web installer](https://repo.hex.pm/elixir-websetup.exe)  
-Click next,next...to complete  
#### Linux(Ubuntu or Debian)  
-Add Erlang solution repo: `wget https://packages.erlang-solutions.com/erlang-solutions_2.0_all.deb && sudo dpkg -i erlang-solutions_2.0_all.deb`     
-Run : `sudo apt-get update`     
-Install the Erlang/OTP platform s: `sudo apt-get install esl-erlang`  
-Install Elixir: `sudo apt-get install elixir`   
#### macOS  
Homebrew  
-Update your homebrew to latest: `brew update`  
-Run: `brew install elixir`  
Macports
-Run: `sudo port install elixir`  

## - Example codes    

#### Integer  
5 --> Integer  
0x1F --> Integer  
div(20,10) --> 2  
rem(7,3) --> 1  
  
#### String  
"hello" --> string  
'hello' --> char list  
String.graphemes("hello") --> [ “h”,”e”,”l”,”l”,”o” ]  
String.duplicate("hello ",2) --> hello hello  
String.downcase("Hello") --> hello  
String.upcase("Hello") --> HELLO  
String.reverse("hello") --> olleh  
Atom.to_string(:hello) --> "hello"  
  
#### List  
[1,2,3,4] --> list  
[head | tail] = [1,2,3] --> head = 1, tail= [2,3]  
List.last([1,2,3,4]) --> 4  
lenght.([1,2,3,4]) --> 3  
hd([1,2,3,4]) --> 1  
  
#### Tuple  
{1,2,3,4} --> tuple  
tuple_size({1,2,3,4}) --> 4  
Tuple.to_list({1,2,3,4}) --> [1,2,3,4]  
  
#### IO  
IO.inspect([1,2,3,4]) --> prints a list [1,2,3,4]  
IO.puts("hello") --> print to console hello  
  
#### Conditions  
if false do     
  x=3+5  
  IO.puts(x)  
else  
  y=7+6  
  IO.puts(y)  
End          --> prints console 13  
  
unless false do  
  x=3+5  
  IO.puts(x)  
else  
  y=7+6  
  IO.puts(y)  
End          --> prints console 8  
  
#### Calculator  
```elixir      
defmodule Calculator do  
 def add(x,y) do  
 x+y  
end  
  
def sub(x,y) do  
 x-y  
end  
def sum(x,y) do  
 x*y  
end  
def div(x,y) do  
 x/y  
end  
end  
Calculator.add(3,4) -->7  
  
Calculator.sub(120,35) --> 85  
  
Calculator.sum(3,25) --> 75  
  
Calculator.div(36,9) --> 4   
``` 
#### Fibonacci  
```  
defmodule Fibonacci do 
  def fib(0) do
 0 
end
  def fib(1) do 
1 
end
  def fib(n) do 
fib(n-1) + fib(n-2) 
	end
end

Fibonacci.fib(25)
75025  
``` 
#### Factorial  
``` 
defmodule Factorial do
   def fac(0) do
   1
   end	
   def fac(n) do
   n * fac(n-1)
   end
end

Factorial.fac(5)
120  
```   

## - Things that are specific to this language?
