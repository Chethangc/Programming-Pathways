# Great Learning Java Learning.
## Agenda
1. What is Java?
2. Install Java and Eclipse
3. Variables and Datatype in java.
4. Operator in Java
5. Flow control statements in Java
6. Object Oriented Programming 
7. Inheritance in Java
8. ArrayList in Java.
9. LinkedList in Java.


## 1. What is Java?

Java is a free and opensource software. Its plug and play, Install once use many times. Its cross-platform compatible (can run on any OS like Windows, Linux, Mac). 
Object oriented programming language, its being said it is pure object oriented language to some extent it is yes but it still supports non object oriented concepts like primitive data type ex: int, float, double, etc.
Since we have the IntWrapper, FloatWrapper,etc it can be considered to some extent it is object oriented language.
Objects - Data or field that has a unique attribute or behaviour. (an object is an instance of a class that encapsulates both data (attributes or properties) and behavior (methods or functions) in a single entity.)


## 2. Installing Java and IDE.

### Install JDK
https://www.oracle.com/java/technologies/javase-downloads.html
Java Development Kit (JDK) - For programming all of the java concepts for a particular version.
JDK provides Java Runtime Environment (JRE) -  Executes the written code.
- Download JDK.
- Install JDK

### Install Eclipse and Usage of Eclipse (Highlights)  
https://www.eclipse.org/downloads/  
Provides the development environment for Java.  
32 bit or 64 bit download.  
#### Eclipse Usage  
1. Create a project -  
 File -> New Java Project -> Enter Project Name -> Finish.  
2. src folder consists of the code.  
3. Create a new package.  
  Right click on src folder -> New -> Package -> Enter the name of the package -> Finish.  
4. Create class  
  Right click on src folder -> New -> Class -> Enter the name of the Class (with option public static void main()) -> Finish.  
  main is function.   

#### First Java Program in eclipse.
```
package test;
public class Test { 
public static void main(String[] args){
	System.out.println("This is chethan");
}
}
```
Program execution starts from main().  
Everything in java need to be written in class. Name of the class should start with capital letter in Java.  
Access Modifier - public, private, protected, default.  
In the above function its public everyone can access.  
void - return type does not return anything.  
static function -A static function can be accessed without object.  
Every line should end with semicolon.  
System is class.  
println function - writes the input argument to console.  

## 3. Variables and Datatype in java.

### Variables

Data in programming needs to be stored for processing in temporary storage space called variables.
Variable stored values can be changed later.
<data-type> <variable-name> = <value>; Declaration and assigning
or 
<data-type <variable>; Declaration of variable.

```
package test;
public class Test { 
public static void main(String[] args){
	int a = 10;
	System.out.println(a);
	//Changing the value.
	a=20;
	System.out.println(a);
}
}
```

### Datatypes
Every variable is associated with a data type.
Types of data
- integer - int (Integer -<value> 0 +<value>)
- floating point numbers. (decimal -<value>.<values> 0 +<value>.<values>)
- boolean values. (True and False)
- String data type. ("<Value>", "<String-data>")
- Others. 
```
package test;
public class Test { 
public static void main(String[] args){
	float a = 10.0f;
	System.out.println(a);
	//Changing the value.
	a=20.0f;
	System.out.println(a);
	Boolean data = true;
	System.out.println(data);
	data = false;
	System.out.println(data);
	String b = "Sam";
	System.out.println(b);

}
}
```
## 4. Operators in Java.
Operators are used for perform the operation
- Arithmetic Operators
- Relational Operators
- Logical Operators

Operators:  
&& - AND  
|| - OR  
\>= - Inclusive greater than  
\>  - Greater than  
and others  

```java
//Arithmetic Operators +, -, *, /
int a=10;
int b=20;
int c = a + b ;
System.out.println(c);
c = a-b;
System.out.println(c);
c = a/b; 
// 0 if we want decimal 0.5 then declare float and use it
System.out.println(c);
c = a*b;
System.out.println(c);

//relational operators - relation between two operands
System.out.println(a<b); //Lessthan
System.out.println(a>b); //Greaterthan
System.out.println(a==b); // Equalto
System.out.println(a!=b); // Not Equalto

//Logical operators
// AND
System.out.println(true && true); // prints true
System.out.println(true && false); // prints false
System.out.println(false && true); // prints false
System.out.println(false && false); // prints false
// OR
System.out.println(true || true); // prints true
System.out.println(true || false); // prints true
System.out.println(false || true); // prints true
System.out.println(false || false); // prints false

```

### Comments
Part of the code that is not compiled by the interpreter is called comments.
This for reading purpose and explanation of the code.


