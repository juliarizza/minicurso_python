# Herança
Como foi explicado antes, podemos criar um objeto que herde de uma classe. Podemos criar um `Gol` que herde de um `Carro`.
```
>>> class Gol(Carro):
>>>     def __init__(self):
>>>         Carro.__init__(self)
>>>         self.cor = "Prata"
>>>         self.quantidade_de_lugares = 5
>>>         self.ar_condicionado_ligado = False
>>>
>>>     def Ligar_ar_condicionado():
>>>         self.ar_condicionado_ligado = True
>>>
>>>     def Ligar():
>>>         self.ligado = True
>>>         self.marcha = 6
```

Agora, nossa classe `Gol` tem as mesmas características e funcionalidades de um carro, porém modificamos algumas coisas. Primeiro, chamamos o construtor de `Carro` para utilizar os mesmos atributos e métodos da classe e, inclusive, editamos alguns atributos. Depois, adicionamos um novo método: o de ligar o ar condicionado. Por último, reescrevemos a função `Ligar()` do carro e definimos que nosso Gol sempre vai ligar e já mudar para a marcha ré!

```
>>> gol = Gol()
>>> gol.Ligar()
>>> gol.Acelerar()
>>> gol.Desligar()
```
Veja esse código em: [https://gist.github.com/JuliaRizza/afaf3d66c194300818d6](https://gist.github.com/JuliaRizza/afaf3d66c194300818d6)