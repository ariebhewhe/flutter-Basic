
# Note : 
fungsi runApp() digunakan untuk menjalankan dan menampilkan UI ( kumpulan widget material design yg telah terbungkus) ke layar. 
Textderection : menentukan arah text.  ltr ( left to right) , rtl (right to left).
center : komponen yang berperan  sebagai kontainer untuk menempatkan daftar komponen lain dan menampilkan di tengah layar.

# Create Flutter 
<pre> Flutter create  hello1 </pre> 
# Hapus test 
<pre> widget_test.dart pada folder test </pre>
# hapus content main.dart pada folder <b> lib </b> 
tulis script dibawah ini:
 <pre>
 import 'package:flutter/material.dart;
 void main(){
 runApp(
    Center(
    child: Text(
      'hello world!',
      textDirection: TextDirection.ltr,
    )
    
    );
 )
 </pre>
 
# Flutter Run
<pre> flutter run </pre>


