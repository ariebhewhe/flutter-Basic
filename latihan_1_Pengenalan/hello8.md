# Note : 
Bagian ini kita membahas tentang pengangan kejadian (event-handling) didalam flutter menggunkan RaisedButton.
- metode Action() : 
metode yang mendifiniskan sendiri dan akan dipanggil pada saat event onpressed terjadi. 

# Buat app hello8 
<pre> flutter create hello8 </pre>
# Ketik kode dibawah ini pada  :
- Main.dart
<pre>
import './HomePage.dart';

void main() => runApp(HelloApp());

class HelloApp extends StatelessWidget {
  @override 
  Widget build(BuildContext context){
    return MaterialApp(
      title: 'Demo FLutter',
      home: HomePage()
    );
  }
  
}
</pre>
- HomePage.dart 
<pre> 
import 'package:flutter/material.dart';
import './HelloButton.dart';
class HomePage extends StatelessWidget {
  @override 
  Widget build(BuildContext context){
    return Scaffold(
      appBar: AppBar(
        title: Text('Demo Flutter'),
      ),
      body: Center(
        child: HelloButton()
      ),
    );
  }
}
</pre>

- HelloButton.dart 
<pre>
class HelloButton extends StatelessWidget {
  @override 
  Widget build(BuildContext context){
    return RaisedButton(
      child: Text('Hello'),
      onPressed: (){
        // aksi yg akan digunakan
        Action(context);
      },
    );
  }

  void Action(BuildContext context){
    var alertDialog = AlertDialog(
      title: Text('Event-Handling'),
      content: Text('Hello World!'),
    );
    showDialog(
      context: context,
      builder: (BuildContext context){
        return alertDialog;
      }
    );
  }

}
</pre>


