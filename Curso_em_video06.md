## Polimorfismo

Poli= muitas.
Morfo = formas.

* Polimorfismo em java, permite que um mesmo nome represente vários comportamentos diferentes.

- Todo método() tem uma assinatura:
 todos os método() têm quantidade e os tipos dos parâmetro
 Dica: O retorno não conta como caracteristica para o polimorfismo;
 Nome,quantiade de paramentros e tipo de parametro.
Polimoformos de sobreposição: quando a quantidade e os tipo de atributos são os mesmo. Podendo se nenhum atributo.

 Tipode de Polimorfismo:
 - Sobreposição: Acontece quando substituímos um método de uma superclasse na sua subclasse, usando a mesma assinatura. Em outras palavras, mesma assinatura em classes distintas 
 - Sobrecarga: Assinaturas diferentes mesma classe, sobrecarga

``` java
 public void reagir(String frase){ }
    
    public void reagir(int hora,int minuto){}
    
    public void reagir(boolean dono){}
``` 
Resumindo:
Polimofirmos de sobreposição:
Mesma assinatura;
Classes diferentes.
Polimorfismo de sobrecarga:
Assinaturas diferentes;
Mesma Classe.