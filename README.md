import 'package:flutter/material.dart';
void main() => runApp(MyApp());
class MyApp extends StatelessWidget {
 @override
 Widget build(BuildContext context) {
 return MaterialApp(
 home: CardDemo(),
 );
 }
}
class CardDemo extends StatelessWidget {
 @override
 Widget build(BuildContext context) {
 return Scaffold(
 appBar: AppBar(title: Text('Card Widget Example')),
 body: Center(
 child: Card(
 elevation: 5, // Adds shadow to the card
 shape: RoundedRectangleBorder(
 borderRadius: BorderRadius.circular(15), // Rounded corners
 ),
 child: Padding(
 padding: const EdgeInsets.all(16.0),
 child: Column(
 mainAxisSize: MainAxisSize.min,
 children: <Widget>[
 Text(
 'Flutter Card View',
 style: TextStyle(fontSize: 24, fontWeight: 
FontWeight.bold),
 ),
 SizedBox(height: 10),
 Text(
 'This is a simple card view using Flutter\'s Card 
widget.',
 style: TextStyle(fontSize: 16),
 textAlign: TextAlign.center,
 ),
 ],
 ),
 ),
 ),
 ),
 );
 }
 }
