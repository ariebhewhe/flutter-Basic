# Note:
latihan ini kita menggunakan kelas Material App dan Scaffold.  <b>Material App</b> adalah aplikasi yang akan dibuat menggunakan 
library dari material desain. Scaffold adalah komponen yang digunakan untuk membentuk struktur widget di dalam suatu halaman,
misal application bar dan badan halaman.  

# Buat aplikasi hello3
<pre> fluttter create hello3 </pre>
# ketik koding dibawah ini :
- Kode Aplikasi untuk run app:
<pre>
import 'package:flutter/material.dart';
void main() => runApp(HelloApp());

class HelloApp extends StatelessWidget {
   @override
   Widget build(BuildContext context){
     return MaterialApp(
       title: 'Hello',
       theme: ThemeData(
         primarySwatch: Colors.blue,
       ),
       home: HomePage(),
     );
   }
}
</pre>

- Kelas untuk menampilkan halaman utama/homepage:
<pre> 
class HomePage extends StatelessWidget {
  @override
  Widget build (BuildContext context){
    return Scaffold(
      appBar: AppBar(
        title: Text('Demo Hello2')
      ),
      body: Center(
        child: Text('Hello World!',textDirection: TextDirection.ltr,),
        
      ),
    );
  }
}

</pre>

