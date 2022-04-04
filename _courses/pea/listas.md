---
layout: classContent
title: "Listas"
course: "PeA"
sectionNo: 0
section: "Aulas"
lectureOrder: "0"
lecture: "Variáveis Complexas"
itemOrder: "0"
type: "Handout"
---

# Listas


Até agora, em nossos programas só conseguimos salvar uma única informação em uma
variável, e isso já resolve muitos dos desafios que encontramos.
  
Contudo temos ainda diversos problemas que para ser resolvidos é mais interessante
que seja possível guardar várias informações na mesma referência (variável)
 
Para isso utilizamos as listas (lists), que é uma estrutura de dados que podemos
guardar mais de um dado em uma variável só. 

---

## Criando listas

Veja só como criar uma lista em python:



```python
minhaLista = ["a", "b", "c"]
print(minhaLista)
```


> Tente executar o código acima, o que acontece?


Perceba, que cada um dos elementos da lista é separado por uma virgula.

---

## Acessando elementos

Podemos acessar esses elementos individualmente utilizando o índice (ou index em
inglês) desse elemento. Para isso abrimos colchete ( [ ) colocamos o número do 
índice que queremos e fechamos colchete ( ] ). Veja: 



```python
print(minhaLista[1])
```


> Adicione o código acime ao final da execução do código anterior. Aconteceu o 
que você havia previsto? Ou aconteceu alguma coisa diferente?

Os Índices em programação podem ser confusos a primeira vista, mas com experiência
vamos acostumando, no caso do script acima, estamos tentando acessar o **elemento 
de índice 1** de nossa lista, que na realidade é o segundo elemento. 

Isso ocorre por que os índices começam no número 0. 

Então no exemplo de minhaLista o **elemento de índice 0** é o caractere **a**, o
**elemento de índice 1** é o caractere **b**, e assim por diante.

 
## Modificando elementos

Para modificar elementos de uma lista, podemos acessá-lo como acabamos de ver, e
atribuir simplesmente atribuir um novo valor a ele. 


```python
minhaLista[1] = "d"
print(minhaLista)
```


---

## Adicionando novos elementos

Uma das facilidades das listas de python é poder anexar novos elementos ao final
da lista, para isso utilizamos a função append de listas


```python 
minhaLista.append("e") print(minhaLista)
```


---

## Modificando elementos

Para modificar elementos de uma lista, podemos acessá-lo como acabamos de ver, e
atribuir simplesmente atribuir um novo valor a ele. 

```python 
minhaLista[1] = "d" print(minhaLista) 
```

---


---

# Código completo 

```python 
minhaLista = ["a", "b", "c"]

print(minhaLista)

print(minhaLista[1])

minhaLista[1] = "d"

print(minhaLista)

minhaLista.append("e")

print(minhaLista)
```

---


---

# Desafio!

Utilizando tudo que você aprendeu até agora, você consegue criar um script que
percorra uma lista qualquer?


# Exercícios.

1. Crie um script que mostre o maior número de uma lista. 
1. Crie um script que faça a soma de todos os números de uma lista.
1. Crie um script que compare duas listas, e fale se elas são idênticas ou não.
1. Crie um script que conte mostre para o usuário os elementos que são iguais
   entre duas listas.
1. Crie um programa de cadastro de nomes, o programa deverá continuar
   cadastrando nomes até o usuário confirmar que não quer mais cadastrar nomes.
   Depois disso o programa deverá mostrar todos os nomes cadastrados, um por
   linha.


