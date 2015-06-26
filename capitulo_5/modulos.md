# Módulos

Um módulo é um arquivo contendo código Python. O nome do arquivo é o nome do módulo com o sufixo `.py` adicionado.

As principais bibliotecas de Python são módulos que você pode importar para dentro de seu código, podendo fazer uso de novas funções.

## Import (Importar)
Módulos podem ser importados para dentro de seu código com o comando import, usualmente localizado no início do seu arquivo. Por exemplo:
```
>>> import datetime
```
`datetime` é um módulo que nos fornece diferentes funções para registrar, verificar e receber datas e horários. Agora temos acesso a funções que pertencem ao módulo datetime, como:
```
>>> datetime.datetime.now()
```

Repetimos `datetime` pois primeiro chamamos o módulo e depois o nome de uma classe do módulo que tem o mesmo nome e o método `now()`.

Esse import é semelhante à:
```
>>> from datetime import *
```
Nesse caso, estamos dizendo que queremos importar tudo (simbolizado por `*`) do módulo `datetime`. Portanto, podemos omitir o primeiro `datetime` quando chamarmos o método, pois já especificamos que queremos tudo aquilo que está dentro do módulo, não o módulo em si.
Além disso, podemos fazer:
```
>>> from datetime import datetime
```
Dessa forma, estamos especificando que queremos importar somente a classe `datetime` do módulo `datetime`. Também poderemos omitir o primeiro `datetime` quando chamarmos o método, pois já indicamos que estamos tirando as informações do módulo e não o módulo em si.