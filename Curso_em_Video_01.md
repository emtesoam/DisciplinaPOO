# Curso em vídeo aula 03

[Aula03](https://www.youtube.com/watch?v=jFI-qqitzwk&list=PLHz_AreHm4dkqe2aR0tQK74m8SFe-aGsY&index=6)

## UML - Diagrama de Classe

 ## Modificadores de visibilidade
    Os modificadores de visibilidade indicam o nível de acesso aos componetes internos de uma classe.
    Símbolos usados UML 
* (+) públco (Ex. Telefone público. Todo mundo pode usar)
    Classe atual e todas as outras classes podem ver e usar.
* (-) privado (Ex. Meu telefone celular. Só eu posso usar)
    Somente a classe atual
* (#) protegido (Ex. Telefone da minha casa. As pessoas da minha casa podem usar)
    Ex. No caixa de um supermercado o caixa é privado, mas o atendente é público, a caixa pode modificar o troco e me entregar. Prém eu não posso mexer no caixa, pois é privado.
    Classe atual e todas as sub-classes  

   ##      Caneta 
  (+)modelo|(+)cor|(-)ponta|(#)tampada
    :---:|:---:|:---:|:---:
  (+)escrever()|(+)rabiscas()|(+)pintar()|(-)destampar() 

O UML (Diagrama de classes) diz que todo molde é um retângulo, com três linda onde a primeira linha fica no nome do molde (Classe) no meio o atributos e por fim os métodos.

   