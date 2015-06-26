# Mensagens de Erro
Sempre que estivermos escrevendo algo errado ou um código com mal funcionamento, o interpretador nos avisa por meio de um erro indicando o arquivo e a linha onde o problema está. Nem sempre a linha é exatamente a mesma de onde se encontra o erro, mas o interpretador sempre indicará onde ocorreu a interrupção da execução do programa.

A maioria dos erros são devido a um erro de digitação ou de coerência do programador, portanto esteja sempre atento! Confira abaixo os erros mais comuns.


## Sintax Error (Erro de Sintaxe)
Acontece quando o interpretador é incapaz de ler o que você escreveu. Provavelmente, são erros de digitação ou dígitos a mais ou esquecidos.  

## Identation Error (Erro de Indentação)
Ocorre sempre que sua indentação está incorretar. Podem ser espaços a mais ou a menos ou mesmo seu bloco de código alinhado de forma errada. 

## Key Error (Erro de Chave)
Ocorre quando tentamos acessar um dicionário usando uma chave que não existe. Provavelmente, sua chave foi escrita de forma errônea e o interpretador não encontrou nenhuma compatível no dicionário. 

## Name Error (Erro de Nome)
Ocorre quando um objeto é chamado antes de ser criado. Por exemplo, chamar uma variável x antes que essa variável tenha sido definida. Pode ser também que tenha escrito o nome da variável de maneira errada, tome cuidado. 

## Value Error (Erro de Valor)
Ocorre quando uma função de conversão é incapaz de executar sua tarefa, por exemplo, a função int() recebe uma string "teste" e é incapaz de converter esse valor em um número inteiro; quando um valor retornado por uma função é inválido; quando procuramos uma string que não existe. 

## Type Error (Erro de Tipo)
Ocorre quando chamamos uma função passando mais parâmetros do que ela realmente deve receber; quando trocamos o tipo de um índice, por exemplo, temos umas lista = ["banana", "maçã", "tomate"]  e tentamos pegar um valor por lista["banana"] porém listas só leem índices que são números inteiros. Dicionários, no entando, leem índices strings. 

## Index Error (Erro de Índice)
Ocorre quando o valor do índice é inválido ou inexistente. Por exemplo, na lista = [1,2,3,4] caso eu pesquise por lista[10] receberei um IndexError porque esse índice não existe.	