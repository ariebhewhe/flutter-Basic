# Note : 
Aplikasi di atas hanya untuk memisahkan file dari main.dart sehingga memudahkan anda untuk mengubah tampilan.

# Buat app hello7
<pre> flutter create hello7 </pre>
# Buat kode pada main.dart 
<pre>
// import file homepage.dart
import './homepage.dart';
void main() => runApp(HelloApp());

class HelloApp extends StatelessWidget {
  @override 
  Widget build(BuildContext context){
    return MaterialApp(
      title: 'Hello',
      theme: ThemeData(
        primarySwatch: Colors.blue
      ),
      home: HomePage()
    );
  }
}
</pre>
# Buat kode  homepage.dart 
letakan filenya di dalam folder lib. 
<pre>
import 'package:flutter/material.dart';

class HomePage extends StatelessWidget {
  @override 
  Widget build(BuildContext context){
    return Scaffold(
      appBar: AppBar(
        title: Text(
          'Demo FLutter'
        ),
      ),
      body: Material(
        color: Colors.blueAccent,
        child:  Center(
          child: Text(
            'Hello World',
            textDirection: TextDirection.ltr,
            style: TextStyle( 
              fontSize:45.0,
              fontStyle : FontStyle.italic,
              color:Colors.white
            )
          ),
        ),
      ),
    );
  }
}
</pre>


