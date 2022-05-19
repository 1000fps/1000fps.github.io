---
layout: classContent
title: "05 - Op. Lógicos"
course: "PeA"
sectionNo: 0
section: "Aulas"
lectureOrder: "0"
lecture: "Python"
itemOrder: "4"
type: "Handout"
---

Acabamos de ver como usar Operadores de Comparação, e os contrução if..else para
tomar decisões em nosso código. 

```python
if (chovendo == True) :
    print("Levar guarda chuva")
else : 
    print("Dia de sol!")
```

Mas algumas vezes precisamos de uma condição mais complexa, e então utilizamos
os operadores lógicos, que são três: E, OU e NÃO(ou negação)

# E Lógico (AND)
Utilizamos este operador, quando precisamos criar uma expressão, que para ser
verdade duas condições precisam ser verdadeiras.

Por exemplo nota e presença em um curso, para um aluno ser aprovado ele precisa
de presença maior que 75% `E` nota maior que 6.0. Isso em código ficaria assim: 

```python
presenca > 75.0 AND nota > 6.0
```

E utilizando junto com o if: 

```python
if (presenca > 75.0 AND nota > 6.0) :
    print("Aluno Aprovado")
else : 
    print("Aluno Reprovado")
```

o `AND` só vai ser verdadeiro, somente se as duas condições forem verdadeiras,
para melhor visualizar podemos montar a _Tabela Verdade_  desse operador: 

| `AND` | `V` | `F` | 
| :---: | :-: | :-: |
| `V` | V | F |
| `F` | F | F | 

# OU Lógico (OR)
As vezes queremos verificar duas condições, e fazer algo se qualquer uma delas for
verdadeira, para isso usamos o `OR`


E a _Tabela Verdade_ do `OR` fica: 


| `OR` | `V` | `F` | 
| :---: | :-: | :-: |
| `V` | V | V |
| `F` | V | F | 

# Não Lógico (NOT)

Por fim, não é raro termos que inverter uma condição, e para isso utilizamos o
`NOT`. Dos três ele é o unico que não tem duas condições a ser testada, ele
apenas inverte o resultado da que ele foi aplicado.


| `OR` | `V` | `F` | 
| :---: | :-: | :-: |
|  | F | V |

# Outras Tabelas Verdade

| `NOT ( AND )` | `V` | `F` | 
| ---: | :-: | :-: |
| `V` | F | V |
| `F` | V | V | 

| `NOT ( OR )` | `V` | `F` | 
| ---: | :-: | :-: |
| `V` | F | F |
| `F` | F | V | 
