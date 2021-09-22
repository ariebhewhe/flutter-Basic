# Buat app dengan nama hello4
<pre> flutter create hello4 </pre>
# Ketik koding dibawah ini 
- Membuat tampilan runn app : 
<pre> 
void main() => runApp(HelloApp());
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
- membuat kelas homepage : 
<pre> 
class HomePage extends StatelessWidget {
  @override
  Widget build(BuildContext context){
    return Scaffold(
      appBar: AppBar(
        title: Text('Demo Flutter'),
      ),
      body:  Center(
        child: Text(
          'Hello World!',
          textDirection : TextDirection.ltr,
          style: TextStyle(
            fontSize:45.0,
            fontStyle: FontStyle.italic,
            color: Colors.red,
          )
        )
      )
    );
  }
}
</pre>
# Note : 
TextStyle : untuk mengatur ukuran, warna, dan format teks pada komponen text
