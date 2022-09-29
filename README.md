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
| 26 | [What is Ticker, Animated Controller and Animation Value?](README.md#what-is-ticker-animated-controller-and-animation-value) |
| 27 | [Vysnc](README.md#vysnc) |
| 28 | [Stream](README.md#stream) |
| 29 | [StreamBuilder](README.md#streambuilder) |
| 30 | [How stream and Future are different?](README.md#how-stream-and-future-are-different) |
| 31 | [Difference b/w @required vs assert](README.md#difference-bw-required-vs-assert) |
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
| 13 | [List vs Map](README.md#list-vs-map) |
| 14 | [Generics](README.md#generics) | 
| 15 | [Method Overriding](README.md#method-overriding) |
| 16 | [Interface](README.md#interface) | 
| 17 | [Static Keyword](README.md#static-keyword) | 
| 18 | [Lambda Expression](README.md#lambda-expression) |
| 19 | [Higher Order Function](README.md#higher-order-function) |

## Flutter

- Flutter is a mobile UI framework developed by google which allows us to build both Android, IOS and even web with one single code base.
- Flutter apps are built using the Dart programming language.
- In Flutter, everything is a widget(i.e) Widgets are the basic building blocks of the user interface.
- Dart uses Flutter SDK which converts or compiles in to native code on both Android and IOS whereas in ReactNative it is partially compiled (i.e.) UI Components only.  

:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)

## Why Flutter

- Dart is a strongly typed language (Statically Typed) Object Oriented Language developed by Google which is quite easy to work.
- By Using single code base we can build Android, IOS mobile Apps and even web application that run on your desktop.
- Flutter allows you to build a simple and Flexible layout system to build beautiful interfaces.  
- For Developers, It supports Faster compilation during development (i.e.) It supports JIT(Just In Time) Compilation -> Hot Reload -> Instant run with in a Second.
- For End Uers, When App is Released it uses AOT (Ahead Of Time) Compilation which helps in faster execution on our devices.
- It gives similar experience compared to Native Apps like Android and IOS.
- It's a Open source.  

__Need to Know__

- Drawbacks of Native App -> Have to Create Two Seperate Apps for both Platforms (i.e.) Two Seperate Code base which difficult to Maintain.
- Drawbacks of Web App -> The performance of this application are not so native (i.e.) It makes the user experience slightly poor and it doesn't support many android and IOS features. 
- Drawbacks of other Hybrid Application (Xamarin, Ionic, Cordova and ReactNative) -> Lacking lot of Features in this Framework. 

:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)

## MaterialApp Class

- MaterialApp is a predefined class in a flutter.
- It is likely the main or core component of flutter.
- It contains widgets that are used for the material design of an application.
- By Default Material Design is built into Flutter but you also find Apple-styled(Cupertino) widgets.

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

- Only StatefulWidget hold state and the Lifecyle of it is as follows,
- __createState () :__ When we build a new StatefulWidget, this one calls createState() right away and this override method must exist
- __initState() :__ it is the first method called after the Widget is created.This is our equivalent to onCreate() and viewDidLoad()
- __didChangeDependencies() :__ This method is called immediately after initState() on the first time the widget is built
- __build() :__ called right after didChangeDependencies(). All the GUI is render here and will be called every single time the UI needs to be render
- __didUpdateWidget() :__ it’ll be called once the parent Widget did a change and needs to redraw the UI
- __deactivate() :__ framework calls this method whenever it removes this State object from the tree
- __dispose() :__ is called when this object and its State is removed from the tree permanently and will never build again.

![life_cycle](https://user-images.githubusercontent.com/78175168/112377615-fc2e9500-8d0b-11eb-9a4d-fdc099b99a71.png)  

:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)  

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

## What is Ticker, Animated Controller and Animation Value?

- It is setup and controlled in three components(i.e.)Ticker, AnimationController and Animation / Tween.
- __Ticker__ - It tells us Changes in value or colour(i.e.)  It triggers a new state so that we can render something different on screen.
- __Animation Controller__ - It is the animation controler class which is going to tell the animation to start, to stop, to go forwards, to loop back, how long to animate for,   all of these things are determined when we create an animation controller and set it's properties.
- __Animation Value__ - It is the thing that actually does the animation.
- The animation values will go from 0 to 1 and by using the value, we can able to change  things such as height, size, color and opacity of a component.  

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

- Stream provide an asynchronous sequence of data.
- By subscribing to the stream of meassages you are essentailly able to get the piece of data as they come in and as they get added to the stream.
- Dart snapshots method gives us a stream and we can handle the stream using the widgets called StreamBuilder.
- There are two kinds of streams Single Subscription and Broadcast.
- __Single Subscription__ There could be a maximum of one listener to this stream and it listens to values coming out of the stream.
- __Broadcast__ There could be the infinite number of the listener to this stream.


__Example__

```ruby
import 'dart:async';

void main() {
  final controller = StreamController();
  
  controller.sink.add(1);
  controller.sink.add(2);
  
  controller.stream.listen((value){
  print(value);
  });
}
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

__Example__  

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

__Example__

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

- If you never want to change a variable then we have to declare using the keyword final or const.
- The __final__ variable can be set only once and is initialized only when we accessed (i.e.) Variables will not be initialized unless we not use it in our Code.
- The __const__ variable are implicitly final but it is a compile-time constant (i.e.) It is initialized during Compilation.

__Need to Know__

- Instance variable can be final but cannot be const.
- If we want to use a const at class level then make it as static const

__Example 1__

```ruby
void main() {
  const int myCount = 3;
  final  mDate = DateTime.now();
  
  print(myCount);
  print(mDate);
}
```

__Example 2__

```ruby
void main() {
    // TODO final
    final mCityName = 'TamilNadu';
    // name = 'Peter'; // TODO Throws an error
  
    // TODO const
    const PI = 3.14;
    const double gravity = 9.8;
}

class Circle {
    final color = 'Red';
    static const PI = 3.14; // TODO If we want to use a const at class level then make it as static const
}
```

:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)  

## Classes and Objects

- A template (blueprint) for creating objects (the real thing) that we're going to showing in our app.
- A class has two important things (i.e.) Properties and Methods.
- Example: If we take a car color and numberOfSeats is properties and drive(), break() is Methods.
- It is a basic unit of Object Oriented Programming and represents the real life entities.
- For example, we can take a Car -> Car is an object.

__Example 1__

```ruby
class car {
  
  int numberOfDoors = 5;
  
  void drive(){
    print('wheels start turning');
  }
    
}
```

- where int numberOfDoors = 5 is the varaible(i.e.) Properties and void drive() is the function(i.e.) Methods  

__Example 2__

```ruby
void main() {

	var student1 = Student(); // TODO One Object, student1 is reference variable
	student1.id = 23;
	student1.name = "Gauthy";
	print("${student1.id} and ${student1.name}");

	student1.study();
	student1.sleep();

	var student2 = Student(); // TODO One Object, student2 is reference variable
	student2.id = 45;
	student2.name = "Ram";
	print("${student2.id} and ${student2.name}");
	student2.study();
	student2.sleep();
}

// TODO Defining states(properties) and behavior of a Student
class Student {
	int id = -1; // TODO Instance or Field Variable, default value is -1
	String ? name; // TODO Instance or Field Variable, default value is null

	void study() {
		print("${this.name} is now studying");
	}

	void sleep() {
		print("${this.name} is now sleeping");
	}
}
```

:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)  

## Constructor

- Constructor is a block of code that initializes the newly created object.
- Constructor resembles an instance method in java but it’s not a method as it doesn’t have a return type.
- It is called when an instance of the class is created. 
- At the time of calling constructor, memory for the object is allocated in the memory.
- It calls a default constructor if there is no constructor available in the class.
- __Types__ -> Default, Parameterized, Named and Constant Constructor

__Need to Know__ 

- In the same class we can have multiple named constructor but we cannot have both default constructor and parametrized constructor at the same time.

__Example 1__

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

__Example 2__

```ruby
void main() {

	// TODO Parameterized Constructor

	var student1 = Student(25, "Gauthy"); // TODO One Object, student1 is reference variable
	print("${student1.id} and ${student1.name}");

	student1.study();
	student1.sleep();

	var student2 = Student(45, "Ram"); // TODO One Object, student2 is reference variable
	print("${student2.id} and ${student2.name}");

	student2.study();
	student2.sleep();

	// TODO Named Constructor
  
	var student3 = Student.myCustomConstructor(); // TODO One object, student3 is a reference variable
	student3.id = 54;
	student3.name = "Rahul";
	print("${student3.id} and ${student3.name}");


	var student4 = Student.myAnotherNamedConstructor(87, "Balu");
	print("${student4.id} and ${student4.name}");
}

// TODO Define states (properties) and behavior of a Student

class Student {

	int id = -1;
	String ? name;

	// TODO Parameterized Constructor 
	//   Student(id, name){
	//     this.id = id;
	//     this.name = name;
	//   }

	// TODO - Code Optimization
	Student(this.id, this.name);

	// TODO Named Constructor
	Student.myCustomConstructor() {
		print("This is my custom constructor");
	}

	// TODO Named Constructor with parameter
	Student.myAnotherNamedConstructor(this.id, this.name);

	void study() {
		print("${this.name} is now studying");
	}

	void sleep() {
		print("${this.name} is now sleeping");
	}
}
```
:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)  

## Inheritance

- Inheritance is the process by which objects of one class acquire the properties & methods of another class. 
- Types - Single Inheritance, Multilevel Inheritance and Hierarchical Inheritance.
- It provides code reusability. 
- It provides the mechanism of Method Overriding (i.e.) It is used to achieve runtime polymorphism.

__Need to Know__

- All the super class are inherited from the class of Object.
- It provides few implementation like toString() -> returns string representation of the Object, hashcode -> returns hashcode representation of the Object and operator == -> To compare two objects.

__Example__

```ruby
void main() {

	var dog = Dog();
	dog.breed = "Labrador";
	dog.color = "Black";
	dog.bark();
	dog.eat();

	var cat = Cat();
	cat.color = "White";
	cat.age = 6;
	cat.eat();
	cat.meow();

	var animal = Animal();
	animal.color = "brown";
	animal.eat();
}

class Animal {

	String ? color;

	void eat() {
		print("Eat !!!");
	}
}

class Dog extends Animal { // TODO Dog is Child class or sub class, Animal is super or parent class

	String ? breed;

	void bark() {
		print("Bark !!!");
	}
}

class Cat extends Animal { // TODO Cat is Child class or sub class, Animal is super or parent class

	int ? age;

	void meow() {
		print("Meow !!!");
	}
}
```
:arrow_up: [__Back to Top__](README.md#flutter-interview-questions) 

## Abstraction

- Abstraction is a process of hiding the implementation details and showing only functionality to the user.
- Abstract Classes are partially defined classes which are declared using abstract keywords.
- It can have both abstract and non-abstract methods (method with the body).
- If a class contains partial implementation then we should declare a class as abstract and it cannot be instantiated.

__Example 1__

```ruby
abstract class Shape {
	double area();
}

class Square implements Shape {
	Square({this.side});
	final double side;
	double area() => side * side;
}

void main() {
	final square = Square(side: 10.0);
	print(square.area());
}
```  

__Example 2__

```ruby
void main() {

	// var shape = Shape();  // TODO Error (i.e.) We Cannot instantiate Abstract Class

	var rectangle = Rectangle();
	rectangle.draw();

	var circle = Circle();
	circle.draw();
}


abstract class Shape {

	// TODO we can define yur Instance variable if needed
	int? x;
	int? y;

	// TODO Abstract Method
	void draw();

	void myNormalFunction() {
		print("This is Normal Function.....");
	}
}

class Rectangle extends Shape {

	void draw() {
		print("Drawing Rectangle.....");
	}
}

class Circle extends Shape {

	void draw() {
		print("Drawing Circle.....");
	}
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
- Static Keyword is used for memory management mainly.

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

## List vs Map

- Dart represents arrays in the form of List objects.
- List is simply an ordered group of objects.  

__Example__

```ruby
void main() {
  
  List<String> myList = [
    'List1',
    'List2',
    'List3',
    'List4'
  ];
  
  print(myList[0]);
  print(myList.indexOf('List1'));
    
}
```
- Dart Map is an object that stores data in the form of a key-value pair.
- Each value is associated with its key, and it is used to access its corresponding value.
- Both keys and values can be any type. In Dart Map, each key must be unique, but the same value can occur multiple times.  

__Example__

```rubyMap<String, int> phoneBook = {
  'Android': 99998888,
  'Flutter': 99998888,
  'IOS': 99998888,
};

main(){
  print(phoneBook['Android']);
  
  phoneBook['Android'] = 888888888;
  print(phoneBook['Android']);
  
  print(phoneBook.length);
  
  print(phoneBook.keys);
  
  print(phoneBook.values);
}
```  
:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)  

## Generics

- Generics are a way to improve type safety in our application (i.e.) We can use them to write code that is safer.

```ruby
void main() {
  
  var mPrimeNumbers = List<int>();
  mPrimeNumbers.addAll([2, 3, 4, 5]);
  mPrimeNumbers.add('Android'); //throws compile time error because of using type annotation  
}
```  
:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)  

## Method Overriding

- If a subclass (child class) has the same method as declared in the parent class, it is known as method overriding in Java.
- The method must have the same name and parameters as in the parent class.
- It is used for runtime polymorphism.

__Example__

```ruby
void main() {

	var dog = Dog();
	dog.eat();

	print(dog.color);
}

class Animal {

	String color = "brown";

	void eat() {
		print("Animal is eating !!!");
	}
}

class Dog extends Animal {

	String ? breed;

	String color = "Black"; // TODO Property Overriding

	void bark() {
		print("Bark !!!");
	}

	// TODO Method Overriding
	void eat() {
		print("Dog is eating !!!");
		super.eat();
		print("More food to eat !!!");
	}
}
```  

:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)


## Interface

- Dart does not have any special syntax to declare interface.
- An Interface in Dart is a normal class.
- An Interface is used when you need concrete implementation of all it's function with in it's sub class.
- It's Mandatory to override all methods in the implementing class.
- We can implement multiple classses but we cannot extend multiple classes during Inheritance.

__Example__

```ruby
void main() {

	var tv = Television();
	tv.volumeUp();
	tv.volumeDown();
}

class Remote {

	void volumeUp() {
		print("+++++++++");
	}

	void volumeDown() {
		print("---------");
	}
}

class AnotherClass {

	void justAnotherMethod() {
		// TODO Code
	}

}

// TODO Here Remote and AnotherClass acts as Interface
class Television implements Remote, AnotherClass {

	void volumeUp() {

		// super.volumeUp(); // TODO Not allowed to call super while implementing a class as Interface
		print("+++++++++");
	}

	void volumeDown() {
		print("---------");
	}

	void justAnotherMethod() {
		print("xxxxxxxxxxxxxx");
	}
}
```  

:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)

## Static Keyword

- It is a Non Access Modifier applicable for Variables and Methods.
- We don't need to create an instance of a Class to use methods or Variables.
- It is mainly Used for Memory Management.

__Need to Know__

- Static Variables are also known as Class Variables.
- Static Methods are also known as Class Methods.
- Static Variables are lazily Initialized (i.e.) they are not initialized until we used in our code.
- We can't able to use the 'this' keyword with in a Static Method.
- From a Static method We can only access static methods and Variables.

__Example__

```ruby
void main() {

	var circle1 = Circle();
	//	circle1.pi; // TODO consumes 4 bytes

	var circle2 = Circle();
	//	circle2.pi; // TODO consumes 4 bytes

	// TODO So Totally 8 bytes(i.e.)Waste of extra 4 bytes

	Circle.pi; // TODO 4 bytes
	Circle.pi; // TOD ONo more memory will be allocated .

	//	circle.calculateArea();
	print(Circle.pi); // TODO Syntax to call Static Variable
	Circle.calculateArea(); // TODO Syntax to call Static Method
}

class Circle {

	static
	const double pi = 3.15;
	static int maxRadius = 5;

	String ? color;

	static void calculateArea() {
		print("Some code to calculate area of Circle");
		// myNormalFunction(); // TODO Not allowed to call instance functions
		// this.color;         // TODO You cannot use 'this' keyword and even cannot access Instance variables
	}

	void myNormalFunction() {
		calculateArea();
		this.color = "Red";
		print(pi);
		print(maxRadius);
	}
}
```

:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)

## Lambda Expression

- Lambda Expression is definition of a Function without a name (i.e.) Nameless Function.
- It is also known as anonymous Function or lambda.

__Need to Know__

- A Function in Dart is an Object.

```ruby
void main() {

	// TODO NOTE: A function in Dart is object
	// TODO Defining Lambda: 1st way
	Function addTwoNumbers = (int a, int b) {
		var sum = a + b;
		print(sum);
	};

	var multiplyByFour = (int number) {
		return number * 4;
	};

	// TODO Defining Lambda: 2nd way: Function Expression: Using Short Hand Syntax or FAT Arrow ( '=>' )
	Function addNumbers = (int a, int b) => print(a + b);

	var multiplyFour = (int number) => number * 4;


	// TODO  Calling lambda function
	addTwoNumbers(2, 5);
	print(multiplyByFour(5));

	addNumbers(3, 7);
	print(multiplyFour(10));
}


// TODO Example of Normal function
void addMyNumbers(int a, int b) {

	var sum = a + b;
	print(sum);
}
```  

:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)

## Higher Order Function

- The Function passed as parameter to another function or a Function can return another function or It can do both.

__Example__

```ruby
void main() {

	// TODO Example One: Passing Function to Higher-Order Function
	Function addNumbers = (a, b) => print(a + b);
	someOtherFunction("Hello World", addNumbers);


	// TODO Example Two: Receiving Function from Higher-Order Function
	var myFunc = taskToPerform();
	print(myFunc(10)); // TODO multiplyFour(10) // number * 4 // 10 * 4 // OUTPUT: 40
}



// TODO Example one: Accepts function as parameter
void someOtherFunction(String message, Function myFunction) { // TODO Higher-Order Function

	print(message);
	myFunction(4, 8); // TODO addNumbers(2, 4) // print(a + b); // print(2 + 4) // OUTPUT: 6
}


// TODO Example two: Returns a function
Function taskToPerform() { // TODO Higher-Order Function

	Function multiplyFour = (int number) => number * 6;
	return multiplyFour;
}
```  

:arrow_up: [__Back to Top__](README.md#flutter-interview-questions)
