# Parte I - Javascript Básico

## 8. Operações

**8.1. Conceito:** 

Como realizar operações com Javascript.

_Observação_ - o sinal de adição (+) pode significar a soma dos elementos ou a concatenação deles:

* `soma`: 1 + 1 = 2, por exemplo

* `concatenção`: "1" + "1" = 11, por exemplo. Se apenas um dos elementos for uma string, ainda assim, será uma concatenação, e **não** uma soma: "1" + 1 = 11, por exemplo. 


**8.2. Estrutura básica:**

```javascript
function nomeFuncao() {
    //código a ser executado
}
``` 

**8.3. Exemplo:** 

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



**8.4. Material complementar:**

- Value Property (em inglês)

Acesso em: 
