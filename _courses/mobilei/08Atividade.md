---
layout: classContent
title: "MaterialApp & Scaffold Basico"
course: "Mobile I"
sectionNo: 0
section: "Aulas"
lectureOrder: "1"
lecture: "Flutter"
itemOrder: "8"
type: "Handout"
---

Na ultima aula, vimos com utilizar os widgets MaterialApp e Scaffold:

O primeiro é responsavel por carregar as confifurações e estilos padrão do
"MaterialApp". 

```dart
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Primeiro Statefull',
      home: const MinhaHome(),
    );
  }
```

Ele tem por parametros o título, que é uma string `title: 'Primeiro Statefull'`,
e o parâmetro home, que deve ser o Widget principal de nossa aplicação. 

O Scaffold, é um componente que pode ter uma série de elementos, comuns
utilizados em diversos aplicativos. 

O Uso básico dele seria com um Cabeçalho, que é um AppBar, e um "corpo" que é o
body. 

```dart
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text("Título"),
      ),
      body: Center(
        child: Text("Corpo do App"), 
          
      ),
    );
  }
```


![](img/800.png)

Na imagem parte selecionada em vermelho é o Componente AppBar, e a parte em
verde é o Componente body.

Atenção, que o parametro appBar do Scafold tem que ser um AppBar ou Algo que
herde de AppBar.


O Scaffold tem ainda uma série de outros parâmetros, que são elementos que
compoem nosso layout, vamos ver mais um que é o BottomNavigationBar


```dart
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text("Título"),
      ),
      body: Center(
        child: Text("Corpo do App"), 
          
      ),
      bottomNavigationBar: BottomAppBar(
        color: Colors.red,
        child: Container(height: 50,
            child:Center(child: Text("Bottom App Bar"))
            )
      )
    );
  }
```


![](img/801.png)

Por enquando o código completo dessa app ficou assim: 

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(const MyApp());
}

class MyApp extends StatelessWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Primeiro Statefull',
      home: const MinhaHome(),
    );
  }
}

class MinhaHome extends StatelessWidget{
    const MinhaHome({Key? key}) : super(key: key);

    @override
    Widget build(BuildContext context) {
        return Scaffold(
            appBar: AppBar(
                title: Text("Título"),
            ),
        body: Center(
            child: Text("Corpo do App"), 
        ),
        bottomNavigationBar: BottomAppBar(
            color: Colors.red,
            child: Container(height: 50,
                child: Center(child: Text("Bottom App Bar"))
            )
        ));
    }
}
```
