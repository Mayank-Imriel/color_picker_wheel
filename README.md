# color_picker_wheel

A simple color picker to select color from given range of colors and set its shade more darker or lighter

## Screenshot
<img rc="ss1.png" height = "300em" />
## Getting Started

To use this plugin :

* add the dependency to your [pubspec.yaml] file.

```yaml
  dependencies:
    flutter:
      sdk: flutter
    color_picker_wheel:
```

* In your file add following import.

```import 'package:color_picker_wheel/color_picker_wheel_widget.dart';
```

* Example

```import 'package:color_picker_wheel/color_picker_wheel_widget.dart';
   import 'package:flutter/material.dart';

   void main() {
     runApp(MyApp());
   }

   class MyApp extends StatelessWidget {
     @override
     Widget build(BuildContext context) {
       return MaterialApp(
         title: 'Color Picker Demo',
         theme: ThemeData(
           primarySwatch: Colors.blue,
           visualDensity: VisualDensity.adaptivePlatformDensity,
         ),
         home: Scaffold(
           appBar: AppBar(
             title: Text("Color Picker Demo"),
           ),
           body: SafeArea(
             child: ColorPickerWheel(
               colorListener: (color) {
                 print("Color select :${color.value}");
               },
             ),
           ),
         ),
       );
     }
   }

```

This project is a starting point for a Dart
[package](https://flutter.dev/developing-packages/),
a library module containing code that can be shared easily across
multiple Flutter or Dart projects.

For help getting started with Flutter, view our 
[online documentation](https://flutter.dev/docs), which offers tutorials, 
samples, guidance on mobile development, and a full API reference.
