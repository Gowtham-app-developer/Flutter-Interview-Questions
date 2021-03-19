# Flutter-Interview-Questions

:point_right: Click :star: if you like the project.   
:point_right: Pull Request are highly appreciated.  
:point_right: Follow me [@Gowtham R](https://twitter.com/Gowtham26730226) for new technical updates.  

| S.No | Content |
| --------	 | ------------ |
| 1 | [Flutter](README.md#flutter-1) |
| 2 | [Why Flutter](README.md#why-flutter) |
| 3 | [MaterialApp Class](README.md#materialapp-class) |
| 4 | [Scaffold Widet](README.md#scaffold-widget) |
| 5 | [pubspec.yaml file](README.md#pubspecyaml-file) |
| 6 | [Hot Reload](README.md#hot-reload) |
| 7 | [Hot Restart](README.md#hot-restart) |
| 8 | [Layout widgets](README.md#core-java) |
| 9 | [Single-child layout widgets](README.md#single-child-layout-widgets) |
| 10 | [Multi-child layout widgets](README.md#multi-child-layout-widgets) |
| 11 | [Difference b/w main() function and the runApp() function in Flutter?](README.md#difference-bw-main-function-and-the-runapp-function-in-flutter) |
| 12 | [Stateful vs Stateless Widget](README.md#stateful-vs-stateless-widget) |
| 13 | [Difference b/w final and const in Flutter?](README.md#difference-between-final-and-const-in-flutter) |
| 14 | [Widget](README.md#core-java) |
| 14 | [Expanded Widget](README.md#core-java) |
| 16 | [SafeArea Widget](README.md#core-java) |
| 18 | [main Axis Alignment and cross Axis Alignment](README.md#core-java) |
| 19 | [lifecycle of a ‘StatefulWidget’](README.md#core-java) |
| 20 | [InheritedWidget](README.md#core-java) |
| 21 | [What is an App state?](README.md#core-java) |

## Flutter

- Flutter is a mobile UI framework developed by google which allows us to build both Android, IOS and even web with one single code base.
- Flutter apps are built using the Dart programming language.
- In Flutter, everything is a widget(i.e) Widgets are the basic building blocks of the user interface.
- Dart uses Flutter SDK which converts or compiles in to native code on both Android and IOS.  

:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)

## Why Flutter

- It is a single code base.
- Dart is a powerful language that is quite easy to work and is very similar to Oops and we can learn easily.
- We can use Flutter and Dart to build Android, IOS mobile Apps and even web application that run on your desktop.
- Flutter allows you to build a simple and Flexible layout system to build beautiful interfaces.
- Hot Reload -> Instant run with in a Second.
- It's a Open source.  

:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)

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
:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)

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

:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)

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

:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)

## Hot Reload

- Hot reload feature quickly compile the newly added code in our file and sent the code to Dart Virtual Machine.
- Once done updating the Code Dart Virtual Machine update the app UI with widgets.
- Hot Reload takes less time then Hot restart.
- There is also a draw back in Hot Reload, If you are using States in your application then Hot Reload preservers the States so they will not update on Hot Reload our set to       their default values.  

:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)

## Hot Restart

- Hot restart is much different than hot reload.
- In Hot restart it destroys the preserves State value and set them to their default.
- So if you are using States value in your application then after every hot restart the developer gets fully compiled application and all the states will set to their             defaults.
- The app widget tree is completely rebuilt with new typed code. 
- Hot Restart takes much higher time than Hot reload.  

:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)

## Layout widgets

- Two Types -> Single-child layout widgets & Multi-child layout widgets.  

:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)

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
:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)

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
:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)

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

## Stateful vs Stateless Widget

__Stateless Widget__

- A widget that has an immutable state.
- Stateless Widgets are static widgets.
- They do not depend on any data change or any behavior change.
- Stateless Widgets do not have a state, they will be rendered once and will not update themselves, but will only be updated when external data changes.
- For Example: Text, Icon, RaisedButton are Stateless Widgets.

__Example__

```ruby
class Screen extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return null;
  }
}
```

__Stateful Widget__

- A widget that has a mutable state.
- Stateful Widgets are dynamic widgets.
- They can be updated during runtime based on user action or data change.
- Stateful Widgets have an internal state and can re-render if the input data changes or if the Widget’s state changes.
- For Example: Checkbox, Radio Button, Slider are Stateful Widgets.

## difference between final and const in Flutter?

- If you never intend to change a variable then we have to declare using the keyword final or const.
- In __const__ Value must be known at compile-time, const birthday = "2020/07/28" Can't be changed after initialized.
- In __final__ Value must be known at run-time, final birthday = getBirthDateFromDB() Can't be changed after initialized.

__Example__

```ruby
void main() {
  const int myCount = 3;
  final  mDate = DateTime.now();
  
  print(myCount);
  print(mDate);
}
```

## Widget

- Widget is a description of a part of UI(i.e.) Widget is a way to declare and construct UI.
- In Flutter, everything is a widget(i.e) Widgets are the basic building blocks of the user interface.
- For example, Button, text, image, list, Padding, Margin, Center, Layout rows and columns, etc.

## Expanded Widget

- By Using an Expanded widget makes a child of a Row, Column, or Flex expand to fill the available space along the main axis (e.g., horizontally for a Row or vertically for a     Column).
