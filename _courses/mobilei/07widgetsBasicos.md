---
layout: classContent
title: "Primeiro projeto minimo"
course: "Mobile I"
sectionNo: 0
section: "Aulas"
lectureOrder: "1"
lecture: "Flutter"
itemOrder: "2"
type: "Handout"
---


#  Widgets básicos. 

Agora que já sabemos criar nossa clase base para uma aplicação flutter, vamos
ver os elementos básicos que iremos usar muito ao longo de nossa trajetorioa com
o flutter.

## Texto (*Text Widget*)

Claramente será bastante comum apresentarmos texto para o usuário, e para isso
utilizamos este widget. 

```dart
Text("Meu texto", textDirection : TextDirection.ltr);
```

O código acima é a forma mais "crua" de se criar um texto, e o colocando como
filho (child) de um containter ele irá ficar como na imagem

![](img/textWidget01.png)

Mas esse elemento tem diversas opções para que possamos deixar as coisas mais
interessantes. 

### Overflow

Utilizamos essa opção quando queremos indicar o que deve acontecer se um texto
for muito grande para seu espaço: 

`TextOverflow.clip`

![](img/textWidget02.png)

Essa opção corta o texto que não cabe no seu espaço.


`TextOverflow.elipsis`

![](img/textWidget03.png)

Essa opção coloca o sinal de reticências (...) depois da quebra do texto.


`TextOverflow.fade`

![](img/textWidget04.png)

Essa opção faz uma transição para o texto ir ficando transparente


`TextOverflow.visible`

![](img/textWidget05.png)

Finalmente, esta mantem o texto sendo mostrado mesmo que fora de seu espaço.


```dart
Text("Meu texto", 
     textDirection: TextDirection.ltr,
     overflow: TextOverflow.ellipsis
     );
```

{:.dica}
Percebeu que em algumas oções o texto "quebrou linha" antes de aplicar o
overflow? podemos utilizar a opção `maxLines` para definir um número maximo de
linhas que queremos que isso aconteça.

```dart
Text("Meu texto",
     textDirection: TextDirecrion.ltr,
     overflow: TextOverdlow.ellipsis,
     maxLines: 1
     );
```

### TextAlign

Ess opção cuida de como o texto ficará alinhado horizontalmente

`TextAlign.center` &nbsp; `TextAlign.end` &nbsp; `TextAlign.justify`

`TextAlign.left` &nbsp; `TextAlign.rigt` &nbsp; `TextAlign.start`

```dart
Text("Meu texto",
     textDirection: TextDirecrion.ltr,
     overflow: TextOverdlow.ellipsis,
     maxLines: 1,
     textAlign: TextAlign.center
     );
```

