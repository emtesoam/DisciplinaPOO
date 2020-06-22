# Curso em vídeo aula 05 - Herança em Programação Orientada a Objetos.

## Herança: Toda classe mãe têm características e comportamentos
- *A herança permite basear uma nova classe na definição de um outra classe previamente existente*
- *A herança será aplicada tanto para as características quanto para os comportamenteos.*
## Mãe(Progenitora/Superclasse){  
          Pessoa
       ------------   
        - nome
        - idade
        - sexo
        ----------
        +fazerAniv();
## }
 ## Filhos (Sub-classe){          
   ALuno              Professor      Funcionario
 ---------         --------------    -----------
  - matr           - especialidade    - setor
  - curso          -  salario         - trabalhando
  --------         ---------------   --------------
  + cancelarMatr() + receberAum()      mudarTrabalho() 
 ## }

 # Herança parte B (Árvore de herança, navegação)

 1. Herança de implementação: (Mas simples, pobre)

 2. Herança para Diferença: (Mas completa,rica )   

 ## Conteitos de Abstrato e Final

 * Classe abstrata:
 Uma classe abstrata não pode ser instanciada.  Só pode servir como Progenitora
 *  Método abstrato:
 Método declarado mas não implementado na Progenitora.
 * Classe Final:
 Não pode ser herdada por autra classe. É obrigatoriamente folha (Não pode ter filho)
 * Método Final:
 Não pode ser sobrescrito pelas sub-classes. Obrigatoriamente herdado 