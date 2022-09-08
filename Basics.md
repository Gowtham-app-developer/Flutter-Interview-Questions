# Flutter-Basics

## Table of Contents

| S.No | Content |
| --------	 | ------------ |
| 1 | [Hello World](Basics.md#hello-world) |
| 2 | [ Adding Comment Line](Basics.md#adding-comment-line) |
| 3 | [Variable Declration](Basics.md#variable-declration) |
| 4 | [Literals and String Interpolation](Basics.md#literals-and-string-interpolation) |
| 5 | [If and Else](Basics.md#if-and-else) |
| 6 | [Ternary Operator](Basics.md#ternary-operator) |
| 7 | [Switch Case Statement](Basics.md#switch-case-statement) |
| 8 | [For Loop](Basics.md#for-loop) |
| 9 | [While Loop](Basics.md#while-loop) |
| 10 | [Do While Loop](Basics.md#do-while-loop) |
| 11 | [Break Keyword](Basics.md#break-keyword) |
| 12 | [Continue Keyword](Basics.md#continue-keyword) |
| 13 | [Function](Basics.md#function) |
| 14 | [Function as Expression](Basics.md#function-as-expression) |
| 15 | [Function [Optional Positional Parameters]](Basics.md#function-optional-positional-parameters) |
| 16 | [Function [Optional Named Parameters]](Basics.md#function-optional-named-parameters) |
| 17 | [Function [Optional Default Parameters]](Basics.md#function-optional-default-parameters) |


## Hello World

- The main function is the entry point of all our Flutter Applications (i.e.) whatever the code we written in the main function will get executed first.

__Example__

```ruby
void main() { // TODO void main() - Entry Point
  
  print("Hello World");
 
  print(4-3);  // TODO Performing some Arithematic Operations
  
  print(false);
  
}
```  
:arrow_up: [__Back to Top__](Basics.md#table-of-contents)

## Adding Comment Line

```ruby
/**
 * This is one type of comment Line
 */

// This is the another type of comment line
```
:arrow_up: [__Back to Top__](Basics.md#table-of-contents)

## Variable Declration

- Dart supports the Following Data Types (i.e.) Numbers (int, double), Strings, Booleans, Lists (also known as Arrays), Maps, Runes (for expressing Unicode character in a String) and Symbols 
- In Dart, We can declare the Value using Data Type (i.e.) String, int, etc (or) using var.
- By using 'var' it will be inferred as data type automatically by compiler.
- __Note:__ All data types in Dart are Objects. Therefore, their initial value is default by 'null' unless we initialize the Values.

__Example__

```ruby
void main() {
  
   // TODO Strings
    String mValue = "Hello World"; // TODO Where String - Data Type, mValue - Variable Name and "Hello World" - Value
    var company = "Amazon";
    print(mValue);
  
    // TODO Numbers: int
    int score = 25;
    var count = 50; // TODO It is inferred as integer automatically by compiler
    int hexValue = 0xEADEBAEE;
    print(score);
  
    // TODO Numbers: double
    double percentage = 95.0;
    var percent = 70.0;
    double exponents = 1.42e5;
    print(exponents);
  
    // TODO Boolean
    bool isValid = true;
    var isAlive = false;
    print(isAlive);
  
}
```  
:arrow_up: [__Back to Top__](Basics.md#table-of-contents)

## Literals and String Interpolation

- __Literals__ - It is the Values where you can assign them to a Variables.
- __String Interpolation__ - It is the process of replacing placeholders with values in a string literal.

```ruby
void main() {

    // TODO Literals
    String s1 = 'Hello World'; // TODO Where 'Hello World' is the String Literals 
    
    // TODO Various ways to define String Literals in Dart
    String s2 = 'Hello World';
    String s3 = "Hello World";
    String s4 = 'It\'s easy';
    String s5 = "It's easy";
    String s6 = 'Hello my Self Gauthy completed B.E in Electronics and Communication'
    'Engineering';
   
    print(s6);
   
   // TODO String Interpolation
    String name = "Hello World";
   
    print("My name is " + name); // TODO Appending the name is just a bad pratice 
    print("My name is $name"); // TODO String Interpolation
    print("The number of characters in String Kevin is ${name.length}");
    
    int l = 20;
    int b = 10;
    
    print("The sum of $l and $b is ${l + b}");
    print("The area of rectangle with length $l and breadth $b is ${l * b}");
}
```  
:arrow_up: [__Back to Top__](Basics.md#table-of-contents)  

## If and Else

```ruby
void main() {

    // TODO IF and ELSE Statements
    var salary = 50000;
    if (salary > 50000) {
        print("You got promotion. Congratulations !");
    } else {
        print("You need to work hard !");
    }
  
    // TODO IF ELSE IF Ladder statements
    var marks = 70;
    if (marks >= 90 && marks < 100) {
        print("A+ grade");
    } else if (marks >= 80 && marks < 90) {
        print("A grade");
    } else if (marks >= 70 && marks < 80) {
        print("B grade");
    } else if (marks >= 60 && marks < 70) {
        print("C grade");
    } else if (marks > 30 && marks < 60) {
        print("D grade");
    } else if (marks >= 0 && marks < 30) {
        print("You have failed");
    } else {
        print("Invalid Marks. Please try again !");
    }
}
```
:arrow_up: [__Back to Top__](Basics.md#table-of-contents)  

## Ternary Operator

```ruby
void main() {

    // TODO Ternary Operator
  
    // TODO condition ? exp1 : exp2
    // TODO If condition is true, evaluates expr1 (and returns its value);
    // otherwise, evaluates and returns the value of expr2.
    int a = 5;
    int b = 10;
    int smallNumber = a < b ? a : b;
  
    print("$smallNumber is smaller");
  
    // TODO exp1 ?? exp2
    // TODO If expr1 is non-null, returns its value; otherwise, evaluates and
    // returns the value of expr2.
    String name = null;
    String nameToPrint = name ?? "Guest";
  
    print(nameToPrint);
}
```
:arrow_up: [__Back to Top__](Basics.md#table-of-contents)  

## Switch Case Statement

```ruby
void main() {
  
    // TODO Switch Case Statements: It is Applicable only for 'int' and 'String'
    
  	String grade = 'A';
    switch (grade) {
        case 'A':
            print("Excellent grade of A");
            break;
        case 'B':
            print("Very Good !");
            break;
        case 'C':
            print("Good enough... But work hard");
            break;
        case 'F':
            print("You have failed..");
            break;
        default:
            print("Invalid Grade..");
    }
}
```
:arrow_up: [__Back to Top__](Basics.md#table-of-contents)  

## For Loop

- Initialize -> Condition Check -> Code Execute -> Increment 

```ruby
void main() {

    // TODO FOR Loop
    // Finding the even numbers between 1 to 10
    for (int i = 1; i <= 10; i++) {
        if (i % 2 == 0) {
            print(i);
        }
    }
  
    // TODO for ..in loop  
    // TODO List is just a collection of data type  
    List planetList = ["Mercury", "Venus", "Earth", "Mars"];
    for (String planet in planetList) {
        print(planet);
    }
}
```
:arrow_up: [__Back to Top__](Basics.md#table-of-contents)  

## While Loop

- Initialize -> Condition Check -> Code Execute -> Increment 

```ruby
void main() {

    // TODO Finding the even numbers between 1 to 10
    
    var i = 1;
    while (i <= 10) {
        if (i % 2 == 0) {
            print(i);
        }
        i++;
    }
}
```
:arrow_up: [__Back to Top__](Basics.md#table-of-contents)  

## Do While Loop

- Initialize ->  Code Execute -> Increment -> Condition Check

```ruby
void main() {

    // TODO Finding the even numbers between 1 to 10
    
    int i = 1;
    do {
        if (i % 2 == 0) {
            print(i);
        }
        i++;
    } while (i <= 10);
}
```
:arrow_up: [__Back to Top__](Basics.md#table-of-contents)  

## Break Keyword

```ruby
void main() {
  
    outerLoop: for (int i = 1; i <= 4; i++) {
        for (int j = 1; j <= 4; j++) {
            print("$i $j");
            if (i == 2 && j == 2) {
                break outerLoop; // TODO outerLoop - We can give it as any name
            }
        }
    }
}
```
:arrow_up: [__Back to Top__](Basics.md#table-of-contents)  

## Continue Keyword

```ruby
void main() {
  
    myLoop: for (int i = 1; i <= 4; i++) { 
        for (int j = 1; j <= 4; j++) { // TODO You can give the name for the inner for Loop too
            if (i == 2 && j == 2) {
                continue myLoop; // TODO continue will skip the code of the nearest for Loop
            }
            print("$i  $j");
        }
    }
}
```
:arrow_up: [__Back to Top__](Basics.md#table-of-contents)  

## Function

- Collection of Statements grouped together to perform an Operation.
- Functions in Dart are Objects (i.e.) Functions can be assigned to a variable or we can passed as a parameter to other functions.
- All Functions in Dart returns a Value and if no return value is specified then it returns null.
- Defining return type is optional but is recommended as per code convention

__Example__

```ruby
void main() {

// TODO Define a Function
// TODO Pass parameters to a Function
// TODO Return value from a Function
// TODO Test that by default a Function returns null
  
	findPerimeter(4, 2);

	int rectArea = getArea(10, 5); 
	print("The area is $rectArea");
  
}

void findPerimeter(int length, int breadth) {

	int perimeter = 2 * (length + breadth);
	print("The perimeter is $perimeter");
}

// TODO int - Return Type, getArea - Function Name, (int length, int breadth) - Parameter
int getArea(int length, int breadth) {

	int area = length * breadth;
	return area;
}
``` 
:arrow_up: [__Back to Top__](Basics.md#table-of-contents)  

## Function as Expression

```ruby
void main() {

// TODO "=>" is known as FAT ARROW
// TODO "=> expression" is a SHORT HAND SYNTAX for { return expression; }
// TODO Example "=> length * breadth" is SHORT HAND SYNTAX for { return length * breadth; }
  
	findPerimeter(6, 2);

	int rectArea = getArea(15, 5); 
	print("The area is $rectArea");
  
}

void findPerimeter(int length, int breadth) => print("The perimeter is ${2 * (length + breadth)}");

int getArea(int length, int breadth) => length * breadth;
```  
:arrow_up: [__Back to Top__](Basics.md#table-of-contents)  

## Function [Optional Positional Parameters]

- A parameter wrapped by [ ] is a positional optional parameter (i.e.) Basically We can skip the parameters of the Right Hand Side.

__Example__

```ruby
void main() {

  // TODO Passing Required Parameters
  printCities("New York", "New Delhi", "Sydney");
	print("");

  // TODO Passing Optional Positional Parameters
	printCountries("USA"); // TODO We can skip the Optional Positional Parameters
  
}

// TODO Required Parameters
void printCities(String name1, String name2, String name3) {

	print("Name 1 is $name1");
	print("Name 2 is $name2");
	print("Name 3 is $name3");
}

// TODO Optional Positional Parameters
void printCountries(String name1, [name2, name3]) {

	print("Name 1 is $name1");
	print("Name 2 is $name2");
	print("Name 3 is $name3");
}
```  
:arrow_up: [__Back to Top__](Basics.md#table-of-contents)  

## Function [Optional Named Parameters]

- A parameter will be disclosed with curly bracket { } and the Sequence of Named Parameter doesn't matter.

__Example__

```ruby
void main() {
  
	findVolume(10, breadth: 5, height: 20);
	print("");

  // TODO Sequence doesn't matter in Named Parameter
	findVolume(10, height: 20, breadth: 5); 
}

void findVolume(int length, {breadth, height}) {

	print("Length is $length");
	print("Breadth is $breadth");
	print("Height is $height");

	print("Volume is ${length * breadth * height}");
}
```
:arrow_up: [__Back to Top__](Basics.md#table-of-contents)  

## Function [Optional Default Parameters]

```ruby
// TODO Optional Default Parameters

void main() {

	findVolume(10); // TODO Default value comes into action
	print("");

	findVolume(10, breadth: 5, height: 30); // TODO Overrides the old value with new one
	print("");

	findVolume(10, height: 30, breadth: 5); // TODO Making use of Named Parameters with Default values
}


findVolume(int length, {int breadth = 2, int height = 20}) {

	print("Lenght is $length");
	print("Breadth is $breadth");
	print("Height is $height");

	print("Volume is ${length * breadth * height}");
}
```
:arrow_up: [__Back to Top__](Basics.md#table-of-contents)  

## Exception Handling 

- The Exception Handling is a mechanism used to handle the runtime errors so that normal flow of the application can be maintained.
- It can be handled using four keyword Types -> try, catch, finally and on.
- Some Common Exception Types -> Format Exception (Datatype doesn't have an expected expected format), IO Exception, Timeout Exception (Schedule timeout happens while waiting for an async result) and Integer Division By ZeroException (Thrown when a number is divided by zero)

```ruby
// TODO ON Clause
// TODO Catch Clause with Exception Object
// TODO Catch Clause with Exception Object and StackTrace Object
// TODO Finally Clause
// TODO Create our own Custom Exception

void main() {

	print("CASE 1");
	// TODO CASE 1: When you know the exception to be thrown, use ON Clause
	try {
		int result = 12 ~/ 4; // where ~/ means divide to integer & return results in the form of Integer
		print("The result is $result");
	} on IntegerDivisionByZeroException {
		print("It Cannot divide by Zero");
	}

	print(""); print("CASE 2");
	// TODO CASE 2: When you do not know the exception use CATCH Clause
	try {
		int result = 12 ~/ 0;
		print("The result is $result");
	} catch (e) {
		print("The exception thrown is $e");
	}

	print(""); print("CASE 3");
	// TODO CASE 3: Using STACK TRACE to know the events occurred before Exception was thrown
	try {
		int result = 12 ~/ 0;
		print("The result is $result");
	} catch (e, s) {
		print("The exception thrown is $e");
		print("STACK TRACE \n $s");
	}

	print(""); print("CASE 4");
	// TODO CASE 4: Whether there is an Exception or not, FINALLY Clause is always Executed
	try {
		int result = 12 ~/ 3;
		print("The result is $result");
	} catch (e) {
		print("The exception thrown is $e");
	} finally {
		print("This is FINALLY Clause and is always executed.");
	}

	print(""); print("CASE 5");
	// TODO CASE 5: Custom Exception (i.e.) Creating an Exception manually
	try {
    throwException();
  } on CustomException {
    print("custom exception has been obtained");
  }
}

class CustomException implements Exception {
  String cause;
  CustomException(this.cause);
}

throwException() {
  throw new CustomException('This is my custom exception');
}
```
## Getter and Setter

```ruby
void main() {

  var student = Student();
  
  // TODO Default Getter and Setter
  student.name = "Gauthy"; // TODO Calling default Setter to set value
  print(student.name); // TODO Calling default Getter to get value

  student.percentage = 438.0;   // Calling Custom Setter to set value
  print(student.percentage);    // Calling Custom Getter to get value
}

class Student {

  // TODO Instance Variable with default Getter and Setter
  String name = "Test"; 

  // TODO Private Instance Variable
  double _percent = 0.00; // TODO _ indicates the Private Instance Variable for its own library

  // TODO Instance variable with Custom Setter
  void set percentage(double marksSecured) => _percent = (marksSecured / 500) * 100;
  
  // TODO Instance variable with Custom Getter
  double get percentage => _percent;
}
```  

## Constructor [Inheritance using Default and Named Constructor]

- By Default, a constructor in a subclass calls the superclass's no arguement Constructor.
- The parent class constructor is always called before child class constructor.
- If default constructor is missing in Parent class, then you must manually call one of the constructor in Super class.

```ruby
void main() {

	var dog1 = Dog("Labrador", "Black");

	print("");

	var dog2 = Dog("Pug", "Brown");

	print("");

	var dog3 = Dog.myNamedConstructor("German Shepherd", "Black-Brown");
}

class Animal {

	String? color;

  // TODO Inheritance with Default Constructor and Parameterised Constructor
	Animal(String color) {
		this.color = color;
		print("Animal class constructor");
	}
  
  // TODO Inheritance with Named Constructor
	Animal.myAnimalNamedConstrctor(String color) {
		print("Animal class named constructor");
	}
}

class Dog extends Animal {

	String? breed;

	Dog(String breed, String color) : super(color) {
		this.breed = breed;
		print("Dog class constructor");
	}

	Dog.myNamedConstructor(String breed, String color) : super.myAnimalNamedConstrctor(color) {
		this.breed = breed;
		print("Dog class Named Constructor");
	}
}
```

## Lists

- Types -> Fixed-Length List, Growable List
- Fixed-Length List -> Length once defined cannot be changed.
- Growable List -> Length is Dynamic.

__Example using Fixed-Length List__

```ruby
void main() {

  // TODO Index:       0   1   2   3   4
  // TODO Elements:    73  64  N   21  12

	List<int> numbersList  = List<int>.filled(5, 0, growable: false); // TODO Declaring Fixed-length list
	numbersList[0] = 73;  // TODO Insert operation
	numbersList[1] = 64;
  	numbersList[2] = 64;
	numbersList[3] = 21;
	numbersList[4] = 12;

	numbersList[0] = 99;   // TODO Update Zeroth Index
	numbersList[1] = 0; // TODO Update first Index

	print(numbersList[0]);
	print("\n");

	for (int element in numbersList) {  // TODO Using Individual Element (Objects)
		print(element);
	}

	print("\n");

	numbersList.forEach((element) => print(element)); // TODO Using forEach Lambda

	print("\n");

	for (int i = 0; i < numbersList.length; i++) { // TODO Using For Loop Index
		print(numbersList[i]);
	}
}
```
__Example using Growable List__

```ruby
void main() {

  // TODO Index:       0   1   2   3   4
  // TODO Elements:    73  64  64   21  12
  
  	List<String> countries = ["USA", "INDIA", "CHINA"];  // Growable List : METHOD 1
  	countries.add("Nepal");
  	countries.add("Japan");

	List<int> numbersList  = <int>[]; // TODO Growable list : METHOD 2
	numbersList.add(73);  // TODO Insert operation
	numbersList.add(64);
  	numbersList.add(64);
	numbersList.add(21);
  	numbersList.add(12);

	numbersList[0] = 99;   // TODO Update Zeroth Index
	numbersList[1] = 0; // TODO Update first Index

	print(numbersList[0]);
	print("\n");

	numbersList.add(24);   // TODO For Adding an Element and it won't support in fixed-length list
  	numbersList.remove(73); // TODO For Removing the List using Elements and it won't support in fixed-length list
  	numbersList.removeAt(3); // TODO For Removing the List using index and it won't support in fixed-length list
  	// numbersList.clear(); // TODO For Removing the List using index and it won't support in fixed-length list

	for (int element in numbersList) {  // TODO Using Individual Element (Objects)
		print(element);
	}

	print("\n");

	numbersList.forEach((element) => print(element)); // TODO Using forEach Lambda

	print("\n");

	for (int i = 0; i < numbersList.length; i++) { // TODO Using For Loop Index
		print(numbersList[i]);
	}
}
```

## Need to know

- Data Type that dart Supports - Strings, Numbers(int,double), Boolean, Lists(Arrays), Maps, Symbols and Runes(for expressing unicode character in a String)
- All the Data Types in Dart are Objects and therefore Values are default by null.
- Difference Between For, While and doWhile -> For will used in the Finite (Already know the number of times the loop should be execite) Loops, While and doWhile will be used in the Indefinite (Don't know the how many the code should execute (oe) Execute the Code based on some conditions) Loops.
- In While Loop we will first check the Condition and in doWhile Loop we will execute the code and then we will check the condition.
