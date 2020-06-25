## Coleções em Java 

Objetivos

1. Compreender como armazenar objetos em estruturas de dados conhecidas como arrays.
utilização de vetores:
- double[] marca= new double[5];
- double[] marca = {10.02, 10.0, 9.56, 9.57, 9.56};
- for(int i = 0;i<5;i++){marca[i]);}

Como utilizar matriz
String[][] tabuleiro = new String[8][8];

2. Conhecer e aprender como usar de forma introdutória um conjunto de classes da biblioteca padrão de Java relacionada à manipulação de coleções de objetos.
String também são vetores e algunas funcionalidades são importantes como: **length**( que da o tamanho da string)

Coleções de Java:
- List: Listar coisas.
- Set: Conjunto de coisas.
- Map: coisas com um identificador único

Para importar a coleção utilizar: **import java.util.hashset;** ou **import java.util.*;**

### Set: Representa como na matemática um conjunto, um grupo de objetos únicos mas sem ordem definida (Sendo impossível, prever a ordem na qual sera apresentado)
O pricipal representante do Set é o **HashSet** 
```java
public class TesteHashSet{
	public static void main(String[] args){
		HashSet itens = new HashSet();
		itens.add("Chocolate");
		itens.add("Bala");
		itens.add("Brigadeiro");
	}
}

```
### List: Como o próprio nome sugre, representa uma lista de objetos sendo que nela os objetos podem se repetir.
Uma classe que é bastante utilizada é a **ArryList**. nela a ordem se mante na qual utilizou para adicionar 

```java
ArrayList nomes = new ArrayList();
nomes.add("Maria");
nomes.add("João");
``` 

### Map: São mapas de estruturas que se relacionam um objeto a outro por exemplo: um numero de CEP ao nome de Uma Rua

```java
public class TesteHashSet{
	public static void main(String[] args){
		HashMap livros = new HashMap();

		livros.put(1, "Volta ao mundo em 80 dias");
		livros.put(2, "Alice no país das maravilhas");
		livros.put(5, "Caninos Brancos ");
	}
}
```
------------------------------------------------------------ 
boolean add(Object) 
Adiciona um elemento na coleção. Como algumas coleções não suportam elementos duplicados (exemplo: Sets), esses métodos retornam verdadeiro (true) ou falso (false) para indicar se a adição foi bem sucedida.
boolean remove(Object) 
Remove determinado elemento da coleção. Se ele não fizer parte da coleção, retorna falso (false).
int size() 
Retorna a quantidade de elementos presentes na coleção.
boolean contains(Object) 
Procura por um determinado objeto na coleção. Vale salientar: a comparação é feita pelo método equals().
Lista Básica de Métodos da Interface Collection
------------------------------------------------------------

Dica:
"
Anote a Dica!
As coleções Java mantêm um mecanismo interno de ordenação e recuperação de dados e para isso fazem uso de tabelas hash. Tais tabelas são utilizadas para que a pesquisa de um objeto seja feita de maneira rápida. Mas, como funciona? Cada objeto é “classificado” pelo seu hashCode, método de java.lang.Object que retorna um int, e com isso podemos agrupar os objetos por esse valor. Quando é realizada uma busca, só é percorrido o grupo de objetos com o mesmo hashCode.
"
### Todas as classes do tipo Set e List descendem (implementam) a interface Collection :
interfaces como contratos que definem um conjunto de métodos que devem ser implementados pelas classes. No caso da interface Collection, ela define métodos para adicionar, remover, verificar a presença de um dado objeto

3. Aprender a utilizar o “for-each” para iterar sobre coleção.

Loop for each também conhecido como **enhancedloop** e **for-in** O for-each loop veio com o Java 6 como um loop especializado que simplifica a iteração sobre Arrays e Coleções. 
```java
int [ ]a = {1,2,3,4}
for (int x = 0 ; x <a.length ; x++) 
	     System.out.print(a[x]);
for (int n : a) 
	     System.out.print(n);
``` 

Como fica o o enchanced:
```java
for ( declaração : expressão ) {}
```

As duas partes são:

    *Declaração*: no bloco de declaração o tipo da variável pode ser compatível com o tipo dos elementos da coleção que você está acessando. Essa variável será a que utilizaremos no corpo do loop e o seu valor será o mesmo que o elemento corrente da coleção.
    *Expressão*: deve ser o Array ou coleção que você deseja iterar sobre. Pode ser qualquer tipo de coleção ou método cujo retorno seja uma coleção ou Array. Os tipos dos elementos dentro da coleção podem ser os seguintes: primitivos, objetos ou até mesmo outra coleção.
```java
long x2;
Long [] la = {7L, 8L, 9L};
Animal [] animals = { new Dog(), new Cat()}

for (Long x2 : la); // x2 já está declarado
for ( Dog d : animals); // você pode receber um Cat
```



4. Escrever códigos que utilizem a versão “genérica”das coleções.
O Generics nos ajudará em dois pontos, na hora de colocarmos e na hora de retirarmos elementos das coleções, através da aplicação do tipo específico
 ArrayList myList = new ArrayList()
generic list<String>myList = new ArrayList<String>()
é assim que fuinciona o generics
```java
List<String> myList = new ArrayList<String>(); // Agora informamos o tipo
myList.add("João"); // neste ponto está OK, adicionamos uma String.
myList.add(new Dog()); // Ops! Agora recebemos um erro de compilação!!!
recuperando:
String s = myList.get(0); // Sem Cast.

```
```java
for (String s : myList) {
    int x = s.length();
    // note que não é necessário utilizar um Cast antes de chamar o método da string "s"!
    // O compilador já sabe que "s" é uma String recuperada da coleção myList.
}
```