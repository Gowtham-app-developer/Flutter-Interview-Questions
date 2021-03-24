# Flutter-Interview-Questions

:point_right: Click :star: if you like the project.   
:point_right: Pull Request are highly appreciated.  
:point_right: Follow me [@Gowtham R](https://twitter.com/Gowtham26730226) for new technical updates.  
:point_right: For Flutter Course visit, this [GitHub Link](https://github.com/AndroidPillars/Flutter)  

## Table of Contents

| S.No | Content |
| --------	 | ------------ |
| 1 | [Flutter](README.md#flutter) |
| 2 | [Why Flutter](README.md#why-flutter) |
| 3 | [MaterialApp Class](README.md#materialapp-class) |
| 4 | [Scaffold Widet](README.md#scaffold-widget) |
| 5 | [pubspec.yaml file](README.md#pubspecyaml-file) |
| 6 | [Hot Reload](README.md#hot-reload) |
| 7 | [Hot Restart](README.md#hot-restart) |
| 8 | [Layout widgets](README.md#core-java) |
| 9 | [Single-child layout widgets](README.md#single-child-layout-widgets) |
| 10 | [Multi-child layout widgets](README.md#multi-child-layout-widgets) |
| 11 | [Difference b/w main() function and the runApp() function in Flutter?](README.md#Difference-bw-main-function-and-the-runapp-function-in-flutter) |
| 12 | [Stateful vs Stateless Widget](README.md#stateful-vs-stateless-widget) |
| 13 | [Difference b/w final and const in Flutter?](README.md#difference-between-final-and-const-in-flutter) |
| 14 | [Widget & Widget tree](README.md#widget--widget-tree) |
| 15 | [Expanded Widget](README.md#expanded-widget) |
| 16 | [SafeArea Widget](README.md#core-java) |
| 18 | [Main Axis Alignment and Cross Axis Alignment](README.md#core-java) |
| 19 | [Lifecycle of a StatefulWidget](README.md#core-java) |
| 20 | [Inherited Widget](README.md#core-java) |
| 21 | [What is an App state?](README.md#core-java) |
| 22 | [Routes & Navigation](README.md#routes--navigation) |
| 23 | [Futures, Asysnc and Await](README.md#futures-asysnc-and-await) |
| 24 | [What are packages and plugins in Flutter?](README.md#what-are-packages-and-plugins-in-flutter) |
| 25 | [Global State](README.md#global-state) |
| 26 | [Vysnc](README.md#vysnc) |
| 27 | [Stream](README.md#stream) |
| 28 | [StreamBuilder](README.md#streambuilder) |
| 29 | [How stream and Future are different?](README.md#how-stream-and-future-are-different) |
| 30 | [Difference b/w @required vs assert](README.md#difference-between-required-vs-assert) |
|    | Dart |
| 1 | [Dart](README.md#dart) |
| 2 | [Anonymous Function](README.md#anonymous-function) |
| 3 | [What is a difference between these operators "?? and ?.](README.md#what-is-a-difference-between-these-operators--and-) |
| 4 | [Final vs Const](README.md#final-vs-const) |
| 5 | [Classes and Objects](README.md#classes-and-objects) |
| 6 | [Constructor](README.md#constructor) |
| 7 | [Inheritance](README.md#inheritance) |
| 8 | [Abstraction](README.md#abstraction) |
| 9 | [Null safety in Dart](README.md#null-safety-in-dart) |
| 10 | [Computed Properties](README.md#computed-properties) |
| 11 | [Static Modifier](README.md#static-modifier) |
| 12 | [Mixins](README.md#mixins) |

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
- It contains widgets that are used for the material design of an application.

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

- The pubspec.yaml is a file where you can provide all the dependencies (optional and required — e.g., plugins, Dart version, font, images) of your Flutter project and also a     place where you configure the project’s name and description.
- For Android developers, this is slightly similar to a build.gradle file.
- yaml is a special type of file called yaml file which stands for YAML Ain't Markup Language.

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
- Examples: Align, AspectRatio, Baseline, Center, ConstrainedBox, Container, CustomSingleChildLayout, Expanded, FittedBox, FractionallySizedBox, IntrinsicHeight, IntrinsicWidth,
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
- Examples: Column, CustomMultiChildLayout, Flow, GridView, IndexedStack, LayoutBuilder, ListBody, ListView, Row, Stack, Table and Wrap

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
:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)

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

```ruby
class Car extends StatefulWidget {  
  const Car({ Key key, this.title }) : super(key: key);   
  
  @override  
  _CarState createState() => _CarState();  
}  
  
class _CarState extends State<Car> {  
  @override  
  Widget build(BuildContext context) {  
    return Container(  
      color: const Color(0xFEEFE),  
           child: Container(  
            child: Container(child: Container())
        )  
    );  
  }  
}  
```  
:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)

## Difference between final and const in Flutter?

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
:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)

## Widget & Widget tree

- __Widget__ is a description of a part of UI(i.e.) Widget is a way to declare and construct UI.
- In Flutter, everything is a widget(i.e) Widgets are the basic building blocks of the user interface.
- For example, Button, text, image, list, Padding, Margin, Center, Layout rows and columns, etc. 
- __Widget tree__ is a structure that represents how our widgets are organized. 
- Web pages have a DOM and Flutter have a Widget Tree.

![flutter-widgets](https://user-images.githubusercontent.com/78175168/111944398-8ead1980-8afd-11eb-80d5-af29c5e8b775.png)


:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)

## Expanded Widget

- By Using an Expanded widget makes a child of a Row, Column, or Flex expand to fill the available space along the main axis (e.g., horizontally for a Row or vertically for a     Column).

```ruby
class DicePage extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Center(
      child: Padding(
        padding: const EdgeInsets.all(8.0),
        child: Center(
          child: Row(
            children: <Widget>[
              Expanded(
                flex: 2,
                child: Padding(
                  padding: const EdgeInsets.all(16.0),
                  child: Image.asset('images/dice1.png'),
                ),
              ),
              Expanded(
                flex: 2,
                child: Padding(
                  padding: const EdgeInsets.all(16.0),
                  child: Image(
                    image: AssetImage('images/dice1.png'),
                  ),
                ),
              ),
            ],
          ),
        ),
      ),
    );
  }
}
```  
:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)

## SafeArea Widget

- SafeArea is basically a padding widget, which adds any necessary padding to your app, based on the device it is running on.
- If your app’s widgets are overlaying any of the system’s features like notches, status bar, camera holes, or any other such features, then SafeArea would add padding around     the app, as required.

```ruby
SafeArea(
  minimum: const EdgeInsets.all(16.0),
  child: Text('My Widget'),
)
```  
:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)

## Main Axis Alignment and Cross Axis Alignment

- The mainAxisAlignment property aligns all the content of Column widget relative to the main axis of Column widget, and crossAxisAlignment property aligns all the content         relative to the cross axis of Column widget.
- The Main Axis for Column widget is the Vertical Axis,(i.e.) “Y Axis”, as it is mainly on vertical Axis, and the Cross Axis for the Column widget is Horizontal Axis, i.e., “X-   Axis”, as the Column widget is crossing the X-Axis.

![omg_one](https://user-images.githubusercontent.com/78175168/111883311-83180080-89e0-11eb-8a98-059c6d640ad0.png)

:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)

## Lifecycle of a StatefulWidget

## Routes & Navigation

- Navigation and routing are some of the core concepts of all mobile application, which allows the user to move between different pages.
- In Flutter, the screens and pages are known as routes, and these routes are just a widget.
- In Android, a route is similar to an Activity, whereas, in iOS, it is equivalent to a ViewController.
- In any mobile app, navigating to different pages defines the workflow of the application, and the way to handle the navigation is known as routing.
- Flutter provides a basic routing class MaterialPageRoute and two methods Navigator.push() and Navigator.pop() that shows how to navigate between two routes.
- Flutter also supports named routes, which are defined in the routes parameter on MaterialApp or CupertinoApp.

__Example [Push uisng Anonymous routes]__
```ruby
onPressed: () {
  Navigator.push(
    context,
    MaterialPageRoute(builder: (context) => SecondRoute()),
  );
}
```
__Example [Pop]__
```ruby
onPressed: () {
  Navigator.pop(context);
}
```

__Example [Push uisng named routes]__
```ruby
return MaterialApp(
   routes: {
    '/': (context) => HomeScreen(),
    '/details': (context) => DetailScreen(),
   },
);
```
:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)  

## Futures, Asysnc and Await

- __Async__ means that this function is asynchronous and you might need to wait a bit to get its result.
- __Await__ literally means - wait here until this function is finished and you will get its return value.
- __Future__ is a type that ‘comes from the future’ and returns value from your asynchronous function. 
- It can complete with success(.then) or with an error(.catchError).
- __.Then((value){…})__ is a callback that’s called when future completes successfully(with a value).

__Example for Synchronous__

```ruby
import 'dart:io';

void main() {
  performTasks();
}

void performTasks() {
  task1();
  task2();
  task3();
}

void task1() {
  String result = 'task 1 data';
  print('Task 1 complete');
}

void task2() {
  Duration threeSeconds = Duration(seconds: 3);
  sleep(threeSeconds);
  String result = 'task 2 data';
  print('Task 2 complete');
}

void task3() {
  String result = 'task 3 data';
  print('Task 3 complete');
}
```

__Example for Asynchronous__

```ruby
import 'dart:io';

void main() {
  performTasks();
}

void performTasks() {
  task1();
  task2();
  task3();
}

void task1() {
  String result = 'task 1 data';
  print('Task 1 complete');
}

void task2() {
  Duration threeSeconds = Duration(seconds: 3);
  Future.delayed(threeSeconds, () {
    String result = 'task 2 data';
    print('Task 2 complete');
  });
}

void task3() {
  String result = 'task 3 data';
  print('Task 3 complete');
}
```

__Example for Futures, Asysnc and Await__

```ruby
import 'dart:io';

void main(){
  performTasks();
}

void performTasks() async{
  task1();
  String taskTwoResult = await task2();
  task3(taskTwoResult);
}

void task1() {
  String result = 'task 1 data';
  print('Task 1 complete');
}

Future task2() async{
  Duration threeSeconds = Duration(seconds: 3);
  String result;
  Future.delayed(threeSeconds, () {
    result = 'task 2 data';
    print('Task 2 complete');
  });

  return result;
}

void task3(String resultData) {
  String result = 'task 3 data';
  print('Task 3 complete$resultData');
}
```
:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)  

## What are packages and plugins in Flutter? 

- The __plugin__ contains both Dart and Native code (kotlin, js and swift).
- The __package__ contains only Dart code.
- The __package__ can use plugins if it wants to and it will still qualify as a package.  

:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)  

## Global State 

- Global state allows you to put data into a global object that can be accessed from any widget. 
- No need to pass around state between different widgets.
- Although global state allows your data to be shared and easily accessible from different widgets, it does not replace local state. 
- They are both different and are used in different context.
- There are several different ways of managing global state in Flutter and Some of them are BLoC, Redux, Inherited Widget, Inherited Model and Scoped Model.

:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)  

## Vysnc

- Vsync basically keeps the track of screen, so that Flutter does not renders the animation when the screen is not being displayed.
- We can create animations using SingleTickerProviderStateMixin or TickerProviderStateMixin.

__Example__

```ruby
class _WelcomeScreenState extends State<WelcomeScreen>
    with SingleTickerProviderStateMixin {
  AnimationController controller;
  Animation animation;

  @override
  void initState() {
    super.initState();

    controller = AnimationController(
      duration: Duration(seconds: 1),
      vsync: this,
    );

    animation = ColorTween(begin: Colors.blueGrey, end: Colors.white)
        .animate(controller);
    controller.forward();
    controller.addListener(() {
      setState(() {});
    });
  }
```
:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)  

## Stream

- Streams provide an asynchronous sequence of data.
- By subscribing to the stream of meassages you are essentailly able to get the piece of data as they come in and as they get added to the stream.
- Dart snapshots method gives us a stream and we can handle the stream using the widgets called StreamBuilder.
- There are two kinds of streams Single Subscription and Broadcast.
- __Single Subscription__ There could be a maximum of one listener to this stream.
- __Broadcast__ There could be the infinite number of the listener to this stream.

```ruby
@override
Widget build(BuildContext context) {
  return StreamBuilder<QuerySnapshot>(
    stream: _firestore.collection('messages').snapshots(),
    builder: (context, snapshot) {
      if (!snapshot.hasData) {
        return Center(
          child: CircularProgressIndicator(
            backgroundColor: Colors.lightBlueAccent,
          ),
        );
      });
```

:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)   

## StreamBuilder

- It will turn our snapshots of data in to actual widgets when the new data arrives from the Stream it will get reduild.
- It will get done using the set state.
- In other words, set state will called every time there's a new value in the stream.
- It consists of two important things stream and builder.
- __stream__ In particular, it's a stream of query snapshots and it knows when new data comes to rebuild itself.
- __builder__ We have to provied the logic for the stream builder should actually do.

```ruby
@override
Widget build(BuildContext context) {
  return StreamBuilder<QuerySnapshot>(
    stream: _firestore.collection('messages').snapshots(),
    builder: (context, snapshot) {
      if (!snapshot.hasData) {
        return Center(
          child: CircularProgressIndicator(
            backgroundColor: Colors.lightBlueAccent,
          ),
        );
      });
```
:arrow_up: [__Back to Top__](README.md#flutter-interview-questions) 

## How stream and Future are different?

- A stream is a combination of Futures
- Future has only one response but Stream could have any number of Response.
- But both works asynchronously and some potential value  

:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)  

## Difference b/w @required vs assert

- __@required__ is an annotation that will create a warning for you to remember that the named parameter is necessary for the class to work as expected.

```ruby
class Test {
  final String a; // say a is mandatory
  final String b;

  Test({
    @required this.a, // annotate it using required
    this.b,
  });
```
- __assert__ stops execution if a boolean condition is false.
- It is mainly useful to check the programming errors like null and it will execute only in the debug mode.

```ruby
import 'package:meta/meta.dart';

class Product {
  final int id;
  final String name;
  final int price;
  final String size;
  final String image;
  final int weight;

  const Product({
    @required this.id,
    @required this.name,
    @required this.price,
    this.size,
    this.image,
    this.weight,
  }) : assert(id != null && name != null && price != null);
}
```  
:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)  

## Dart

- Dart is an open-source, general-purpose, object-oriented programming language with C-style syntax developed by Google in 2011.
- It is a statically typed language.
- Dart compiles to modern JavaScript to run in the browser and compiles to native code to run on mobile platforms like Android and iOS.
- It is Productive and Fast because of using JIT compiler [Hot Reload] and AOT compiler.

:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)  

## Anonymous Function

- An anonymous function is a function without a name. 
- An anonymous function allows us to tell the computer to do something without explicitly having to create this entire function by giving it a name and call its name.
- For example when we were coding up on our on pressed which expected a void callback.

```ruby
(){
//To Do Something
}
```

__Example in Dart using Anonymous Function__

```ruby
onPressed: (){
//To Do Something
}
```
:arrow_up: [__Back to Top__](README.md#flutter-interview-questions) 

## What is a difference between these operators "?? and ?.

- Null-aware operators in dart allow you to make computations based on whether or not a value is null. 
- It’s shorthand for longer expressions.

__Default operator(??)__

- Use ?? when you want to evaluate and return an expression if another expression resolves to null.

__Syntax__

```ruby
var value = mVariable ?? defaultValue
```
__Safe navigation operator(?.)__

- We can use nullable types by appending a question mark ? to a variable type

```ruby
class Car {
  String name;
}

void main() {
  Car hyundai;
  // prints null
  print(hyundai?.name);
  // throws null is not an object exception
  print(hyundai.name);
}
```
:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)  

## Final vs Const

- If you never intend to change a variable then we have to declare using the keyword final or const.
- The __final__ variable can be set only once.
- The __const__ variable is a compile-time constant.(Const variables are implicitly final.) 

__Example__

```ruby
void main() {
  const int myCount = 3;
  final  mDate = DateTime.now();
  
  print(myCount);
  print(mDate);
}
```
:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)  

## Classes and Objects

- A template (blueprint) for creating objects (the real thing) that we're going to showing in our app.
- A class has two important things (i.e.) Properties and Methods.
- Example: If we take a car color and numberOfSeats is properties and drive(), break() is Methods.
- It is a basic unit of Object Oriented Programming and represents the real life entities.
- For example, we can take a Car -> Car is an object.

__Example__

```ruby
class car {
  
  int numberOfDoors = 5;
  
  void drive(){
    print('wheels start turning');
  }
    
}
```

- where int numberOfDoors = 5 is the varaible(i.e.) Properties and void drive() is the function(i.e.) Methods

:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)  

## Constructor

- Constructor is a block of code that initializes the newly created object.
- Constructor resembles an instance method in java but it’s not a method as it doesn’t have a return type.
- It is called when an instance of the class is created. 
- At the time of calling constructor, memory for the object is allocated in the memory.
- It calls a default constructor if there is no constructor available in the class.

__Example__

```ruby
void main(){
  
  Human mHuman = Human(mHeight: 10.0);
  
  print(mHuman.height);
  
  mHuman.talk('Hello World');
 
}

class Human{
  
  double height;
  int age = 60;
  
  Human({double mHeight}){
    height = mHeight;
  }
  
  void talk(String mStringText){
    print(mStringText);
  }
}
```
:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)  

## Inheritance

- Inheritance is the process by which objects of one class acquire the properties & methods of another class. 
- It provides code reusability. 
- It is used to achieve runtime polymorphism.

__Example__

```ruby
void main(){
  
  Monkey mMonkey = Monkey();
  print(mMonkey.height);
  
  mMonkey.talk('Hello World');
  mMonkey.monkeWeight();
}

class Human{
  
  double height = 10.0;
  int age = 60;
  
  void talk(String mStringText){
    print(mStringText);
  }
}

class Monkey extends Human{
  
  double weight = 150.0;
  
  void monkeWeight(){
     print('Weight$weight');
  } 
}
```
:arrow_up: [__Back to Top__](README.md#flutter-interview-questions) 

## Abstraction

- Abstraction is a process of hiding the implementation details and showing only functionality to the user.
- It can have abstract and non-abstract methods (method with the body).
- In other words, Split up the functionality in to different Component.

__Example__

```ruby
abstract class Shape {
	double area();
}

class Square implements Shape{
	Square({this.side});
  final double side;
  double area() => side * side;
}

void main(){
	final square = Square(side: 10.0);
  print(square.area());
}
```
:arrow_up: [__Back to Top__](README.md#flutter-interview-questions) 

## Null safety in Dart

- Null safety is a major new productivity feature that helps you avoid null exceptions, a class of bugs that are often hard to spot.
- Dart is a type-safe language. 
- This means that when you get a variable of some type, the compiler can guarantee that it is of that type. 
- But type safety by itself doesn’t guarantee that the variable is not null.
- You can use nullable types by appending a question mark ? to a variable type as of in the below example,

__Example__

```ruby
void main() {
  String? word;
  
  print(word); // prints null
}
```

:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)  

## Computed Properties

- Computed Properties are the features of Dart language that can be used to define properties whose value is computed reather than stored.
- Getters and setters are special methods that provide explicit read and write access to an object's properties.

__Example__

```ruby
abstract class Shape {
	double get area;
}

class Square implements Shape{
	Square({this.side});
  final double side;
  double get area => side * side;
}

void main(){
	final square = Square(side: 10.0);
  print(square.area);
}
```
:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)  

## Static Modifier

- Static means that you don't have to create an instance of the class to use the methods or variables associated with the class.
- Static is a non-access modifier applicable only to a blocks, variables, methods and nested classes.
- Static Keyword in Java is used for memory management mainly.

```ruby
void main() {

 Square.workout(radius : 5.44);
  
}

class Square {
  
  static int numberOfSides = 4;
  
  static void workout({double radius}){
    double calculation = 2 * numberOfSides * radius;
    print(calculation);
  }
  
}
```
:arrow_up: [__Back to Top__](README.md#flutter-interview-questions) 

## Mixins

- In object-oriented programming languages, a Mixin is a class that contains methods for use by other classes without having to be the parent class of those other classes.
- In other words mixins are normal classes from which we can borrow methods(or variables) from without extending the class.
- In dart we can do this by using the keyword with.

__Example__

```ruby
void main() {

 Animal().move();
 Duck().fly();
}

class Animal {
  
  void move(){
    print('Dynamic Value');
  }
}
  
mixin CanSwim {
  void swim(){
    print('Swim');
  }
}

mixin CanFly {
  void fly(){
    print('Fly');
  }
}

class Duck extends Animal with CanSwim, CanFly{
 
}
```
:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)  

