# Dicionários
Dicionários são conjuntos de `chave:valor`. O melhor para entender, é vendo. Dicionários podem ser definidos de duas maneiras:
```
>>> dict1 = dict(nome='fulano', idade=29)
>>> dict2 = {'nome':'fulano', 'idade':29}
>>> print(dict1)
{'idade':29, 'nome':'fulano'}
>>> print(dict2)
{'idade':29, 'nome':'fulano'}
```
A chave é a forma como identificamos o valor. Nesse caso, `nome` e `idade` são chaves e `fulano` e `29` são valores associados a elas.

Um valor dentro de um dicionário pode ser retornado a partir de sua chave. Dessa forma, o dicionário funciona como uma lista onde os índices tem nome, ao invés de serem apenas numerados.
```
>>> print(dict1['nome'])
'fulano'
```

Além disso, você pode adicionar novos valores a um dicionário simplismente informando uma chave que ele ainda não possui e alterar valores associando novos valores a uma chave existente.
```
>>> dict1['altura'] = 1.80
>>> print(dict1['altura'])
1.80
>>> dict2['nome'] = 'ciclano'
>>> print(dict2['nome'])
'ciclano'
```

## Métodos
Os principais métodos dos dicionários são:
1. `clear()` - remove todos os itens do dicionário;
2. `get(x)` - retorna o valor que está associado à chave x dentro do dicionário;
3. `items()` - retorna todos os items dentro do dicionário no formato (chave, valor);
4. `keys()` - retorna todas as chaves do dicionário;
5. `values()` - retorna todos os valores do dicionário;