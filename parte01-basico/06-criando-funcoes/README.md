# Parte I - Javascript Básico

## 6. Criando Funções

**6.1. Conceito:** 

Função é um bloco de códigos com uma sequência de comandos/códigos. É uma das principais coisas que se usa em Javascript.
A função é executada quando alguma coisa a "chama". Ela pode ser usada várias vezes no mesmo script.

**6.2. Estrutura básica:**

**- Parte 1: - Declaração e uso:** 

Uma função é definida pela palavra `function`, seguida pelo seu nome, seguida por parênteses ().
O código a ser executado é colocado dentro de chaves {}.

```javascript
function nomeFuncao() {
    //código a ser executado
}
``` 
**Lembrando que:**
* Para ser uma função, é necessário utilizar parênteses no final do nome, por exemplo: `fazerAcao()`

:shipit: **Boas práticas** 

* A **boa prática** dita que o nome da função se inicie com letra minúscula
* Caso de nomear a função possua mais de uma palavra, cada nova palavra deve estar em letra maiúscula
 seguindo o padrão `camelCase`. 
* Não devemos utilizar acentuação no nome da função. Na verdade, **não use em lugar algum**.

**- Parte 2 - funções com parâmetros:**

Dentro dos parênteses () - que vem logo após o nome da função - podem haver informações. Essas informações são chamadas de `parâmetros`, também conhecidos como `argumentos`. Dentro da função, os parâmetros se comportam como variáveis locais.
Os parâmetros devem ser separados por vírgulas.

**6.3. Exemplos:** 

**Exemplo 1 - Utlização no HTML**

* No HTML:

```html
<button onclick="trocarDiv()"></button>
```

- onde:

`onclick` - ao clicar neste elemento (tag)

`trocarDiv()` - chama a função


* No Javascript:

```javascript
function trocarDiv() {
  var area = document.getElementById("area");
  var texto = prompt("Qual seu nome?");
  
  area.innerHTML = texto;
}
```

- onde:

`document.getElementById("area")` - procura elemento (tag) com id 'area'

`trocarDiv()` - nome da função

`var area` - variável chamada 'area', tem o valor do elemento de id 'area'

`var texto` - variável chamada 'texto'. tem o valor do prompt com a mensagem "Qual seu nome?"

`area.innerHTML` - vai alterar a informação interna do HTML da variável 'area'

` = texto;` - o valor a ser alterado no 'area.innerHTML' é o que está contido na variável 'texto'

**Exemplo 2 - Funções com parâmetros:**

* No HTML:

```html
<button onclick="trocarDiv('Fulano')">Fazer ação</button>
```

- onde:

`onclick` - ao clicar neste elemento (tag button)

`trocarDiv()` - chama a função

`'Fulano'` - parâmetro da função

* No Javascript:

```javascript
function trocarDiv(nome) {
  var area = document.getElementById("area");
  var texto = prompt("Qual seu sobrenome?");
  
  area.innerHTML = nome+" "+texto;
}
```

- onde:

`document.getElementById("area")` - procura elemento (tag) com id 'area'

`trocarDiv()` - nome da função

`var area` - variável chamada 'area', tem o valor do elemento de id 'area'

`var texto` - variável chamada 'texto', tem o valor do prompt com a mensagem "Qual seu nome?"

`area.innerHTML` - vai alterar a informação interna do HTML da variável 'area'

` = nome+" "+texto;` - o valor a ser alterado no 'area.innerHTML' é o que está contido no parâmetro 'nome' (neste caso, 'Fulano'), somado à 'texto', que será a resposta inserida pelo usuário no prompt "Qual seu sobrenome?" Se o usuário digitasse, por exemplo, 'De Tal', o retorno seria 'Fulano De Tal'

**Exemplo 3 - Funções com mais de um  parâmetro:**

* No HTML:

```html
<button onclick="trocarDiv('Fulano', 25)">Fazer ação</button>
```

- onde:

`onclick` - ao clicar neste elemento (tag button)

`trocarDiv()` - chama a função

`'Fulano'` - parâmetro 1

`25` - parâmetro 2

* No Javascript:

```javascript
function trocarDiv(nome, idade) {
  var area = document.getElementById("area");
  var texto = prompt("Qual seu nome?");
  
  area.innerHTML = nome+" "+texto+" tem" +idade+" anos";
}
```

- onde:

`document.getElementById("area")` - procura elemento (tag) com id 'area'

`trocarDiv()` - nome da função

`var area` - variável chamada 'area', tem o valor do elemento de id 'area'

`var texto` - variável chamada 'texto', tem o valor do prompt com a mensagem "Qual seu nome?"

`area.innerHTML` - vai alterar a informação interna do HTML da variável 'area'

` = nome+" "+texto+" tem" +idade+" anos";` - o valor a ser alterado no 'area.innerHTML' é o seguinte:
  - a informação do parâmetro 'nome' (neste caso, 'Fulano'), mais
  - a informação da variável 'texto', que será a resposta inserida pelo usuário no prompt "Qual seu sobrenome?", mais
  - a palavra "tem", mais
  - a informação do parâmetro 'idade' (neste caso, 25), mais
  - a palavra "anos"
 
 Então, se o usuário digitasse, por exemplo, 'De Tal', o retorno seria: Fulano De Tal tem 25 anos

**6.4. Material complementar:**

- Functions (em inglês)

Acesso em: https://www.w3schools.com/js/js_functions.asp
