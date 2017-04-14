# Parte I - Javascript Básico


## 1. Criando variáveis


**1.1. Conceito:**

As variáveis servem para armazenar dados.

Os dados podem ser: 

**Tipos primitivos**

* **string** - sequência de caracteres, basicamente texto
* **número**  - dados numéricos. Números inteiros ou ponto flutuante _float_
* **booleano**  - true ou false. Também chamado de _boolean_
* **null** - uma palavra-chave que indica um valor nulo
* **undefined** - valor que uma variável **não inicializada** recebe ao ser declarada

**Tipos Mistos**

* **array** - Conjunto ou coleção de dados de um tipo ou todos os tipos acima.
* **objeto** - Mais informações no módulo de JavaScript Avançado


Depois de definir uma variável, ela pode ser usada no código, para substituir todo o valor definido para ela.

Uma variável pode ser modificada no decorrer do script.

Além das variáreis, existem as constantes. Depois de definida, a constante terá um valor permanente. As constantes não podem ser modificadas durante o script.

Os nomes das variáveis e das constantes são chamados **_identificadores_**. Os identificadores **não** podem ser repetidos. Eles devem ser específicos e seguem as seguintes regras:

* deve ter pelo menos um caractere

* o primeiro caractere de um identificador precisa ser uma letra, um underline (_) ou um cifrão($)

* além de underline (_) ou cifrão($) não são permitidos outros caracteres especiais

* não são permitidos espaços

* a boa prática indica utilizar `camelCase` nos identificadores, ou seja, a primeira palavra é toda minúscula e as demais palavras iniciam com letra maiúscula (ver exemplo abaixo: `nomeVar`)

Você pode inicializar (definir informações) ou não inicializar (não definir informações) em sua `var`. Se você não inicializar, o valor é considerado indefinido (`undefined`, ou seja, ele ainda não tem nenhuma informação. Para usar, você deve ter inicializado (definido um valor).

Além do `undefined`, existe o `NaN` (not a number), que quer dizer "não é um número". Isto aparece quando realizamos cálculos que prevêem números mas que, por alguma razão, são determinados dados não-numéricos para se trabalhar.


**1.2. Estrutura básica:**

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
var nome = "Fulano"; // string

var idade = 90; // número - no caso um inteiro
```

- Utilizar variáveis:

```javascript
/*
Ao rodar o código abaixo (carregar a página),
o alert vai mostrar a mensagem em uma janela
*/
alert("Meu nome é: "+nome); // o operador '+' aqui concatena

var x = 10;
var y = 30;

var soma = x + y; // aqui o '+' realiza a soma de fato

// Imprime no console do browser o resultado:
console.log(soma); 
```

- Definir constante:

```javascript
const TAXRATE = .925;
```

- Definir um booleano:

```javascript
var ceuAzul = true;
```

- Definir um array:

```javascript
// Para aprender a declarar

// Usa-se [] para declarar um array em JavaScript

// Array de strings
var cesta = ['laranja' , 'maçã' , 'banana' , 'abacaxi'];

// Array de inteiros
var naturais = [ 1 , 3 , 8, 23 ];

/*
Samba do criolo doido. 
Dá pra fazer, mas não faça isso 
a menos que tenho um bom motivo
*/ 
var samba = ['capacete vermeio', 20 , true , null ];
```

- Definir um objeto:

```javascript
// Para aprender a declarar

// Usa-se {} para declarar um objeto em JavaScript

var pessoa = {
	nome: "Asdrúbal",
	idade: 39,
	telefone: '55-1234-56789'
}

// Teste no seu browser ;)
alert(pessoa.nome);
```

:shipit: **Boas práticas** 

**NUNCA** inicialize suas váriáveis, objetos ou arrays com o valor `undefined`. Caso contrário, será muito mais difícil corrigir um bug ou encontrar um erro, visto que este tipo de dado é utilizado pelo interpretador do JavaScript para identificar uma **variável declarada mas ainda não utilizada.**

**1.4. Material complementar:**

- JavaScript Variables (em inglês)

Acesso em: https://www.w3schools.com/js/js_variables.asp

- Valores, Variáveis e Literais

Acesso em: https://developer.mozilla.org/pt-PT/docs/Web/JavaScript/Guia/Valores,_Vari%C3%A1veis_e_Literais

- Constantes

Acesso em: Use a cabeça! Javascript, de Michael Morrison
