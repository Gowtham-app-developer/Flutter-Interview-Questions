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

## Scaffold Widget

- A Scaffold Widget provides a framework which implements the basic material design visual layout structure of the flutter app. 
- A Scaffold Widget is used under MaterialApp, it gives you many basic functionalities like AppBar, BottomNavigationBar, Drawer, FloatingActionButton etc.
- It provides APIs for showing drawers, snack bars and bottom sheets. 

```ruby
import 'package:flutter/material.dart';

void main() => runApp(
      MaterialApp(
        home: Scaffold(
          backgroundColor: Colors.blueGrey,
          appBar: AppBar(
            centerTitle: true,
            title: Text('Home'),
            backgroundColor: Colors.blueGrey[900],
          ),
          body: Center(
            child: Image(
              image: NetworkImage(
                  'https://www.w3schools.com/w3css/img_lights.jpg'),
            ),
          ),
        ),
      ),
    );
```

## pubspec.yaml file

- This is a special type of file called yaml file which stands for YAML Ain't Markup Language.
- The pubspec.yaml is a file where you can provide all the dependencies (optional and required — e.g., plugins, Dart version, font, images) of your Flutter project and also a     place where you configure the project’s name and description.
- For Android developers, this is slightly similar to a build.gradle file.

```ruby
flutter:

  # The following line ensures that the Material Icons font is
  uses-material-design: true

  # To add assets to your application, add an assets section, like this:
  assets:
    - images/

```
