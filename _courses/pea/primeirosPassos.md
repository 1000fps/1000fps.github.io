---
layout: classContent
title: "02 - Primeiros Passos"
course: "PeA"
sectionNo: 0
section: "Aulas"
lectureOrder: "0"
lecture: "Python"
itemOrder: "1"
type: "Handout"
---

# Meu primeiro script Python 

Agora que estamos com o Python configurado, vamos criar o nosso primeiro
primeiro programa. 

Abra o Thonny -- Ou seu editor de texto favorito -- e coloque o seguinte código:
 

```python
print("Uhul! Python é muito legal")
```

Feito isso salve o arquivo como `olaPython.py`

![](//TODO)

Agora clique no simbolo de "Tocar/Play" no editor. Se tudo deu certo teremos
algo como na imagem:

![](//TODO)


{:.dica}
Se você gosta de atalhos, podemos utilizar a tecla F5 no teclado para executar
nosso programa também. No Visual Studio Code também funciona.

## Mas o que aconteceu?

Quando pedimos para o Thonny "rodar" nosso script, na verdade estamos pedindo
para que o **Interpretador** Python executa `linha a linha` o que está escrito
em nosso código. No caso é apenas o comando `print` que irá "Imprimir no
terminal" o que quer que tenhamos passado dentro dos parenteses dela.

Temos que tomar MUITO cuidado quando estamos escrevendo nossos códigos em python
pois os espaços em branco tem significado!!! Veja:

```python
print("Uma Linha")
 print("Outra Linha")
print("Ainda outra linha")
```
O Código acima dará erro, pois a segunda linha tem um espaço vazio antes do
comando.


