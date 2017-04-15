# Parte I - Javascript Básico

## 7. Modificando uma lista

**7.1. Conceito:** 

Manipulação de elementos de uma lista.

* Substituir conteúdo: `inner HTML`

* Adicionar conteúdo ao conteúdo existente: existem várias formas de fazer


**7.2. Estrutura básica:**

```javascript
function nomeFuncao() {
    //código a ser executado
}
``` 

**7.3. Exemplo:** 

```javascript
function adicionarIngrediente() {
  var ing = document.getElementById("ingrediente").value;
  var listahtml = document.getElementById("lista").innerHTML;
  
  listahtml = listahtml + "<li>"+ing+"</li>";
  
  document.getElementById("lista").innerHTML = listahtml;
}
```

- onde:

`adicionarIngrediente()` - nome da função

`var ing` - variável chamada 'ing', tem o valor do elemento de id 'ingrediente' somado ao `value`

`var listahtml` - variável chamada 'listahtml', tem o valor do elemento de id 'lista' e armazena o conteúdo do innerHTML na variável 'listahtml'

`value` - pega o valor digitado pelo usuário

` listahtml = listahtml + "<li>"+ing+"</li>";` - esta linha de código vai pegar o conteúdo que tem na var 'listahtml' e vai somar a este conteúdo o que o usuário digitar

`"<li>"+ing+"</li>"` - inclui a informação digitada pelo usuário (ing) no item da lista (tag "li")


- resumindo: neste exemplo, você pega o conteúdo do elemento atual, adiciona mais conteúdo a ele e substitui depois.



**7.4. Material complementar:**

- Value Property (em inglês)

Acesso em: https://www.w3schools.com/jsref/prop_option_value.asp
