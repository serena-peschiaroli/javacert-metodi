

- 1. 

What will the following code print when run?

The are 1 correct answers

public class Pass2 {

public static void main(String[] args) {
int x= 6;
doStuff(x);
System.out.print(" main x

= "+ x);

}

void doStuff(int x) {
System.out.print(" do Stuff x

= " + ++x);

}
}

doStuff x = 6 main x = 7
doStuff x = 7 main x = 7
doStuff x = 6 main x = 6
-[x] Compilation fails
doStuff x = 7 main x = 6
An exception is thrown at runtime

_____________________________________________________________________

- 2. 

Which statement is true about a mutator method?

The are 1 correct answers

It replaces the default constructor
It returns mutated instance members
It must be declared private
-[x] It can be used to assign data to instance members

_____________________________________________________________________

- 3. 

Given the following code what is the result?
The are 1 correct answers

public class App {

int num;

public int add(int x) {
num = num + x;
return num;

}

public void add(int x) {
num = num + x;

}

public static void main(String[] args) {
App obj = new App();
obj.add(100);
int ans = obj.add(100);
System.out.println(obj.num);

}

}

300
100
200
-[x] A compilation error occurs



_____________________________________________________________________

- 4. 

Determine the expected output of the following code.
The are 1 correct answers

package com.company;

class Parent{
private int[] array = {1,2};

public int getArray(){
return array;

}

}

public class Main {

public static void main(String[] args) {
Parent main = new Parent();
System.out.print(main.getArray());

}

}

1
runtime error
-[x] Compile time error
12
Zero
1,2


_____________________________________________________________________

- 5. 

Which statement about varargs in Java is true?

There are 2 correct answers

A method can have multiple varargs parameters.
Varargs can be used in combination with other parameters, if the varargs parameter is the first one.
A method with a varargs parameter cannot have other parameters.
-[x] A varargs parameter implicitly creates an array.
-[x] Varargs can be used in combination with other parameters, if the varargs parameter is the last one.
A method with a varargs parameter cannot be overloaded.


_____________________________________________________________________

- 6. 

Given below code in Messenger.java:


class Messenger {

 String msg;

 Messenger(String msg) {this.msg = msg;}

 public void writeMsg() {

  System.out.println(msg);

 }

 public void readMsg() {

  // line n1

 }

}


And the code fragment in Main.java:


public class Main {

 public static void main(String[] args) {

  Messenger m = new Messenger(“All the best“);

  m.readMsg();

 }

}


Which code fragment can be inserted at line n1 to enable the code to print: All the best?

The are 1 correct answers

void writeMsg();
Messenger.writeMsg();
-[x] writeMsg();
m.writeMsg();

_____________________________________________________________________

- 7. 

dentify two class variables:

The are 2 correct answers

-[x] private static int numberOfSquares = 20;
-[x] public static int counter = 0;
private Measure cm;
public int size = 10;
int scale = 35;

_____________________________________________________________________

- 8. 

Which of the following type will not return anything?
The are 1 correct answers

-[x] void
int
none of these
float
null
short


_____________________________________________________________________

- 9. 

Which statement is true about a Java method?

The are 1 correct answers

It must be declared with an access modifier
-[x] It cannot be defined within another method
It must accept a parameter and return a value
It cannot be defined as static final


_____________________________________________________________________

- 10. 

iven:


public class Test {

 static int var2 = 200;

 public static void print() {

  System.out.println(var2);

 }

 public void print (int var1) { //line n1

  System.out.println(var1);

  var2 = var2 + var1; //line n2

  print();

 }

 public static void main(String[] args) {

  Test obj = new Test();

  obj.print(100);

 }

}


What is the result?

The are 1 correct answers

100
-[x] 100 300
A compilation error occurs at line n2
A compilation error occurs at line n1
300
300 100

_____________________________________________________________________

- 11. 

What will the code produce as its output?
The are 1 correct answers

package com.company;

class Number{
int getNumber(){
return 1;

}

public class Main {
private static int a;

public static void main(String[] args) {
System.out.println(getNumber());
}

static int getNumber(){
Number number = new Number();
a = number.getNumber();
return a+1;

}

}

}

-[x] 2
3
zero
runtime error
compile time error
1


_____________________________________________________________________

- 12. 

In method overloading we take an existing method an re-implement it, whereas in method overriding we create methods with same name but different parameters.
The are 1 correct answers

Correct
-[x] Incorrect


_____________________________________________________________________

- 13.   

Given the code:


public class Calc {

 // line n1

  return a + b;

 }

 public static void main(String[] args) {

  Calc obj = new Calc();

  int c = obj.sum(10,20);

  System.out.println(“sum is “ + c);

 }

}


Which code fragment, when inserted at line n1, enables the code to print sum is 30?

The are 1 correct answers

int sum(int a, b) {
-[x] int sum(int a, int b) {
int sum(int, int) {
int sum(int[] a, b) {


_____________________________________________________________________


- 14. 

Which of the following method signatures is an example of a valid method overload for public void sendMessage(String msg)?

There are 2 correct answers

public void sendMessage(String msg, int count)
private void sendMessage(String msg)
private void sendMessage(String author)
public int sendMessage(String msg)
-[x] public void sendMessage(int msg)
-[x] private void sendMessage(String msg, String author)






_____________________________________________________________________

- 15. 

Given the code fragment:


class Course {

 String name;

 static int count = 0;

 public Course(String name) {

  this.name = name;

  count++;

 }

}

public class App {

 public static void main(String[] args) {

  Course c = new Course(“Java Programming“);

  // line n1

 }

}


Which code fragment, when inserted at line n1, enables the code to print Java Programming:1?

The are 1 correct answers

System.out.println(name + ":" + count);
System.out.println(c.name + ":" + count);
-[x] System.out.println(c.name + ":" + Course.count);
System.out.println(Course.name + ":" + c.count);



_____________________________________________________________________


- 16. 

Which of the following return type does not return anything?
The are 1 correct answers

double
-[x] void
long
char
boolean
short


_____________________________________________________________________

- 17.  

Will the below code produce number zero as the output?


package com.company;

class Number{

 int getNumber(int a){ return a; }

 int getNumber(int a, int b){ return a+b; }
}

public class Main {

 private static int a;

 public static void main(String[] args) {

  Number number = new Number();

  a = number.getNumber(a);

  a = number.getNumber(a,a);

  System.out.println(a);

 }
}

The are 1 correct answers

-[x] TRUE
FALSE


_____________________________________________________________________

- 18.   

Assuming the following overloaded methods exist, which method is called when process(5) is executed?

The is 1 correct answer



void process(int num) {
System.out.println("Processing int");

}

void process(long num) {
System.out.println("Processing long");

}

void process(double num) {
System.out.println("Processing double");

}

-[x] process(int num)
process(long num)
process(double num)
Compilation fails
None of the above
A Runtime Exception occurs


_____________________________________________________________________


- 19. 

Which if the following statement is correct?
The are 1 correct answers

None of the option is correct
-[x] Methods are overloaded
classes are overloaded
Variables are overloaded
All options are correct
Variables and Methods both are overloaded



_____________________________________________________________________

- 20. 

Given the following contents of two java source files:

What changes, when made independently, will enable the code to compile and run?

package commons.text;
public class StringUtils {
static String capitalize(String msg) {
//return code here

}

}

And:

//line 1
public class TestClass {
public static void main(String[] args) {
String output = StringUtils.capitalize("jason donovan");
System.out.println(output);

}

}

Add the following import on line 1: import commons.text.*;
Add the following import on line 1: import StringUtils;
-[x] Add the following import on line 1: import commons.text.StringUtils;
Add the following import on line 1: import common.text;
The code compiles without any change: Replace StringUtils.capitalize(“jason donovan”) to commons.text.StringUtils.capitalize(“Jason donovan“)
None of the above



_____________________________________________________________________