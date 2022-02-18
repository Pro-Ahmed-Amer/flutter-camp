# **Flutter Camp " DNA Turkey"**

***

## <u>Flutter #01</u>

1- StatefulWidget

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(const MyApp());
}

class MyApp extends StatefulWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return Container();
  }
}
```

***

2- StatelessWidget

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(const MyApp());
}

class MyApp extends StatelessWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  Widget build(BuildContext context) {
    return Container();
  }
}
```

***

3- Scaffold

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: MyApp(),));
}

class MyApp extends StatefulWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return Scaffold();
  }
}
```


<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p1.png" alt="p1.png">
</p>


***

4- Change Background Color 

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: MyApp(),));
}

class MyApp extends StatefulWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.deepPurpleAccent,
    );
  }
}
```


<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p2.png" alt="p2.png">
</p>


***

5- App Bar

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: MyApp(),));
}

class MyApp extends StatefulWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.black,title: Text("DNA SCHOLARSHIP"),),
    );
  }
}
```

<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p3.png" alt="p3.png">
</p>

***

6- Body and Text

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: MyApp(),));
}

class MyApp extends StatefulWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.black,title: Text("DNA SCHOLARSHIP"),),
      body: Text("Test Text",style: TextStyle(fontSize: 20,color: Colors.deepPurpleAccent),),
    );
  }
}
```


<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p4.png" alt="p4.png">
</p>

***

7- Center

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: MyApp(),));
}

class MyApp extends StatefulWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.black,title: Text("DNA SCHOLARSHIP"),),
      body: Center(
        child: Text("Test Text",style: TextStyle(fontSize: 20,color: Colors.deepPurpleAccent),),
      )
    );
  }
}
```


<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p5.png" alt="p5.png">
</p>

***

8- Container

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: MyApp(),));
}

class MyApp extends StatefulWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.black,title: Text("DNA SCHOLARSHIP"),),
      body: Center(
        child: Container(
          height: 200,
          width: 200,
          color: Colors.amberAccent,
        )
      )
    );
  }
}
```


<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p6.png" alt="p6.png">
</p>

***

9- Container with Border Radius

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: MyApp(),));
}

class MyApp extends StatefulWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.black,title: Text("DNA SCHOLARSHIP"),),
      body: Center(
        child: ClipRRect(
          borderRadius: BorderRadius.all(Radius.circular(50)),
          child: Container(
            height: 200,
            width: 200,
            color: Colors.amberAccent,
          ),
        )
      )
    );
  }
}
```

<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p7.png" alt="p7.png">
</p>

***

10- Child

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: MyApp(),));
}

class MyApp extends StatefulWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.black,title: Text("DNA SCHOLARSHIP"),),
      body: Center(
        child: ClipRRect(
          borderRadius: BorderRadius.all(Radius.circular(50)),
          child: Container(
            height: 200,
            width: 200,
            color: Colors.amberAccent,
            child: Center(
              child: Text("HELLO",style: TextStyle(fontSize: 20,color: Colors.blue),),
            )
          ),
        )
      )
    );
  }
}
```

<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p8.png" alt="p8.png">
</p>

***

11- Icon

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: MyApp(),));
}

class MyApp extends StatefulWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.black,title: Text("DNA SCHOLARSHIP"),),
      body: Center(
        child: ClipRRect(
          borderRadius: BorderRadius.all(Radius.circular(50)),
          child: Container(
            height: 200,
            width: 200,
            color: Colors.amberAccent,
            child: Center(
              child: Icon(Icons.add,size: 50,color: Colors.blue,)
            )
          ),
        )
      )
    );
  }
}
```

<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p9.png" alt="p9.png">
</p>

***

12- Image by Direct Link

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: MyApp(),));
}

class MyApp extends StatefulWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.black,title: Text("DNA SCHOLARSHIP"),),
      body: Center(
        child: ClipRRect(
          borderRadius: BorderRadius.all(Radius.circular(50)),
          child: Container(
            height: 200,
            width: 200,
            color: Colors.amberAccent,
            child: Center(
              child: Image.network("https://w7.pngwing.com/pngs/340/946/png-transparent-avatar-user-computer-icons-software-developer-avatar-child-face-heroes.png")
            )
          ),
        )
      )
    );
  }
}
```


<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p10.png" alt="p10.png">
</p>


***

13- Image from File


<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p-11.jpg" alt="p-11.jpg">
</p>


<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p-12.jpg" alt="p-12.jpg">
</p>

***

14- Column

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: MyApp(),));
}

