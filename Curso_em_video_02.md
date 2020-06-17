
ContaBanco

+ numConta
# tipo
- dono
- saldo
- status

abrirConta()
fecharConta()
depositar()
sacar()
pagarMensalidade()

Algumas situações

**Topo** da conta aceita dois valores:
cc: conta corrente
cp: conta poupança

abrir contar()
    boolean true or false
 - Abrir conta corrente ganha= R$ 50 
 - Abrir conta poupaça ganha=
 R$ 150

fechar contar()
  vericar se tem saldo
  verificar se não tem divida

depositar()
 - status da conta precisa esta verdadeiro

sacar() 
    - estados abrir conta verdadeiro
    - saldo na conta para sacar
pagarMensalidade()
   - fazer um gatilho para sempre que chamar mensalidade vai ser cobrada RS 12 CC e 20 CP diretamente do saldo       

metodo construtor{
    abrirConta= falso
    saldo=0
}