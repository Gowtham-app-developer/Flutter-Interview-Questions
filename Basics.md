# Flutter-Basics

## Table of Contents

| S.No | Content |
| --------	 | ------------ |
| 1 | [Hello World](Basics.md#adding-comment-line) |

## Hello World

```ruby
// TODO void main is the Entry Function

void main(){
  
  print("Hello World");
  
  print(4-3); // Performing Arithematic Operations
  
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
:arrow_up: [__Back to Top__](Basics.md#table-of-contents 

## Variable Declration

```ruby
void main() {
  
    String mValue = "Hello World"; // Where String - Data Type, mValue - Variable Name and "Hello World" - Value
    print(mValue);
  
    // TODO Numbers: int
    int score = 25;
    var count = 50; // It is inferred as integer automatically by compiler
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
## Literals and String Interpolation

```ruby
void main() {

    // TODO Literals - It is the Values where you can assign them to a Variables.
    String s1 = 'Hello World'; // Where Hello World is the Literals 
    
    // TODO Various ways to define String Literals in Dart
    String s2 = 'Hello World';
    String s3 = "Hello World";
    String s4 = 'It\'s easy';
    String s5 = "It's easy";
    String s6 = 'Hello my Self Gauthy completed B.E in Electronics and Communication'
    'Engineering';
   
    print(s6);
   
   // String Interpolation
    String name = "Hello World";
   
    print("My name is " + name); // Appending the name is just like a bad pratice 
    print("My name is $name"); // String Interpolation
    print("The number of characters in String Kevin is ${name.length}");
    
    int l = 20;
    int b = 10;
    
    print("The sum of $l and $b is ${l + b}");
    print("The area of rectangle with length $l and breadth $b is ${l * b}");
}
```

## Need to know

- Data Type that dart Supports - Strings, Numbers(int,double), Boolean, Lists(Arrays), Maps, Symbols and Runes(for expressing unicode character in a String)
- All the Data Types in Dart are Objects and therefore Values are default by null.
