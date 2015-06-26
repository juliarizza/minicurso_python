# Strings
Uma string é qualquer coisa definida entre aspas. Por exemplo:
```
>>> string1 = "Isso é uma string"
>>> string2 = "10" #não é mais um número, mas sim uma string
```

As aspas podem ser simples (' ') ou duplas (" "). A única exigência é que, caso use aspas dentro de uma string, elas devem ser diferentes daquelas que iniciaram a string.
```
>>> print("Isso é uma citação: 'Citação'.")
Isso é uma citação: 'Citação'.
```

Apesar disso, o caractere \ pode escapar símbolos, isto é, quando usado antes de um símbolo, ele será lido como parte da string, não como parte do código.
```
>>> print('It\'s friday!')
It's friday!
```

Strings que ocupam múltiplas linhas podem ser definidas com aspas triplas:
```
>>> string_grande = """vamos fazer um teste
                       esse é um teste"""
```

## Formatação de Strings
Strings podem ser *fatiadas*. Por exemplo, `Python` tem 6 letras. Porém, começamos a contar do 0. Então `P` é a letra 0, `y` a letra 1, `t` a letra 2 e assim por diante. Dessa forma, podemos pegar um pedaço da string apenas indicando em qual caracter começar e qual terminar:
```
>>> teste = "Python"
>>> teste[0:3] #indicando 3 ele só vai fatiar até a letra de posição 2
'Pyt'
>>> teste[3] #irá buscar somente pela letra na posição 3
'h'
>>> teste[-1] #o sinal negativo indica que irá na ordem inversa
'n'
>>> teste[0:6:2]
'Pto' #escreve de 2 em 2 letras
```

Existe também um recurso conhecido como operador %, que serve para formatar as strings. Basicamente, são três os tipos de formatação que temos:
1. %s - serve para substituir string;
2. %d - serve para substituir números inteiros em uma frase destinada a um print;
3. %f - serve para substituir floats (números em aritmética de ponto flutuante).

As três formatações acima relacionadas são usadas normalmente para aplicações em uma frase destinada a um print.
```
>>> compra= 'maçã'
>>> tipo='verde'
>>> quilos = 1.5
>>> print('Maria comprou %f quilos de %s %s.' % (quilos,compra,tipo))
Maria comprou 1.5 quilos de maçã verde.
```

Como vimos acima o operador % pode ser utilizado para formatação de números também. Com ele é possível também determinar a quantidade de números após a vírgula de um float.
```
>>> num=245.47876749
>>> print('%.2f' % (num))
245.48
```
Percebemos que Python fez uma aproximação do número real, possibilitando que o resultado de uma futura operação seja o mais preciso possível.

Ainda que essa formatação seja a mais comum, as strings Python possuem um método específico para formatação que evita muitas dores de cabeça e ainda deixa mais explícito o que você está exibindo em cada local. 
```
>>> compra= 'maçã'
>>> tipo='verde'
>>> quilos = 1.5
>>> "Maria comprou {peso} quilos de {produto} {tipo}.".format(peso=quilos, produto=compra, tipo=tipo)
Maria comprou 1.5 quilos de maçã verde.
```

## Manipulação de Strings
Pelo fato de uma string ser uma sequência imutável, isso nos dá a possibilidade de manipularmos essa sequência.
```
>>> a = 'matemática'
>>> a[2]+a[-5]+a[-4:]
>>> 'tática'
```
As operações matemáticas, nesse caso, podem ser utilizadas para concatenar strings.
```
>>> b = "bla"
>>> 10*b
'blablablablablablablablablabla'
```

## Métodos
Assim como a maioria dos outros tipos básicos, as strings possuem métodos. Métodos são funções inclusas dentro de um tipo de dado, que vão valer para qualquer valor desse tipo. Os métodos são chamados da seguinte forma `.nome_metodo(argumentos)`. A função **format()**, vista anteriormente, é um método das strings.

Segue uma lista dos mais comuns:
1. `capitalize()` - retorna uma cópia da string com o primeiro caractere maiúsculo;
2. `lower()` - retorna uma cópia da string com todos os caracteres em minúsculo;
3. `upper()` - retorna uma cópia da string com todos os caracteres em maiúsculo;
4. `endswith(texto)` - retorna um valor True ou False avisando se a string termina com aquele caractere ou pedaço de texto informado;
5. `startswith(texto)` - o mesmo do `endswith()`, porém verificando no início da string;
6. `find(texto)` - retorna o menor índice onde o valor de texto passado pode ser encontrado dentro da string;
7. `split(separador)` - retorna uma lista das palavras da string quando separamos elas pelo separador informado;