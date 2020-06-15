# Aula 02 - Classes, atributos e métodos 
 
## **Objetivos**

1. Entender a teoria sobre Classe;
    - Classe é um modelo/molde/froma de construção de objetos
    - O modelo define as características e comportamentos que os objetos irão desempenhar: 
        - características = seus valores
        - comportamentos = desempanhar ações 
    -  A classe abstrada não existe (Concretamente)       
_Elas as classes abstratas só servem para gerar objetos, por não existirem_ 
 

2. Entender em detalhes uma classe codificada usando a linguagem Java;

    - O nome de uma variável deve ser uma sequência de letras Unicode e dígitos, iniciando sempre com uma letra, "$" ou o caractere de sublinhado "_".
    - Caracteres subsequentes podem ser letras, dígitos, $ ou "_".
    - Espaços não são permitidos em nomes de variáveis.
    - Palavras reservadas da linguagem, tais como, class, int, float, for, while etc. não podem ser usadas como nomes de variáveis.
    - Nomes de variáveis são sensíveis a letras minúsculas e maiúsculas. Em outras palavras, dois atributos com nomes "placa" e "Placa", por exemplo, são considerados dois atributos diferentes.


3. Criar atributos e métodos em classes Java.


    Um dos oito tipos de dados primitivos.
- Inteiros: byte (1 byte), short (2 bytes), int (4 bytes), long (8 bytes);
- Reais: float (4 bytes), double (8 bytes)
- Booleanos: boolean (1 byte)
- Caracter: char (2 bytes)
- O nome de uma classe ou interface.
- Uma coleção.

## Constantes:
Para declarar uma constante, use a palavra chave **final** antes da declaração do atributo e inclua um valor inicial para esse último. O valor de uma constante nunca poderá ser modificado.
```java
class Matematica {
	final int DEZENA = 10;
	final double E = 2.71828;
}
```
### Metodo _Get_: Serve para retornar o valor de um atributo

`String getCor(){
    return cor;
}`


**Método get não possui parâmetro**
--- 
### Método _Set_: Serve para alterar o valor de um atributo
`void setCor(String cor){
    this.cor=cor;
}`

### Definição do métodos
! [DefineçãodoMétodo](Screenshot_2020-06-15 Material Didático - IMD.png)


``` java
void setCor (String cor){
    this.cor = cor; 
    } ``` 

Void | topo de retorno
SetCor | nome do método
(String cor) | Lista de parâmetro
{this.cor = cor} | Corpo do método
