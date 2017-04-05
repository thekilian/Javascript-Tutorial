Parte I - Javascript Básico


1. Criando variáveis


1.1. Conceito:

As variáveis servem para armazenar dados.

Os dados podem ser: texto (sequência de caracteres), número (dados numéricos) e booleando (true ou false).

Depois de definir uma variável, ela pode ser usada no código, para substituir todo o valor definido para ela.

Uma variável pode ser modificada no decorrer do script.

Além das variáreis, existem as constantes. Depois de definida, a constante terá um valor permanente, elas não podem ser modificadas durante o script.

Os nomes das variáveis e das constantes são chamados identificadores. Os identificadores não podem ser repetidos. Eles devem ser específicos e seguem as seguintes regras:

* deve ter pelo menos um caractere

* o primeiro caractere de um identificador precisa ser uma letra, um underline (_) ou um cifrão($)

* além de underline (_) ou cifrão($) não são permitidos outros caracteres especiais

* não são permitidos espaços

* a boa prática indica utilizar camelCase nos identificadores, ou seja, a primeira palavra é toda minúscula e as demais palavras iniciam com letra maiúscula (no exemplo abaixo: nomeVar)

Você pode inicializar (definir informações) ou não inicializar (não definir informações) sua var. Se você não inicializar, o valor é considerado indefinido (undefined), ou seja, ele ainda não tem nenhuma informação. Para usar, você deve ter inicializado (definido um valor).

Além do undefined, existe o NaN (not a number), que quer dizer "não é um número". Isto aparece quando realizamos cálculos que prevêem números mas que, por alguma razão, são determinados dados não-numéricos para se trabalhar.


1.2. Estrutura:

const TAXRATE; //não inicializada

var nomeVar = "valor"; //inicializada

- onde:

var é o código JS que inicia a definição da variável

nomeVar é qualquer identificador escolhido para esta variável

valor é o valor (rsrs) que esta variável passa a ter

- observações:

* o ponto e vírgula (;) é ESSENCIAL no final de cada código - ele finaliza aquela linha de código

* as aspas ("") na palavra valor indicam que ela é uma string. Uma string é interpretada pelo JS como texto

* para ser interpretado como número, ele não deve ser posto entre aspas ou deve-se usar parseInt() - veremos sobre o parseInt em "8. Operações"


1.3. Exemplos:

- Definir (inicializar) variáveis:

var nome = "Fulano";

var idade = 90;

- Utilizar variáveis:

alert("Meu nome é: "+nome); //ao rodar o código (carregar a página) o alert vai mostrar a mensagem em uma janela

- Definir constante:

const TAXRATE = .925;


1.4. Material complementar:

- JavaScript Variables (em inglês)
Acesso em: https://www.w3schools.com/js/js_variables.asp

- Valores, Variáveis e Literais
Acesso em: https://developer.mozilla.org/pt-PT/docs/Web/JavaScript/Guia/Valores,_Vari%C3%A1veis_e_Literais

- Constantes
Acesso em: Use a cabeça! Javascript, de Michael Morrison
