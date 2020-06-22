## Herança 

Objetivos

1. Entender o que é herança.
Herança é um mecanimos que permite uma classe herdade todos os atributos e métodos de uma outra classe
*hierarquia de classe ou de herança: É o mapeamento do tipo árvore de relacionamento que se formam entre classes como resultado da heranças.*  
Quanto mais alta a classe na hierarquia, mas abstrata é a classe;
sobre: abstrata;
dese: concreto;
* classe mãe ou superclasse
* classe filha ou subclasse
* Ancestral e descendente
* Raiz (base) e Folha
Generalização,Especialização,Herança simples, Herança Multipla.
2. Conhecer quais os tipos de herança existentes em POO.
Classes que Fornecem a Herança|Classes que Herdam de Outras
                        |:---:|:---:|
                   Superclasse|Subclasse
    
                           Mãe|Filha
                          Tipo|Subtipo
- Ancestral: É uma classe que aparece na hierarquia de classe em uma posição acima da progenitora (Mãe;
- Descendente: Dada uma classe,toda classe que aparece abaixo dela na hierarquia é uma descendente da classe dada;
- Raiz o base: É a classe no topo da hierarquia:
- Folha: É uma classe sem filha.    

1. Generalização: As classes mais genericas e abstratas dísponiveis que podem ser usadas para outras descenderem delas.
2.  Especialização: Possui um estado mais e comportamento mais especializado, ou seja, com mais detalhes de informação;


3. Entender o funcionamento da herança durante a execução do programa.
 -  Herança multipla: É uma capacidade de uma classe possuir mais de uma superclasse e herdar varias variáveis e métodos combinados da superclasse;
Em jaca usa-se a palavar: **Interfaces** paa heranças multiplas
 - Herança simplies: Cada classe pode ter apenas uma superclasse , embora uma superclasse possa ter várias subclasses; 
Em java usa-se a Palavar: **extends** para herança simples

4. Programar em Java usando a herança.
### A classe object: Todas as classe em Java descende de uma classe chamada object, mesmo que a declaração das palavras _extends Object_ seja omitida, a classe object é considerada a classe raiz da hieraquia de todas as classe java, sendo portanto, ancestral toda as classe da linguagem;

### Quando umas das classes usa a relação de herança, podemos dizer que essa classe possui um relacionamento chamado "É um" com a classe da qual ela herda. Tal relação também indica que uma classe é do mesmo tipo que a outra. Assim, nos exemplos anteriores, podemos dizer que "Automóvel" "é um" transporte Terreste , assim como podemos dizer que Terrestre "é um" (ou tipo de) transporte.

Não faz parte desta disciplina falar sobre interfaces. Também não é obrigatório que você já domine a simulação de herança múltipla usando interface em Java. Para isso, sugerimos que você primeiro domine a herança simples para no futuro procurar saber sobre o assunto.

Como leitura complementar, propomos o próprio tutorial Java da Sun, que pode ser acessado pelo seguinte endereço:

<http://java.sun.com/docs/books/tutorial/index.html>

Artigo da web que fala sobre herança:

<http://www.tiexpert.net/programacao/java/heranca.php>

