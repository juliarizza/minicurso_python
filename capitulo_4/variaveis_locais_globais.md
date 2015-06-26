
#Variáveis locais e globais
Quando usamos funções, precisamos nos atentar às variáveis. Variáveis locais existem somente dentro da função onde foram instanciadas, já variáveis globais existem fora da função e podem ser acessadas por todas as funções e módulos. Observe:
```
>>> def multiplica(num1, num2):
>>>     a = num1
>>>     b = num2
>>>     return(a*b)
```
Nesse caso, `a` e `b` são variáveis que só existem dentro da função multiplica. Logo, são variáveis locais.
```
>>> comida = "arroz"
>>> def qual_a_comida():
>>>     print(comida)
>>> qual_a_comida()
>>> print(comida)
```
Aqui, definimos a variável `comida` fora da função, então ela é uma variável global. Logo, podemos acessar a variável `comida` tanto dentro quanto fora da função.
Observe esse exemplo:
```
>>> comida = "arroz"
>>> def muda_comida():
>>>     comida = "batata"
>>>     print("Comida: {nova_comida}".format(nova_comida=comida))
>>> print(comida) #comida antes de mudar
'arroz'
>>> muda_comida() #chamando a função
'Comida: batata'
>>> print(comida) #comida depois da função muda_comida()
'arroz'
```
A `comida` continua sendo `arroz`! Isso acontece porque, para Python, a variável `comida` fora da função e a variável `comida` dentro da função são duas coisas diferentes. Uma é uma variável global e a outra é local. Para alterarmos a variável global ao invés de criarmos uma local dentro da função, devemos avisar que estamos chamando a variável global:
```
>>> comida = "arroz"
>>> def muda_comida():
>>>     global comida #avisando que queremos a variável global
>>>     comida = "batata"
>>>     print("Comida: {nova_comida}".format(nova_comida=comida))
>>> print(comida) #comida antes de mudar
'arroz'
>>> muda_comida() # chamando a função
'Comida: batata'
>>> print(comida) #comida depos da função muda_comida()
'batata'
```