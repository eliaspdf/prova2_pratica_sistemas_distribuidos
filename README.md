# prova2_pratica_sistemas_distribuidos

Aluno: Elias Pina de faria
Data: 18/11/2026

1. situação-problema

o codgio de sistema de controle de processamento aprsentava três erros de lófica. 


2. primeira execução

ao executar pela primeira vez, o sistema apresentava erros na concorrência, replicação, consistência e tolerância a falhas.


3. problema A - concorrência
problema: o código falava que o máximo de pediso simultaneos eram 3.
alteração: apenas alterei esse número para 2.

4. problema B - replicação e consistência
problema: o código sincronizava a réplica na propria réplica, o que ocasionou o mal funcionamento.
alteração: eu sincronizei a réplica na principal.

5. problema C - tolerância a falhas
problema: o segundo "if" na parte de consultar estoque estava igual o primeiro, para consultar o principal, que fazia acabar no mesmo resultado.
alteração: eu mudei o segundo if, de principal para replica.

 6. validação do programa
após as correções, o programa cumpriu corretamente sua função.

7. análise técnica
questão 1
R: ele limita o máximo de pedidos.

questão 2
R: para que o programa possa conversar entre sí antes de processar os pedidos.

questão 3
R: é praticamente prever o que pode dar de errado. e nesse programa ele aparece quando o principal não está online.

questão 4
R: serve para barrar pedidos, quando chega no máximo.

questão 5
R: deve acontecer antes, para que o processamento possa acontecer corretamente.
