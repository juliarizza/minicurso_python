# Classes
Agora os conceitos de Orientação a Objeto serão realmente aplicados. Vamos começar definindo o nosso molde de um carro, e, por isso, vamos chamá-lo de classe. Portanto, uma classe nada mais é que o molde de um objeto.
```
>>> class Carro:
>>>     def __init__(self):
>>>         self.cor = "Preto"
>>>         self.quatidade_de_lugares = 7
>>>         self.velocidade_maxima = 200
>>>         self.ligado = False
>>>         self.marcha = 1
>>>         self.velocidade = 0
```

A instrução `class` cria uma nova classe e é seguida pelo nome que queremos dar a ela. A primeira coisa que fazemos é criar um novo método (uma função específica da classe) e esse método é o `__init__`. Esse é um método especial chamado de construtor e é executado sempre que um novo objeto da classe é criado, para construir esse objeto. Ele recebe `self` (si mesmo) como parâmetro, isto é, faz uma referência ao objeto em si.
```
>>> carro = Carro()
```
O que acabamos de fazer foi criar um novo objeto e dizer que esse objeto será igual a um `Carro`, isto é, terá as mesmas características e ações que nossa classe `Carro` tem.

Podemos modificar os atributos do nosso novo carro:
```
>>> carro.cor = "Vermelho"
>>> carro.velocidade_maxima = 250
```
Agora, nosso objeto tem diferentes atributos, mas a classe continua sendo um molde com os valores que passamos quando a definimos. Note que acessamos os atributos por `objeto.atributo` e essa é a forma padrão de acessá-los. Caso queira verificar o status de um atributo, dê um print do atributo desejado. Por exemplo:
```
>>> print(carro.cor)
```
Vamos adicionar algumas funcionalidades para o nosso carro:
```
>>> class Carro:
>>>     def __init__(self):
>>>         self.cor = "Preto"
>>>         self.quatidade_de_lugares = 7
>>>         self.velocidade_maxima = 200
>>>         self.ligado = False
>>>         self.marcha = 1
>>>         self.velocidade = 0
>>>
>>>     def Ligar(self):
>>>         self.ligado = True
>>>
>>>     def Acelerar(self):
>>>         self.velocidade += 10
>>>
>>>     def Freiar(self):
>>>         self.velocidade -= 10
>>>
>>>     def Trocar_Marcha(self, nova_marcha):
>>>         self.marcha = nova_marcha
>>>
>>>     def Desligar(self):
>>>         self.ligado = False
```
Agora nosso carro tem várias funcionalidades. Note que todos os métodos devem receber `self` para indicar que estamos trabalhando com o objeto em si.

Chamamos o método da mesma forma como verificamos os atributos: indicando o objeto e o método que estamos chamando. Confira abaixo e verifique o status dos atributos a medida que executa os métodos.
Vamos dirigir um pouco:
```
>>> carro.Ligar()
>>> carro.Acelerar()
>>> carro.Trocar_Marcha(2)
>>> carro.Freiar()
>>> carro.Desligar()
```

Veja esse código em: [https://gist.github.com/JuliaRizza/afaf3d66c194300818d6](https://gist.github.com/JuliaRizza/afaf3d66c194300818d6)