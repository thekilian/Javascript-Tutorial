Parte I - Javascript Básico


1. Criando variáveis


1.1. Conceito:

As variáveis servem para armazenar valores, que podem ser números e textos.

Depois de definir uma variável, ela pode ser usada no código, para substituir todo o valor definido para ela. 


1.2. Estrutura:

var nome = "valor";

- onde:

var é o código JS que inicia a definição da variável

nome é qualquer nome escolhido para esta variável

valor é o valor (rsrs) que esta variável passa a ter

- observações:

* o ponto e vírgula (;) é ESSENCIAL no final de cada código. Ele finaliza aquela linha de código.

* as aspas ("") na palavra valor indicam que ela é uma string. Uma string é interpretada pelo JS como texto.

* para ser interpretado como número, o número não deve ser posto entre aspas. 


1.3. Exemplos:

- Definir variáveis:

var nome = "Fulano";

var idade = 90;

- Utilizar variáveis:

alert("Meu nome é: "+nome); //ao rodar o cógigo (carregar a página) o alert vai mostrar a mensagem em uma janela
