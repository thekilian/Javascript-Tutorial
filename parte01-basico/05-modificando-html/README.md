# Parte I - Javascript Básico

## 5. Modificando o HTML

**5.1. Conteúdo:** 

Alterar o HTML de **exibição**.
Este comando **não vai alterar** o arquivo HTML. Se a página for atualizada, volta ao padrão.


**5.2. Estrutura:**

```javascript
document.getElementById('nome_do_id').innerHTML = "";
```

**5.3. Exemplo:** 

* Exemplo 1 - ao clicar no botão, substituir por informação do prompt:
```javascript
<button onclick="document.getElementById('area').innerHTML = prompt('Qual seu nome?');">Fazer a ação</button>
```

- onde:
* `document` - vai no documento
* `getElementById` - procura elemento (tag) com id 'area'
* `inner.HTML` - vai substituir informação no innerHtml, ou seja, na parte interna do HTML
* `prompt` - substitui pelo prompt, ou seja, pela informação que o usuário digitar


* Exemplo 2 - alterar nome do botão:
```javascript
<button onclick="this.innerHTML = prompt('Qual o nome do botão?');">Fazer a ação</button>
```

- onde:
* `this` - é o prórpio elemento 


**5.4. Material complementar:**

- document.getElementById() Method (em inglês)

Acesso em: https://www.w3schools.com/jsref/met_document_getelementbyid.asp

- innerHTML Property (em inglês)

Acesso em: https://www.w3schools.com/jsref/prop_html_innerhtml.asp
