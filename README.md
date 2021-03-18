# Flutter-Interview-Questions

# Topics

## Flutter

| S.No | Content |
| --------	 | ------------ |
| 1 | [Flutter](https://github.com/AndroidPillars/Flutter/blob/master/CHAPTER-1.md#what-is-flutter) |
| 2 | [Why Flutter](https://github.com/AndroidPillars/Flutter/blob/master/CHAPTER-1.md#why-flutter) |
| 3 | [MaterialApp Class](https://github.com/AndroidPillars/Flutter/blob/master/CHAPTER-2.md#materialapp-class) |
| 4 | [Scaffold Widet](https://github.com/AndroidPillars/Flutter/blob/master/CHAPTER-2.md#scaffold-widet) |
| 5 | [Assets and pubspec file](https://github.com/AndroidPillars/Flutter/blob/master/CHAPTER-2.md#working-with-assets-and-pubspec-file) |
| 6 | [MaterialApp Class](README.md#core-java) |
| 7 | [Stateful vs Stateless Widget](README.md#core-java) |
| 8 | [Hot Reload](README.md#core-java) |
| 9 | [Hot Restart](README.md#core-java) |
| 10 | [Single-child layout widgets](README.md#core-java) |
| 11 | [Multi-child layout widgets](README.md#core-java) |
| 12 | [Material Icons](README.md#core-java) |
| 13 | [Widget](README.md#core-java) |
| 14 | [Expanded Widget](README.md#core-java) |
| 15 | [Material Icons](README.md#core-java) |
| 16 | [SafeArea Widget](README.md#core-java) |
| 17 | [pubspec.yaml file](README.md#core-java) |
| 18 | [main Axis Alignment and cross Axis Alignment](README.md#core-java) |
| 19 | [lifecycle of a ‘StatefulWidget’](README.md#core-java) |
| 20 | [InheritedWidget](README.md#core-java) |
| 21 | [difference between "main()" and "runApp()" functions in Flutter](README.md#core-java) |
| 22 | [What is an App state?](README.md#core-java) |

## Flutter

- Flutter is a mobile UI framework developed by google which allows us to build both Android, IOS and even web with one single code base.
- Flutter apps are built using the Dart programming language.
- In Flutter, everything is a widget(i.e) Widgets are the basic building blocks of the user interface.
- Dart uses Flutter SDK which converts or compiles in to native code on both Android and IOS.

## Why Flutter

- It is a single code base.
- Dart is a powerful language that is quite easy to work and is very similar to Oops and we can learn easily.
- We can use Flutter and Dart to build Android, IOS mobile Apps and even web application that run on your desktop.
- Flutter allows you to build a simple and Flexible layout system to build beautiful interfaces.
- Hot Reload -> Instant run with in a Second.
- It's a Open source.

## MaterialApp Class

- MaterialApp is a predefined class in a flutter.
- It is likely the main or core component of flutter.
- We can access all the other components and widgets provided by Flutter SDK in our App.

```ruby
import 'package:flutter/material.dart';

void main() => runApp(
      MaterialApp(
        home: Center(
          child: Text('Hello world'),
        ),
      ),
    );
```  
