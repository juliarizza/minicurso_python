# Funções
Funções são aqueles nomes que usamos para realizar alguma ação em nosso código. Por exemplo, quando utilizamos `input()` em nosso programa, estávamos utilizando a função `input()` para solicitar uma informação do usuário. Podemos, também, criar nossas próprias funções.

A definição de uma função é dada pela instrução `def` seguida do nome da função. Logo depois, especificamos dentro de parênteses os parâmetros que a função deve receber.
```
>>> def subtrai(num1, num2):
>>>     print(num1-num2)
```
Nesse caso, a função `subtrai` recebe um parâmetro chamado `num1` e um parâmetro chamado `num2`. Logo, estamos deixando claro que o usuário, quando chamar a função `subtrai`, deve informar dois parâmetros.

Em seguida, definimos que essa função deve executar uma subtração entre `num1` e `num2` e imprimir o resultado na tela.

Uma função não é executada assim que definida, mas somente quando é chamada. Para chamar uma função fazemos:
```
>>> subtrai(10, 4)
6
```

Ou seja, chamamos a função pelo nome que demos a ela e passamos os parâmetros que ela requer. Porém, nem sempre queremos imprimir o resultado da nossa função da tela.
```
>>> def subtrai(num1, num2):
>>>     return(num1-num2)
```
Realizar a subtração e imprimir a subtração na tela são duas coisas diferentes. Logo, podemos suprimir o print e deixar a função realizar o cálculo apenas. Usando `return`, podemos informar o resultado da função sem precisar imprimi-lo na tela.

A função também pode não ter parâmetros ou ter parâmetros opcionais. Nesse caso, daremos um valor padrão para o parâmetro. Assim, se o usuário não informar um valor para o parâmetro, usaremos seu valor padrão.
```
>>> def repetir(qtd, caractere='a'):
>>>     return(qtd*caractere)
>>> repetir(10)
'aaaaaaaaaa'

>>> repetir(20, '*')
'********************'
```

Inclusive, parâmetros podem ser especificados na chamada da função, mesmo quando são obrigatórios. Caso não sejam nomeados, devem seguir a ordem na qual foram definidos.
```
>>> repetir(qtd=20, caractere='*')
'********************'
```


