# Condições
As condições são exatamente isso, condições para que determinado código seja executado. São elas que selecionam o que vai acontecer e o que não dentro do nosso programa.

## If (Se)
Traduzindo a palavra `if` do inglês temos o equivalente a *se* no português. Quando digo "Se você colocar a blusa preta vai parecer mais magro.", estou indicando uma condição para você parecer mais magro.

Dessa forma, se eu tenho um bloco de código depois da expressão `if` ele só será executado se as condições indicadas após o `if` forem verdadeiras. Assim:
```
>>> ten = 10
>>> if ten == 10:
>>>     print("Dez é igual a dez.")
Dez é igual a dez.
```
Repare que eu utilizei o operador lógico `==` para comparar se o valor da variável `ten` é igual a `10`. A resposta me retornou `True`, isto é, a comparação confirmou que dez é igual a dez, então o meu código pôde ser executado.

Preste atenção também que, logo após a expressão do `if` eu dei um certo espaço antes de voltar a digitar meu código. Isso é chamado **indentação**, um recuo antes do código para diferenciar um bloco de códigos de outro. Isso é bom quando eu tenho mais código depois do `if`, assim eu posso separar o que eu quero que seja executado sempre e o que eu quero que seja executado só quando o `if` for verdadeiro.

A identação em Python tem o valor (não obrigatório, mas de senso comum e da PEP-8) de 4 espaços.
```
>>> ten = 10
>>> one = 1
>>> if ten and one:
>>>     print("Os valores existem.")
Os valores existem.
```

Da mesma forma funcionam os operadores lógicos. Lembre-se que o `and` só retorna `True` quando ambos os valores forem verdadeiros. Então meu `if` só executará meu código se os valores que passei forem verdadeiros, nesse caso se eles existirem.

E é possível não existirem? Sim! Existe outro tipo Python, o `None`, para esse tipo de valor.
```
>>> vazio = None
>>> teste = "teste"
>>> if teste and vazio:
>>>     print("Ops!")
```
Se executar esse código não tera resultado algum, porque a comparação do `if` retornou `False`.

## Else (Se não)
O `else` é um operador usado sempre em conjunto com o `if` e significa *"se não"*. É como dizer "Se você colocar a blusa preta vai parecer mais magro, se não vai parecer robusto.". Nesta condição, se fizer algo terá um resultado, se não fizer terá um resultado diferente.
```
>>> ten = 10
>>> if ten != 10:
>>>      print("Dez é diferente de dez.")
>>> else:
>>>     print("Dez é igual a dez.")
Dez é igual a dez.
```

Vamos traduzir isso para uma frase: "Se `ten` for diferente de `10`, então imprima 'Dez é diferente de dez.' na tela, se não, imprima 'Dez é igual a dez.' na tela.".

Claro que dez não é diferente de dez! Então meu `if` retornou `False`, logo eu recorri ao `else`. Sempre que meu `if` for `False` o `else` será executado.

Perceba que, neste caso, o `else` está alinhado com o `if` e não com o bloco de código dentro dele, pois é uma condicional diferente e deve ser executado somente se o `if` for `False`.

## Elif (else if)
Quando eu digo "Se você colocar a blusa preta vai parecer mais magro, se colocar a blusa justa vai parecer mais forte, se não vai parecer mais robusto." tenho mais de uma condição diferente para você. Para esse tipo de caso, utilizamos o `elif`, indicando que temos mais de uma condição para verificar antes de executar o `else`. Veja só:
```
>>> blusa = "justa"
>>> if blusa == "preta":
>>>     print("Pareço mais magro.")
>>> elif blusa == "justa":
>>>     print("Pareço mais forte.")
>>> else:
>>>     print("Pareço mais robusto.")
Pareço mais forte.
```

O caminho que percorremos nesse caso foi:
1. Comparar se a variável `blusa` é igual a `"preta"`.
2. A comparação deu `False`, então não vamos executar o que está dentro do bloco de código do `if`.
3. Comparar se a variável `blusa` é igual a `"justa"`.
4. A comparação resultou em `True`, então executamos o bloco de código dentro do `elif` e ignoramos o `else`.

Podemos ter quantas condições desejarmos, alinhando um `elif` após outro. Faça o teste!