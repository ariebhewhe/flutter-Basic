# note : 
skript diatas adalah untuk mengatur warna latar belakang layar dengan bantuan komponen color dari kelas material. 

# Buat app dengan nama hello6
<pre> Flutter create hello6 </pre>
# ketik koding dibawah ini : 
- untuk run app 
<pre>
void main() => runApp(HelloApp());

class HelloApp extends StatelessWidget {
  @override
  Widget  build(BuildContext context){
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
- untuk homepage
<pre>

class HomePage extends StatelessWidget {
  @override 
  Widget build(BuildContext context){
    return Scaffold(
      appBar: AppBar(
        title: Text('Demo Flutter'),
      ),
      body:  Material(
        color: Colors.blueAccent,
        child: Center(
          child: Text(
            'Hello World',
            textDirection: TextDirection.ltr,
            style: TextStyle( 
              fontSize : 45.0,
              fontStyle : FontStyle.italic,
              color : Colors.white
            )
          ),
        ),
      ),
    );
  }
}
</pre>

