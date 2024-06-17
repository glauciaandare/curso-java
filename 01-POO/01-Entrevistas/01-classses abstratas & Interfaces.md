## Perguntas sobre classes abstratas e interfaces 

1- O que são classes abstratas e como elas diferem de classes regulares em Java?

Classes abstratas são usadas para representar conceitos abstratos e não podem ser instanciadas. Elas diferem de classes regulares porque podem conter métodos abstratos, que são declarados sem uma implementação.

***

2 - Pode uma classe abstrata ser instanciada? Por quê?

Não, uma classe abstrata não pode ser instanciada diretamente porque ela pode conter métodos abstratos que não têm corpo e, portanto, não podem ser executados.

---

3 - Quais são os cenários em que você usaria uma classe abstrata?

Classes abstratas são úteis quando você tem uma base comum para várias subclasses, mas nunca espera criar objetos da classe base.

******

4 - O que são interfaces em Java e como elas diferem de classes abstratas?

Interfaces são contratos que definem métodos que devem ser implementados por classes que as implementam. Diferem de classes abstratas porque todas os métodos em uma interface são implicitamente abstratos e públicos, e interfaces não podem conter estado (atributos).

___

5 - Pode uma interface conter métodos implementados em Java?

Sim, a partir do Java 8, interfaces podem conter métodos padrão com implementação, além de métodos estáticos.

***

6 - Como o polimorfismo se relaciona com classes abstratas e interfaces?

O polimorfismo permite que objetos sejam tratados como instâncias de suas classes base ou interfaces, proporcionando flexibilidade no uso de diferentes tipos de objetos de maneira intercambiável.

***

7 - Quando você escolheria usar uma interface em vez de uma classe abstrata?

Você usaria uma interface quando precisasse definir um contrato que poderia ser implementado por classes que pertencem a diferentes hierarquias de classes.

***

8 - Pode uma classe em Java implementar múltiplas interfaces?

Sim, uma classe em Java pode implementar várias interfaces, o que permite a herança múltipla de tipo.
***

9 - Como você pode usar interfaces para implementar a separação de preocupações?

Interfaces permitem a separação de preocupações ao definir contratos claros para funcionalidades, permitindo que diferentes implementações sejam trocadas sem afetar o código que depende da interface.
***

10 - Quais são as limitações ao usar classes abstratas e interfaces?

As limitações das classes abstratas incluem a impossibilidade de múltipla herança de implementação. Já as interfaces não podem conter estado e, até o Java 7, não podiam conter implementações de métodos.