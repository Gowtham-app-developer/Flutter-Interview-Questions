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

__Example__

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

__Example__

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

__Example__

```ruby
flutter:

  # The following line ensures that the Material Icons font is
  uses-material-design: true

  # To add assets to your application, add an assets section, like this:
  assets:
    - images/

```

## Hot Reload

- Hot reload feature quickly compile the newly added code in our file and sent the code to Dart Virtual Machine.
- Once done updating the Code Dart Virtual Machine update the app UI with widgets.
- Hot Reload takes less time then Hot restart.
- There is also a draw back in Hot Reload, If you are using States in your application then Hot Reload preservers the States so they will not update on Hot Reload our set to       their default values. 

## Hot Restart

- Hot restart is much different than hot reload.
- In Hot restart it destroys the preserves State value and set them to their default.
- So if you are using States value in your application then after every hot restart the developer gets fully compiled application and all the states will set to their             defaults.
- The app widget tree is completely rebuilt with new typed code. 
- Hot Restart takes much higher time than Hot reload.

## Layout widgets

- Two Types -> Single-child layout widgets & Multi-child layout widgets.

## Single-child layout widgets 

- The single child layout widget is a type of widget, which can have only one child widget inside the parent layout widget.
- Align, AspectRatio, Baseline, Center, ConstrainedBox, Container, CustomSingleChildLayout, Expanded, FittedBox, FractionallySizedBox, IntrinsicHeight, IntrinsicWidth,
  LimitedBox, Offstage, OverflowBox, Padding, SizedBox, SizedOverflowBox and Transform.
  
__Example__

```ruby
import 'package:flutter/cupertino.dart';
import 'package:flutter/material.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        backgroundColor: Colors.teal,
        body: SafeArea(
            child: Container(
              height: 100.0,
              width: 100.0,
              margin: EdgeInsets.only(left: 30.0),
              padding: EdgeInsets.all(20.0),
              child: Text('Hello World'),
              color: Colors.orange,
            ),
          ),
      ),
    );
  }
}
```

## Multi-child layout widgets

- The multiple child widgets are a type of widget, which contains more than one child widget, and the layout of these widgets are unique. 
- Column, CustomMultiChildLayout, Flow, GridView, IndexedStack, LayoutBuilder, ListBody, ListView, Row, Stack, Table and Wrap

__Example__

```ruby
import 'package:flutter/material.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        backgroundColor: Colors.teal,
        body: SafeArea(
            child: Column(
              crossAxisAlignment: CrossAxisAlignment.stretch,
              children: <Widget>[
                Container(
                  height: 100.0,
                  child: Text('Container 1'),
                  color: Colors.orange,
                ),
                SizedBox(height: 20.0,),
                Container(
                  height: 100.0,
                  child: Text('Container 2'),
                  color: Colors.blue,
                ),
                SizedBox(height: 20.0,),
                Container(
                  height: 100.0,
                  child: Text('Container 3'),
                  color: Colors.red,
                ),
              ],
        )),
      ),
    );
  }
}
```

## Difference b/w main() function and the runApp() function in Flutter?

- In Dart, __main()__ acts as the entry point for the program whereas __runApp()__ attaches the given widget to the screen.

__Example__

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
