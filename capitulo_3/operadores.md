# Operadores Relacionais
São símbolos utilizados para fazer comparações. Confira os operadores relacionais de Python na imagem abaixo:
[Operadores relacionais](http://cdn.dicasdeprogramacao.com.br.s3.amazonaws.com/wp-content/uploads/2013/03/Operadores-relacionais.jpg)

Quando a comparação é realizada utilizando tais operadores, os resultados são booleanos informando se tal comparação é verdadeira ou falsa.
```
>>> 10 > 5
True
>>> 10 < 5
False

>>> a = 10
>>> b = 5
>>> a > b
True
```

# Operadores Lógicos
Dada a lógica binária anteriormente, confira as tabelas verdade. Os operadores **NOT**, **AND** e **OR** são chamados operadores lógicos e nos auxiliam a fazer comparações mais complexas.
```
>>> not True
False
```
Acabei de falar que algo não é verdadeiro, então só pode ser falso. Logo, o resultado é falso.

```
>>> True and True
True
>>> True and False
False
>>> False and True
False
>>> False and False
False
```
Pela tabela verdade do operador `and`, somente quando ambos os valores forem verdadeiros, o resultado será verdadeiro. Do contrário será falso.

```
>>> True or True
True
>>> True or False
True
>>> False or True
True
>>> False or False
False
```
Já com o operador `or`, o resultado será verdadeiro sempre que pelo menos um dos valores for verdadeiro. Somente quando ambos forem falsos, o resultado será falso.