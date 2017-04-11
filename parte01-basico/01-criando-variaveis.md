# Parte I - Javascript Básico


## 1. Criando variáveis


**1.1. Conceito:**

As variáveis servem para armazenar dados.

Os dados podem ser: 

* **_string_** - sequência de caracteres, basicamente texto
* **número**  - dados numéricos, números inteiros ou ponto flutuante _float_
* **booleano**  - true ou false. Também chamado de _boolean_
* **_null_** - uma palavra-chave que indica um valor nulo - 
* **_undefined_** - valor que uma variável **não inicializada* recebe ao ser declarada
* **objeto** - Mais informações no módulo de JavaScript Avançado

Depois de definir uma variável, ela pode ser usada no código, para substituir todo o valor definido para ela.

Uma variável pode ser modificada no decorrer do script.

Além das variáreis, existem as constantes. Depois de definida, a constante terá um valor permanente, elas não podem ser modificadas durante o script.

Os nomes das variáveis e das constantes são chamados identificadores. Os identificadores não podem ser repetidos. Eles devem ser específicos e seguem as seguintes regras:

* deve ter pelo menos um caractere

* o primeiro caractere de um identificador precisa ser uma letra, um underline (_) ou um cifrão($)

* além de underline (_) ou cifrão($) não são permitidos outros caracteres especiais

* não são permitidos espaços

* a boa prática indica utilizar `camelCase` nos identificadores, ou seja, a primeira palavra é toda minúscula e as demais palavras iniciam com letra maiúscula (ver exemplo abaixo: `nomeVar`)

Você pode inicializar (definir informações) ou não inicializar (não definir informações) em sua `var`. Se você não inicializar, o valor é considerado indefinido (`undefined`, ou seja, ele ainda não tem nenhuma informação. Para usar, você deve ter inicializado (definido um valor).

Além do `undefined`, existe o `NaN` (not a number), que quer dizer "não é um número". Isto aparece quando realizamos cálculos que prevêem números mas que, por alguma razão, são determinados dados não-numéricos para se trabalhar.


**1.2. Estrutura:**

```javascript
const TAXRATE; // não inicializada - undefined

var nomeVar = "valor"; // inicializada - string
```
- onde:

`var` é o código JavaScript que inicia a definição da variável

`nomeVar` é qualquer identificador escolhido para esta variável

`"valor"` é o valor (rsrs) que esta variável passa a ter

**Observações:**

* o ponto e vírgula (;) é **ESSENCIAL** no final de cada código - ele finaliza aquela linha de código

* as aspas ("") na palavra _valor_ indicam que ela é uma `string`. Uma string é interpretada pelo JavaScript como texto - veremos sobre string, (adição e concatenação) em "8. Operações"

* para ser interpretado como número, ele não deve ser posto entre aspas ou deve-se usar parseInt() - veremos sobre o parseInt em "8. Operações"


**1.3. Exemplos:**

- Definir (inicializar) variáveis:

```javascript
var nome = "Fulano";

var idade = 90;
```

- Utilizar variáveis:

```javascript
alert("Meu nome é: "+nome); //ao rodar o código (carregar a página) o alert vai mostrar a mensagem em uma janela
```

- Definir constante:

```javascript
const TAXRATE = .925;
```

**1.4. Material complementar:**

- JavaScript Variables (em inglês)

Acesso em: https://www.w3schools.com/js/js_variables.asp

- Valores, Variáveis e Literais

Acesso em: https://developer.mozilla.org/pt-PT/docs/Web/JavaScript/Guia/Valores,_Vari%C3%A1veis_e_Literais

- Constantes

Acesso em: Use a cabeça! Javascript, de Michael Morrison
