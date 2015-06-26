# Listas
Uma lista é um conjunto de valores separados por vírgula e é bastante versátil.
```
>>> lista1 = [1, 5, 10, 15]
```

Assim como as string, cada item de uma lista tem uma posição começando em 0 e toda lista pode ser fatiada. Portanto, eles podem ser retornados por:
```
>>> lista1[2]
10
>>> len(lista1)
4
```
**Obs:** `len()` é uma função que indica o tamanho daquilo que está dentro de seus parênteses. No caso, nossa lista tem 4 elementos, portanto seu tamanho é 4.

# Tuplas
Tuplas são semelhantes às listas, uma sequência de valores separados por vírgulas e definidas entre parênteses. Porém, sua maior diferença reside no fato de que é imutável, ainda assim pode conter objetos mutáveis dentro dela, como uma lista.
```
>>> t1 = (123, 'teste', 123)
```

## Métodos
Os principais métodos das listas e tuplas são aqueles utilizados para realizar alguma ação com seus valores. Segue uma lista:
1. `append(x)` - adiciona o elemento x ao final da lista;
2. `pop(x)` - remove e retorna o valor do elemento que estiver no índice x;
3. `index(x)` - retorna o menor índice do elemento x;
4. `count(x)` - conta quantas vezes x se repete na lista;
5. `sort()` - ordena a lista;
6. `clear()` - remove todos os elementos da lista;
7. `remove(x)` - remove o primeiro elemento cujo valor é x encontrado na lista;

# Sets
É uma lista definida entre chaves, a qual representa um conjunto sem elementos repetidos. Enquanto uma tupla, por exemplo, pode ter dois elementos iguais, um set não terá.
```
>>> s1 = {111, 123, 12, 111}
>>> print(s1)
{111, 123, 12}
```