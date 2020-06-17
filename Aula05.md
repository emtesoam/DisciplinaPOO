##  Aula 05 - Encapsulamento 


 
Objetivos

1. Conhecer os conceitos ligados a encapsulamento;
**Encapsulamento é a característicada da POO capaz de ocultar partes (dados e detalhes) da emplementação interna de classes, do mundo exterior**
- Com o emcapsulamento só podemos ver as classes apenas pelos métodos.
**public**
**private**
**protected**
**Package ou Friendly**
 **public**:  garante que o atributo ou método da classe seja acessado ou executado a partir de qualquer outra classe.

**private**: pode ser acessado, modificado ou executado apenas por métodos da mesma classe, sendo totalmente oculto ao programador (ou outros objetos do sistema) que for usar instâncias dessa classe.

**protected**: funciona como o private, exceto que as classes filhas ou derivadas também terão acesso ao atributo ou método. Veremos mais sobre classes filhas na aula de Herança.

**Package ou Friendly**: não são palavras reservadas de modificadores de acesso. Os atributos e métodos são chamados de Package ou Friendly, quando não possuem modificadores, ou seja, são os atributos e métodos declarados sem modificadores. Isso significa que podem ser acessados por todas as classes pertencentes a um mesmo pacote (pacotes são pastas onde estão inseridos os arquivos das classes, para ajudar a organizá-las. Falaremos sobre pacotes em aulas futuras).



2. Entender, através de um contra-exemplo (exemplo errado), a importância do encapsulamento;
3. Entender com a “correção” do exemplo como se aplica essa característica de encapsulamento, tão importante para a programação OO.

