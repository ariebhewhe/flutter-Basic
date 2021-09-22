# Note : 
contoh diatas saya akan menggunakan <b>textstyle</b>. untuk keperluan diatas silakan ambil font pada 
link website <a href="http://fonts.google.com"> http://fonts.google.com </a> dan donwload font extra ke dalam folder fonts 
( jk belum ada silakan buat folder dahulu ). 

# Buat App hello5
<pre> flutter create hello5 </pre>
# ketik script dibawah ini : 

- untuk runnApp / tampilan (step 1)
<pre>
void main () => runApp(HelloApp());
class HelloApp extends StatelessWidget {
  @override
  Widget build(BuildContext context){
    return MaterialApp(
      title: 'Hello',
      theme: ThemeData(
        primarySwatch: Colors.blue,
      ),
      home: HomePage()
    );
  }
}
</pre>

- untuk homepage  (step 2): 
<pre>

class HomePage extends StatelessWidget {
  @override 
  Widget build(BuildContext context){
    return Scaffold(
      appBar: AppBar(
        title:  Text('Demo FLutter',
         style: TextStyle(
        decoration: TextDecoration.none,
        fontFamily: 'MarckScript'
      )
        ),
      ),
  body: Center(
    child: Text(
      'Hello World!',
      textDirection: TextDirection.ltr,
      style: TextStyle(
        fontSize: 45.0,
        decoration: TextDecoration.none,
        fontFamily: 'MarckScript',
        fontWeight: FontWeight.w400,
      )
    ),
  ),
    );
  }
  
}
</pre>

# Tambahkan settingan pubspec.yaml
<pre>
fonts:
    - family: MarckScript
      fonts:
        - asset: fonts/MarckScript-Regular.ttf
          weight: 400

</pre>