class MyApp extends StatefulWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.black,title: Text("DNA SCHOLARSHIP"),),
      body: Column(
        children: [
          
          Container(
            height: 100,
            color: Colors.blue,
          ),

          Container(
            height: 100,
            color: Colors.amberAccent,
          ),

          Container(
            height: 100,
            color: Colors.deepPurpleAccent,
          ),

          Container(
            height: 100,
            color: Colors.deepOrange,
          ),

        ],
      )
    );
  }
}
```


<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p-13.png" alt="p-13.png">
</p>

***

16- Row

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: MyApp(),));
}

class MyApp extends StatefulWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.black,title: Text("DNA SCHOLARSHIP"),),
      body: Row(
        children: [

          Container(
            width: 50,
            color: Colors.blue,
          ),

          Container(
            width: 50,
            color: Colors.amberAccent,
          ),

          Container(
            width: 50,
            color: Colors.deepPurpleAccent,
          ),

          Container(
            width: 50,
            color: Colors.deepOrange,
          ),

        ],
      )
    );
  }
}
```


<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p-14.png" alt="p-14.png">
</p>

***

17- Stack

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: MyApp(),));
}

class MyApp extends StatefulWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.black,title: Text("DNA SCHOLARSHIP"),),
      body: Center(
        child: Stack(
          children: [

            Container(
              height: 200,
              width: 200,
              color: Colors.blue,
            ),

            Container(
              height: 150,
              width: 150,
              color: Colors.amberAccent,
            ),

            Container(
              height: 100,
              width: 100,
              color: Colors.deepPurpleAccent,
            ),

            Container(
              height: 50,
              width: 50,
              color: Colors.deepOrange,
            ),

          ],
        ),
      )
    );
  }
}
```


<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p-15.png" alt="p-15.png">
</p>

***

18- Column and Row

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: MyApp(),));
}

class MyApp extends StatefulWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.black,title: Text("DNA SCHOLARSHIP"),),
      body: Column(
        children: [

          Container(
            height: 100,
            color: Colors.blue,
            child: Row(
              children: [
                Text("row1",style: TextStyle(fontSize: 25),),
                Text("row2",style: TextStyle(fontSize: 25),),
                Text("row3",style: TextStyle(fontSize: 25),)
              ],
            ),
          ),

          Container(
            height: 100,
            color: Colors.amberAccent,
            child: Row(
              children: [
                Text("row1",style: TextStyle(fontSize: 25),),
                Text("row2",style: TextStyle(fontSize: 25),),
                Text("row3",style: TextStyle(fontSize: 25),)
              ],
            ),
          ),

          Container(
            height: 100,
            color: Colors.deepPurpleAccent,
            child: Row(
              children: [
                Text("row1",style: TextStyle(fontSize: 25),),
                Text("row2",style: TextStyle(fontSize: 25),),
                Text("row3",style: TextStyle(fontSize: 25),)
              ],
            ),
          ),

          Container(
            height: 100,
            color: Colors.deepOrange,
            child: Row(
              children: [
                Text("row1",style: TextStyle(fontSize: 25),),
                Text("row2",style: TextStyle(fontSize: 25),),
                Text("row3",style: TextStyle(fontSize: 25),)
              ],
            ),
          ),

        ],
      )
    );
  }
}
```


<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p-16.png" alt="p-16.png">
</p>


***

19- Size Box

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: MyApp(),));
}

class MyApp extends StatefulWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(backgroundColor: Colors.black,title: Text("DNA SCHOLARSHIP"),),
      body: Column(
        children: [

          Container(
            height: 100,
            color: Colors.blue,
            child: Row(
              children: [
                Text("row1",style: TextStyle(fontSize: 25),),
                SizedBox(width: 20,),
                Text("row2",style: TextStyle(fontSize: 25),),
                SizedBox(width: 20,),
                Text("row3",style: TextStyle(fontSize: 25),)
              ],
            ),
          ),

          SizedBox(height: 50,),
          Container(
            height: 100,
            color: Colors.amberAccent,
            child: Row(
              children: [
                Text("row1",style: TextStyle(fontSize: 25),),
                SizedBox(width: 20,),
                Text("row2",style: TextStyle(fontSize: 25),),
                SizedBox(width: 20,),
                Text("row3",style: TextStyle(fontSize: 25),)
              ],
            ),
          ),
          SizedBox(height: 50,),
          Container(
            height: 100,
            color: Colors.deepPurpleAccent,
            child: Row(
              children: [
                Text("row1",style: TextStyle(fontSize: 25),),
                SizedBox(width: 20,),
                Text("row2",style: TextStyle(fontSize: 25),),
                SizedBox(width: 20,),
                Text("row3",style: TextStyle(fontSize: 25),)
              ],
            ),
          ),
          SizedBox(height: 50,),
          Container(
            height: 100,
            color: Colors.deepOrange,
            child: Row(
              children: [
                Text("row1",style: TextStyle(fontSize: 25),),
                SizedBox(width: 20,),
                Text("row2",style: TextStyle(fontSize: 25),),
                SizedBox(width: 20,),
                Text("row3",style: TextStyle(fontSize: 25),)
              ],
            ),
          ),

        ],
      )
    );
  }
}
```


<p align="center" width="100%">
    <img width="33%" src="Flutter Camp\p-17.png" alt="p-17.png">
</p>


***

