---
layout: classContent
title: "Variáveis 1"
course: "Mobile I"
sectionNo: 0
section: "Aulas"
lectureOrder: "0"
lecture: "Dart"
itemOrder: "0"
type: "Handout"
---

Antes de começarmos a trabalhar com o flutter, vamos fazer uma revisão básica de
programação utilizando a linguagem **DART**. 


**DART** e uma linguagem *fortemente tipada*, que conta com inferência do tipo
de variáveis. Isso significa que depois de definido o tipo de uma variável não
será possível alterá-lo.  

Bom, mas como definimos uma variável? Basta usar a palavra chave `var` e
atribuir nossa variável. Veja:

```dart
var umaVariavel = "Lorem ipsum dolor sit amet";
```

No caso acima, `umaVariavel` é do tipo `String`, que foi inferido do conteúdo
que foi atribuído. 

Durante nossas aulas, vamos procurar sempre inicializar nossas variáveis. 

# Tipos *Build-in* simples[^1]

Como toda linguagem de programação **DART** tem alguns tipos básicos padrão,
entre eles temos os tipos numéricos, `int` e `double`, temos também o tipos
`String`, que já vimos, e não menos importante `bool`. Basta declarar e
atribuirmos corretamente, que o tipo será inferido. 

```dart
var variavelInt = 42;

var variavelDouble = 3.14;

var variavelString = "Era uma vez...";

var variavelBool = true;
```

Se quisermos, podemos sim utilizar as anotações de tipos para garantir que nossa
variável seja de um tipo específico. Reescrevendo o código acima com anotações
de tipos ficaria como abaixo: 

```dart
int variavelInt = 42;

double variavelDouble = 3.14;

String variavelString = "Era uma vez...";

bool variavelBool = true;
```

### Conversões

Muitas vezes, por diversos motivos, precisamos converter de um tipo para outro,
o **DART** fornece algumas funções bastante uteis para isso. 

```dart
// String para int
var resposta = int.parse("42");

//String para double
var euler = double.parse("2.71828");

//int ou double para String
var resposta_texto = resposta.toString();
var euler_texto = euler.toString();
```

### Interpolação de Strings

É bastante comum que a gente queira colocar uma variável no meio de um texto
para apresentar para o usuário. Para isso **DART** tem a funcionalidade de
_String Interpolation_, em que podemos utilizar o construto `${expressão}` para
inserir variáveis ou expressões mais complexas no meio de nossos textos: 

```dart
var idade = 45;

var saida = "A idade é de ${idade} anos";
```

No exemplo acima, a variável saída conterá a String `"A idade é de 45 anos"`

# Operadores

Agora que já vimos como criar variáveis, vamos relembrar o uso de operadores a
começar pelos operadores matemáticos: 

## Operadores Matemáticos.

| Operador | Nome | Exemplo de uso | Resultado | 
| :------: | :--: | :------------: | :-------: |
| + | Adição | `42 + 58` | 100 | 
| - | Subtração | `42 - 58` | -16 | 
| * | Multiplicação | `42 * 58 ` | 2436 |  
| / | Divisão | `42 / 58` | 0.724... | 
| % | Resto da divisão inteira (mod) | `42 % 12` | 6 | 

Os operadores na tabelas acima funcionam como na matemática, sem maiores
surpresas até aqui. 

## Operadores de atribuição

Além da atribuição simples, que é feita utilizando o sinal de igual (`=`)
podemos juntar com alguns outros operadores:

```dart
var i = 1;
var j = 1.0; 
var k = 1.0; 

i += 1; //2

j -= 1; //0 

i *= 2; //4

k /= 2; //0.5

```


## Operadores Relacionais

Utilizamos os operadores relacionais para criar diversas condições que vamos
testar em nosso código


| Operador | Nome | Exemplo | Resultado | 
| :------: | :--: | :-----: | :-------: |
| == | Igualdade | `"42" == 42` | false | 
| != | Diferente | `"42" == 42` | true | 
| > | Maior que | `42 > 58` | false |
| >= | Maior ou igual a | `42 >= 42` | true | 
| < | Menor que | `42 < 58` | true | 
| <= | Menor ou igual a | `58 <= 42` | false | 

## Operadores Lógicos:

Por fim, mas não menos importante, temos os operadores lógicos, em que podemos
relacionar uma ou duas condições (que podemos definir com os operadores lógicos
por exemplo) para decisões mais complexas. 

### Negação `!expressão`

O operador de negação inverte o resultado de uma condição, veja a tabela dele:

| `!`| true | false | 
| :--: | :--: | :---: |
| &nbsp;&nbsp; | false | true | 

### Ou lógico `||`

O operador ou lógico, será verdadeiro, se pelo menos um dos seus lados sejam
verdadeiros: 

| `||` | true | false | 
| :--: | :--: | :---: |
| true | true | true | 
| false | true | false | 

### E lógico `&&`

Já o operador lógico E, será verdadeiro se AMBAS suas condições forem
verdadeiras.

| `&&` | true | false | 
| :--: | :--: | :---: |
| true | true | false | 
| false | false | false | 

---
# Referências
[^1]: [Documentação DART \(inglês\)](https://dart.dev/guides/language/language-tour#built-in-types)
