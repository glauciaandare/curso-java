Você deve usar uma classe abstrata quando:

- Quer fornecer uma implementação parcial de uma classe, deixando alguns métodos como abstratos para serem implementados pelas subclasses1.
- Deseja compartilhar código entre várias subclasses, pois as classes abstratas permitem que você defina métodos não abstratos com implementações que podem ser herdadas1.
- Tem uma hierarquia de classes que compartilham um conjunto comum de comportamentos e quer garantir que certos métodos sejam implementados em todas as subclasses1.
- Precisa de um modelo para outras classes seguirem, mas não quer que instâncias dessa classe modelo sejam criadas2.


Por exemplo, se você está criando um sistema de animais em um zoológico e sabe que todos os animais precisam de um método para se alimentar, mas a forma como se alimentam é diferente para cada animal, você pode criar uma classe abstrata ```Animal``` com um método abstrato ```alimentar```. As subclasses específicas, como ```Leao``` e ```Girafa```, implementariam esse método de maneiras diferentes.

Aqui está um exemplo simples em Java:

```java
// Classe abstrata Animal
public abstract class Animal {
    public abstract void alimentar();

    // Método concreto que todas as subclasses podem herdar
    public void respirar() {
        System.out.println("Respirando...");
    }
}

// Classe concreta Leao que estende Animal
public class Leao extends Animal {
    @Override
    public void alimentar() {
        System.out.println("O leão está comendo carne.");
    }
}

// Classe concreta Girafa que estende Animal
public class Girafa extends Animal {
    @Override
    public void alimentar() {
        System.out.println("A girafa está comendo folhas.");
    }
}
```

Neste exemplo, ```Animal``` é uma classe abstrata que define o método abstrato ```alimentar```, que deve ser implementado por todas as subclasses. Além disso, ```Animal``` também possui um método concreto ```respirar```, que é compartilhado por todas as subclasses. As classes ```Leao``` e ```Girafa``` são concretas e fornecem implementações específicas do método ```alimentar```.

