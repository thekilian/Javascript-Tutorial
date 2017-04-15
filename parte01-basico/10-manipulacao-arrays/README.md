# Parte I - Javascript Básico

## 10. Manipulação de arrays

**10.1. Conceito:** 

Array é uma variável mais avançada - uma variável composta - que armazena vários valores.

Os elementos dentro do array seguem a ordem numérica, iniciando pelo zero (0), ou seja, o primeiro item de um array é considerado zero (0); o segundo item é o um (1); e assim por diante. 


**10.2. Estrutura básica:**

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

**10.3. Exemplos:** 

**Exemplo 1 - array completa:**

```javascript
var lista = ["arroz", "feijão", "carne", 20];

lista;
```

_Resultado: ["arroz", "feijão", "carne", 20]_

- onde:

`var lista` - define valores para a variável `lista` (neste caso, arroz, feijão, carne, 20)

`lista` - chama a variável `lista`

`Resultado` - mostrará o resultado (neste caso, todos os elementos do array: ["arroz", "feijão", "carne", 20])


**Exemplo 2 - um elemento do array:**

```javascript
var lista = ["arroz", "feijão", "carne", 20];

lista[0];
```

_Resultado: "arroz"_

- onde:

`var lista` - define valores para a variável `lista` (neste caso, arroz, feijão, carne, 20)

`lista[0]` - chama o primeiro elemento da variável `lista`

`Resultado` - mostrará o resultado (neste caso, o primeiro elemento do array: "arroz")


**Exemplo 2 - tamanho do array:**

```javascript
var lista = ["arroz", "feijão", "carne", 20];

lista.lenght;
```

_Resultado: 4_

- onde:

`var lista` - define valores para a variável `lista` (neste caso, arroz, feijão, carne, 20)

`lenght` - retorna o número de elementos do array

`Resultado` - mostrará o resultado (neste caso, o número total de elementos do array: 4)


**10.4. Material complementar:**

- Arrays (em inglês)

Acesso em: https://www.w3schools.com/js/js_arrays.asp
