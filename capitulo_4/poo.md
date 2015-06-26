# Orientação a Objetos
Vamos mergulhar mais a fundo dentro da linguagem e ter uma noção melhor da Orientação a Objetos. Primeiro, uma breve introdução a esse conceito:

"A orientação a objetos é um modelo de análise, projeto e programação de sistemas de software baseado na composição e interação entre diversas unidades de software chamadas de objetos." - Wikipedia

Os objetos na programação são como representações de objetos reais. Por isso, podemos resumir a POO em um exemplo simples:

Definimos um objeto `carro` e esse objeto tem **métodos** (ações) e **atributos** (características).

Nesse caso, um `carro` pode ter um método `Ligar()`, `Acelerar()`, `Freiar()`, `Trocar_Marcha()`, `Desligar()`, etc. Tudo isso são ações que um `carro` poderia fazer.

Além disso, um `carro` pode ter atributos como `Cor`, `Quantidade_de_Lugares`, `Velocidade_Maxima`, etc. Essas são características que podem variar dependendo do carro.

Outra característica importante é a capacidade de **herança** dos objetos. Então, eu poderia criar um objeto chamado `Gol` que herda os métodos e atributos do objeto `carro` e ainda pode ter seus próprios. Portanto, todo `Gol` seria um `carro`, mas nem todo `carro` seria um `Gol`.


Meu `Gol` teria o mesmo método `Ligar()`, herdado de `carro`, mas ele também teria um método `Ligar_ar_condicionado()` que o objeto `carro` não tinha. Podemos, até, modificar o método `Ligar()` do `Gol`, fazendo com que ele ligue de um jeito diferente que o objeto `carro`.