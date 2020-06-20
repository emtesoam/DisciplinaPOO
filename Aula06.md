## Composição ou Agregação


Objetivos
1. Saber o que significa Composição ou Agregação;

É um mecanismo de reaproveitamento (Reutilização) de classes utilizdo pala POO para aumentar a produtividade e qualidade no desenvolbimento de software.
 ### Simplificando, composição é a utilização de obejtos (ou instâncias) menores para cria uma objeto/instância maior. (Unir objetos) 
2. Criar objetos na linguagem Java que são compostos por outros objetos, fazendo uso prático do conceito de Composição;

Os métodos construtore das classes componetes (motor e direção) que fazem parte compsta (Automovél) podem ser chamadas de três maneiras:
 - Caso 1: Chamadas nos próprios construtores da classe que é composta.
``` java
class Automovel{
	private Motor motor;

	public void ligarPrimeiraVez(){
		motor = new Motor();
	}

	public void ligarPrimeiraVez(int potencia){
		motor = new Motor(potencia);
	}
}
```
  - Caso 2: Chamadas em qualquer método da classe que é composta;
``` java
class Automovel{
	private Motor motor;

	public void ligarPrimeiraVez(){
		motor = new Motor();
	}

	public void ligarPrimeiraVez(int potencia){
		motor = new Motor(potencia);
	}
}

```
  - Caso 3: Chamadas fora da classe que pe composta.
  ``` java
    public static void main(String[] args){
        Automovel automovel = new Automovel();
        Motor motor = new Motor();
        automovel.setMotor(motor)

    }
  ```

3. Entender como se comporta os modificadores de acesso de Java na Composição.

- Quando declaramos atributos públicos nas classes e reutilizamos essas classes dentro de outras, esses atributos podem não ser acessados facilmente, através da classe de composição;

- Quando temos atributos privados nas classes e reusamos essas classes, declarando suas instâncias como públicas, os atributos não passam a ser públicos;


### Quando ocorre o inveso do caso anterior, mas reforça que private não deixa de ser privado mesmo quando na classe que usa da composição (Automével) torna sue atributo (Direção) publc.

## Dica: Quando uma classe usa a composição para agregar outra classes, podemos dizer que ela em um relacionamento chamado "tem um". o qual descreve um relacionamento em que uma classa contém uma instância de outra classe