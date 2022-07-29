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

## Hello World

```ruby
void main(){ // TODO void main -> It is the Entry Function
  
  print("Hello World");
  
  print(4-3); // TODO Performing Arithematic Operations
  
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

```ruby
void main() {
  
    String mValue = "Hello World"; // TODO Where String - Data Type, mValue - Variable Name and "Hello World" - Value
    print(mValue);
  
    // TODO Numbers: int
    int score = 25;
    var count = 50; // TODO It is inferred as integer automatically by compiler
    int hexValue = 0xEADEBAEE;
  
    // TODO Numbers: double
    double percentage = 95.0;
    var percent = 70.0;
    double exponents = 1.42e5;
  
    // TODO Strings
    String name = "Google";
    var company = "Amazon";
  
    // TODO Boolean
    bool isValid = true;
    var isAlive = false;
    
    print(score);
    print(exponents);
    print(isAlive);
  
    // NOTE: All data types in Dart are Objects.
    // Therefore, their initial value is by default 'null'
}
```  
:arrow_up: [__Back to Top__](Basics.md#table-of-contents)

## Literals and String Interpolation

```ruby
void main() {

    // TODO Literals - It is the Values where you can assign them to a Variables.
    String s1 = 'Hello World'; // TODO Where Hello World is the Literals 
    
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
   
    print("My name is " + name); // TODO Appending the name is just like a bad pratice 
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
  
    // condition ? exp1 : exp2
    // If condition is true, evaluates expr1 (and returns its value);
    // otherwise, evaluates and returns the value of expr2.
    int a = 5;
    int b = 10;
    int smallNumber = a < b ? a : b;
  
    print("$smallNumber is smaller");
  
    // exp1 ?? exp2
    // If expr1 is non-null, returns its value; otherwise, evaluates and
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

__Example__

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


## Need to know

- Data Type that dart Supports - Strings, Numbers(int,double), Boolean, Lists(Arrays), Maps, Symbols and Runes(for expressing unicode character in a String)
- All the Data Types in Dart are Objects and therefore Values are default by null.
- Difference Between For, While and doWhile -> For will used in the Finite (Already know the number of times the loop should be execite) Loops, While and doWhile will be used in the Indefinite (Don't know the how many the code should execute (oe) Execute the Code based on some conditions) Loops.
- In While Loop we will first check the Condition and in doWhile Loop we will execute the code and then we will check the condition.