## 5. Flowcontrol statements.
### Decision Control Statements
### if else Statement.
In the programming most of the time we need to make a trun based on the decision 
Like below: 
```
if its raining
	play chess
else
	play football/throwball
```

```
if(<condition>){
<Statements>
}
```

```
int a - 20;
int b = 82;
if(a>b){
System.out.println("a is greater than b");
}
else {
System.out.println("b is greater than a");
}
```

### if , else if Statement.
This kind of condition check is used for checking multiple conditions. 
like below:
```
int a - 20;
int b = 82;
if(a == b){
System.out.println("a is equal to b");
}
else if (a>b){
System.out.println("a is greater than b");
}
else {
System.out.println("b is greater than a");
}
```

## Looping Statements.

Reapting a task until a condition is statisfied.
Repeating task multiple times.

Ex: 
Fill up bucket until it full.
Bucket it full is condition.
Adding water is repeatative action.


Looping statements are:
- while
- for
- do while <not in this learning>

### while
To Repeat the statements until the condition is satisfied.
```java
// Syntax
while(<condition>)
{
<Statements to repeat>
}

int a=1;
while(a>=10){
System.out.println(a);
}
//Print 1 - 10 
```

### for loop

To Repeat the statements until the condition is satisfied.
Contains the three values initialize, condition check, increment/decrement usally

initialize - all the statments execute before the loop starts;
condition check - based on which the loop repeats;
increment and decrement - executed after the each loop execution.

```java
for(int i =0; i<10; i++){
System.out.println(i);
}
// prints 0-9
for(int i=0; i<7; i+2){
System.out.println(i);
}
// prints 2,4,6
```
### Pattern Problem
```java
int n=5;
for(int i =0; i < n; i ++){
for (int j=1; j<=i; j ++){
System.out.println("*");
}
System.out.println();
}
``` 
Output:
```java
*
**
***
****
*****

```
Nested for loop is for loop inside the loop, for each time of outer loop inner for loop is executed.
inner for loop execution times is outer for loop execution * inner for loop execution in normal increment.


## Arrays in Java
### Single Dimension 
Helps to store multiple elements of the same data type in java.  
Variable can store only one element.
Multiple elements in same storage space.
100 variable for 100 students
1 array for 100 students is better approach.
It can store same data type only.
['a', 'b', 'c', 'd', 'e', 'f', 'g']


```java
//Array example
char[] a= new char[5];
a[0] = 'a'
a[1] = 'b'
a[2] = 'c'
a[3] = 'd'
a[4] = 'e'

for(int i=0; i<5; i++){
System.out.println(a[i]);
}

//Assigning the value to the Array using forloop
int[] b= new int[10];

for(int i=1; i<=10; i++){
a[i-1] = i;
}
//store 1-10
```
Adding two arrays:
```java
int[] a= new int[5];
int[] b= new int[5];
int[] c= new int[5];
int num=5;

for(int i=0; i<5; i++){
a[i] = i;
b[i] = num;
++num;
c[i] = a[i]+b[i]
System.out.println(c[i]);
}
```

### Multi Dimension Array
Consists rows and coloumns
Array a (2x2) a[0][0], a[1][0], a[0][1] a[1][1]

```java
int[][] a = new int[3][3];
int num = 1
for(int i=0; i<3; i++){
for(int j=0;j<3;j++){
a[i][j] = num;
++num;
}
}

for(int i=0; i<3; i++){
for(int j=0;j<3;j++){
System.out.println(a[i][j]);
}
System.out.println("");
}
```
## Functions in Java

Function in real life is the task that that we do.
Like eating, running, cycling.

Function is block of code that performs a specific action/task.
Ex:
Deposit - Deposit money.
Withdraw - Withdraw money
Balance - Check the balance.

Induvidial Function
```java
public static void main(String[] args){
callchethan(); //Calling
add(10,20);

//Return
Test project = new Test();
int result;
result = project.add(10,20);
System.out.println(result);
}
//non-parameterized function
//Defination
public static void callchethan(){
System.out.println("Call Chethan");
}
//parameterized function
//Defination
public static void add(int num1, int num2){
System.out.println(num1+num2);
}
// non-static Function
public int add(int num1, int num2){
return num1+num2;
}

```
Swapping Function
```java
public static void swapFunction(int a, int b){
System.out.println("Before swapping, a= "+a+"b="+b);
int temp;
temp=a;
a=b;
b=temp;
System.out.println("Before swapping, a= "+a+"b="+b);
}
```
Method Overloading
```java
public static int area(int n1, int n2){
return n1*n2; // Rectangle
}
public static float area(int n){
return 3.14f*n*n; // Circle
}
```
Methods having same but different in parameters or return type.
Main function is starting and ending of the program.
