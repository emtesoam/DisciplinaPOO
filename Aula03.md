## Aula 03 - Objetos, construtores 

# Objetivos

1.  Conhecer o conceito e a criação dos métodos Construtores.
- Construtires são: Construtores representam o código que roda sempre que você usa a palavra-chave new.
- bserve que esse método possui o mesmo nome da classe Carro e não possui tipo de retorno, pois seu retorno, como já mencionamos, é justamente a referência para o objeto na memória
    Ex.: 
    ```java
    class Carro {		
	String cor;
	String placa;
	Carro(String placa, String cor){
		this.placa = placa;
		this.cor = cor;
	}

}
    ```
  - Construtor é um método especial.
    - O construtor não é chamando diretamente.
        - O construtor é executado sempre que um objeto correspondente for construido.
            - construtor não possui valo de retorno.


            

- O que são construtores?

    Construtores são métodos especiais para a criação e inicialização de novas instâncias de classe (objetos).
    Inicializam o novo objeto e seus atributos.
    Criam todos os outros objetos de que esse objeto necessita.
    Realiza todas as outras operações que ele precisa para ser inicializado.

- O que faz o operador new?

    Ele inicializa o novo objeto e seus atributos, criam todos os outros objetos de que esse objeto necessita e realizam todas as outras operações de que ele precisa para ser inicializado.



2. Aprender como criar um objeto em Java.

