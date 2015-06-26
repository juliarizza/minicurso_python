# Funções Embutidas em Python
Acompanhe a seguir uma lista das principais funções que estão embutidas na linguagem.

`abs(x)`
Retorna o valor absoluto de um número. O argumento deve ser um inteiro ou um ponto flutuante.

`all(iterável)`
Retorna True se todos os elementos do iterável forem verdadeiros (ou se o iterável não está vazio).

`any(iterável)`
Retorna True se qualquer elemento do iterável for verdadeiro. Se o iterável for vazio, retorna False.

`bin(x)`
Converte um número inteiro em uma string binária. O resultado é uma expressão válida de Python.

`chr(i)`
Retorna uma string representando um caractere ao qual seu código Unicode aponta para o inteiro i. Por exemplo, chr(97) retorna a string 'a'. Isso é o inverso de ord(). A extensão válida do argumento é de 0 a 1,114,111 (0x10FFFF na base 16). ValueError será exibido se i estiver fora desse alcance.

`delattr(objeto, nome)`
Este é semelhante ao setattr(). Os argumentos são um objeto e uma string. A string deve ser o nome de um dos atributos do objeto. A função deleta o atributo nomeado, desde que o objeto aceite isso. Por exemplo, delattr(x, 'foobar') é equivalente a deletar x.foobar.

`enumerate(iterável, inicio=0)`
Retorna um objeto enumerado. iterável deve ser uma sequência, um iterador, ou qualquer outro objeto que suporte iteração. O método __next__() do iterador retornado pelo enumerate() returna uma tupla contendo uma contagem (do inicio que é padrão para 0) e os valores obtidos da iteração através do iterável.

`getattr(objeto, nome[, default])`
Retorna o valor do objeto nomeado por objeto. nome deve ser uma string. Se a string é o nome de um dos atributos do objeto, o resultado é o valor desse atributo. Por exemplo, getattr(x, 'foobar') é equivalente a x.foobar. Se o atributo nomeado não existir, default é retornado caso informado, se não o AttributeError é exibido.

`hasattr(objeto, nome)`
Os argumentos são um objeto e uma string. O resultado é True se a string é o nome de um dos atributos do objeto, False se não for.

`help([objeto])`
Invoca o sistema de ajuda embutido. (Essa função é pretendida para o uso interativo.) Se nenhum argumento for passado, o sistema de ajuda interativo inicia no console do interpretador. Se o argumento é uma string, então a string é vista como o nome de um módulo, função, classe, método, chave, ou tópico da documentação, e a página de ajuda é exibida no console. Se o argumento é qualquer outro tipo de objeto, a página de ajuda do objeto é gerada.

`len(s)`
Retorna o comprimento (o número de itens) de um objeto. O argumento deve ser uma sequência (como uma string, bytes, tupla, lista, ou range) ou uma coleção (como um dicionário, set, ou frozen set).

`max(arg1, arg2, *args[, chave])`
Retorna o maior item de um iterável ou o maior de dois ou mais argumentos.

`min(arg1, arg2, *args[, chave])`
Retorna o menor item de um iterável ou o menor de dois ou mais argumentos.

`open(file, mode='r', buffering=-1, encoding=None, errors=None, newline=None, closefd=True, opener=None)`
Abre o file (arquivo) e retorna um objeto de arquivo correspondente. Se o arquivo não pode ser aberto, um OSError é exibido. mode é uma string opcional que especifica a forma como o arquivo será aberto. Seu padrão 'r' significa abrir para leitura em modo texto. Outros valores comuns são o 'w' para escrever (editando o arquivo se ele já existe), 'x' para criação exclusiva e 'a' para adicionar (o que em alguns sistemas Unix, significa que todas as escritas serão adicionadas ao fim do arquivo).

`ord(c)`
Dada uma string representando um caractere Unicode, retorna um inteiro representando o código Unicode que aponta para o caractere. Por exemplo, ord('a') retorna o inteiro 97 e ord('\u2020') retorna 8224. Isso é o inverso de chr().

`range(inicio, fim[, passos])`
Ao invés de ser uma função, range é na verdade um tipo de sequência imutável. inicio é o valor onde ela inicia e fim o valor onde termina.

`round(numero[, n])`
Retorna o valor do número de ponto flutuante arredonado para n digitos depois do ponto decimal. Se n for omitido, ele é padrão para zero.

`setattr(objeto, nome, valor)`
Isso é semelhante a getattr(). Os argumentos são um objeto, uma string e um valor arbitrário. A string deve nomear um atributo existente ou novo. A função associa o valor ao atributo, desde que o objeto permita. Por exemplo, setattr(x, 'foobar', 123) é equivalente a x.foobar = 123.

`sorted(iterável[, chave][, revertido])`
Retorna uma nova lista ordenada a partir dos itens de iterável.

`sum(iterável[, inicio])`
Soma o início e os itens de um iterável da esquerda para a direita e retorna o total. inicio é padrão para 0.