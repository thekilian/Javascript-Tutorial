# Parte I - Javascript Básico

## 9. Arrays

**9.1. Conceito:** 

Array é uma variável mais avançada - uma variável composta - que armazena vários valores.

Os elementos dentro do array seguem a ordem numérica, iniciando pelo zero (0), ou seja, o primeiro item de um array é considerado zero (0); o segundo item é o um (1); e assim por diante. 


**9.2. Estrutura básica:**

```javascript
var nome_array = [item1, item2, item3, item4, item5...];
``` 

_Observação_ - ordem os elementos: var nome_array = [0, 1, 2, 3, 4, ...];

- Um array também pode ser apresentado em múltiplas linhas, da seguinte forma:

```javascript
var nome_array = [
  item1,
  item2,
  item3,
  item4,
  item5
  ...
];
``` 

**9.3. Exemplos:** 

**Exemplo 1 - lista:**

```javascript
var lista = ["arroz", "feijão", "carne", 20];

lista;
```

_Resultado: ["arroz", "feijão", "carne", 20]_

- onde:

`var lista` - define valores para a variável `lista` (neste caso, arroz, feijão, carne, 20)

`lista` - chama a variável `lista`

`Resultado` - mostrará o resultado (neste caso, todos os elementos do array: ["arroz", "feijão", "carne", 20])


**Exemplo 2 - soma #2:**

```javascript
var x = 20;
var y = x + 30;

alert(y);
```

_Resultado: 50_

- onde:

`var x` - define valores para a variável `x` (neste caso, 20)

`var y` - define valores para a variável `y` (neste caso, x + 30)

`alert(y)` - chama a variável `y` via `alert`

`Resultado` - alert mostrará o resultado (neste caso, a soma dos valores 20 e 30)


**Exemplo 3 - concatenação #1:**

```javascript
var x = "5" + "3";

alert(x);
```

_Resultado: 53_

- onde:

`var x` - define valores para a variável `x` (neste caso, "5" + "3")

`alert(x)` - chama a variável `x` via `alert`

`Resultado` - alert mostrará o resultado (neste caso, a concatenação dos valores "5" e "3")


**Exemplo 4 - concatenação #2:**

```javascript
var x = "20";
var y = x + "30";

alert(y);
```

_Resultado: 2030_

- onde:

`var x` - define valores para a variável `x` (neste caso, "20")

`var y` - define valores para a variável `y` (neste caso, x + "30")

`alert(y)` - chama a variável `y` via `alert`

`Resultado` - alert mostrará o resultado (neste caso, a concatenação dos valores "20 e "30")


**Exemplo 5:**

* No HTML:

```html
<input type="text" name="campo1" id="campo1"/>
<input type="text" name="campo2" id="campo2"/>
<button onclick="somar()"></button>
```

* No Javscript:

```javascript
function somar() {
  var campo1 = parseInt(document.getElementById("campo1").value);
  var campo2 = parseInt(document.getElementById("campo2").value);
  
  var soma = campo1 + campo2;
  
  alerta(soma);
}
```


- onde:

`somar()` - nome definido para a função

`var campo1` - define valores para a variável `campo1` (neste caso, o que o usuário inserir no campo 1 - por causa do `value`)

`var campo2` - define valores para a variável `campo2` (neste caso, o que o usuário inserir no campo 2 - por causa do `value`)

`parseInt()` - transforma elemento em número

`value` - pega o valor inserido pelo usuário (neste caso, o que for inserido nos campos 1 e 2, respectivamente)

`var soma` - define valores para a variável `soma` (neste caso, a soma dos valores inseridos pelo usuário nos campos 1 e 2)

`alert(soma)` - chama variável `soma` via `alert`



**9.4. Material complementar:**

- Arrays (em inglês)

Acesso em: https://www.w3schools.com/js/js_arrays.asp
