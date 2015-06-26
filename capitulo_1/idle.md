# IDLE, o Interpretador
Como dito antes, o interpretador da linguagem Python é chamado IDLE (Integrated DeveLopment Environment). Em um primeiro momento, o IDLE é semelhante a uma linha de comando, mas suas funções se extendem além disso. A partir dele, temos acesso a uma interface gráfica que nos permite reproduzir código instantaneamente ou criar arquivos Python para serem executados posteriormente.

## Iniciando o IDLE
Novamente, siga os passos:

### No Windows
1. Menu Iniciar
2. Programas
3. Python 3.x
4. IDLE

### No Linux
Abra o terminal e digite o comando (substituindo o `x` pela sua versão):
```
$ idle-python3.x &
```

### No OS X
Abra o terminal e digite (substituindo o `x` pela sua versão):
```
IDLE3.x &
```

## Primeiros comandos
A linha de comando é indicada pelas setas `>>>` e, como o nome diz, é nela que você deve dar os comandos sobre o que a linguagem deve fazer. Sua primeira tarefa é executar um **print**, o comando para imprimir uma mensagem na tela. O retorno, isto é, o resultado da execução deve sair logo abaixo. Siga o exemplo:
```
>>> print("Hello, World!")
Hello World
```

## Fazendo contas
Além de tudo isso, o interpretador pode funcionar como uma calculadora. A execução de cálculos é simples:
```
>>> 10+5 #adição
15
>>> 20-11 #subtração
9
>>> 2*10 #multiplicação
20
>>> 30/2 #divisão
15
>>> 2**4 #exponenciação
16
>>> 10 % 8 #resto da divisão inteira
2
>>> 120-30+2**3 #múltiplas operações
98
```
**Obs:** o símbolo # indica um comentário e ele não interfere na execução.