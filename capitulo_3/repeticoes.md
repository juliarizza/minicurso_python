# Repetições
Repetições ou laços ou loops funcionam para repetir um determinado código várias vezes, geralmente terminando quando determinada condição é alcançada.

Um jeito de fazer isso é repetindo o mesmo código várias vezes na mão:
```
>>> print(1)
>>> print(2)
>>> print(3)
1
2
3
```

Porém, isso não é recomendável e com certeza não está na lista de boas práticas. Confira abaixo algumas maneiras de fazer isso de forma mais fácil, principalmente quando temos MUITAS repetições (imagina fazer isso 100 vezes?).

## While (Enquanto)
Do inglês, `while` tem o mesmo significado que *enquanto*. É como dizer "Enquanto eu não tiver 10 chocolates, me traga mais um.", ou seja, enquanto a minha vontade (minha condição) não for satisfeita, você vai continuar me trazendo chocolates. De volta à sequência de números:
```
>>> x = 1
>>> while x <= 3:
>>>     print(x)
>>>     x = x+1
1
2
3
```
A repetição `while` vai executar seu bloco de código **enquanto** x for menor ou igual a 3. Então, imprimiremos o valor de x na tela três vezes e incrementaremos seu valor em um ao final de cada execução para que a próxima tenha um valor diferente até a condição ser satisfeita.

O incremento de 1 no valor também pode ser feito de forma mais fácil por:
```
>>> x += 1
```
A operação `+=` fará com que a variável sempre seja incrementada pelo valor indicado em seguida.

A repetição também pode ser interrompida antes da condição ser satisfeita através do comando `break`.
```
>>> x = 1
>>> while x < 10:
>>>     print(x)
>>>     if x == 3:
>>>         break
>>>     x += 1
1
2
3
```
Nesse caso, se x for igual a `3`, eu interrompo a repetição, mesmo que a condição indique que ela só iria parar quando alcançasse o valor `10`.


##For (para) in (em)
Tenho um novo comando para você: "Para cada chocolate na caixa, me entregue ele.", então você vai me entregar cada chocolate que está na caixa.
```
>>> lista = [1,2,3]
>>> for numero in lista:
>>>     print(numero)
1
2
3
```
Neste caso, para cada número na lista vamos imprimi-lo na tela.

A repetição `for` também pode ser interrompida com o comando `break` e, neste caso, também pode receber um `else`.
```
>>> lista = [1,2,3]
>>> for numero in lista:
>>>     if numero == 4:
>>>         print("Achei o 4.")
>>>         break
>>> else:
>>>     print("Não encontrei o 4.")
Não encontrei o 4.
```
Agora, o `else` será chamado sempre que o `for` terminar de percorrer a lista e o `break` não for acionado.