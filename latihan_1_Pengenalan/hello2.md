# note : 
case ke 2 ini untuk menghandle masalah tampilan. Hasilanya sama dengan hello 1. semua kelas turunan dari <b> StatelessWidget </b> 
perlu dibuat <b> @override </b> terhadap metode build(). dengan cara ini kita dapat mengembangkan aplikasi.

# Buat app hello 2
<pre> flutter create hello2  </pre>
# ketik program dibawah ini : 
<pre>
import 'package:flutter/material.dart';

void main() =>runApp(HelloApp());

class HelloApp extends StatelessWidget {
   @override
   Widget build(BuildContext context){
     return Center(
       child: Text('Hello World!',
       textDirection: TextDirection.ltr),
     );
     
}
</pre>
