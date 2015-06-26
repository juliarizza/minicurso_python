# Tipos Básicos

Vamos entender um pouco melhor a parte teórica de Python. A documentação completa pode ser encontrada pode ser encontrada no [site oficial](http://python.org) (http://python.org).

## Variáveis: o que são, como comem, onde dormem, quem são elas?
Eu gosto muito da explicação de que a variável é uma etiqueta e o valor é uma caixa.
Você precisa identificar uma caixa, então vai colar nela uma etiqueta com uma identificação. Logo, sempre que você precisar daquele valor, vai procurar pela etiqueta que identifica ele.
```
>>> ten = 10
>>> print(ten)
10
```
Se você precisa que aquela identificação seja de outra caixa, pode tirar a etiqueta de uma e colocar em outra. Da mesma forma, a variável pode mudar de valor.
```
>>> ten = 10
>>> ten = 42
>>> print(ten)
42
```
`ten` é a variável e `42` é o seu valor. Sempre que eu "chamar" a variável `ten`, ela vai me informar seu valor.
O nome de uma variável apenas não pode conter espaços em branco, começar com números ou ser uma palavra reservada (palavras que já são utilizadas em algum lugar dentro da linguagem, ex: not, return, class, else, etc).

Ao contrário da maioria das outras linguagens, em Python, não é necessário declarar as variáveis que serão usadas, tampouco definir seu tipo. A própria sintaxe do dado a ser armazenado identica o tipo da variável para armazená-lo. Por exemplo, caso deseje-se atribuir o valor `3` à variável `A`, basta digitar `A=3`. Python saberá que `A` é um número inteiro. Por outro lado, se o valor a ser armazenado fosse `3,2` que é um dado do tipo "ponto flutuante", este deveria ser expresso como `A=3.2`.