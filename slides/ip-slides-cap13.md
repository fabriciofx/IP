---
marp: true
theme: gaia
backgroundColor: white
color: black
paginate: true
footer: Introdução à Programação - Fabrício Barros Cabral <<fabricio.cabral@ead.ifpe.edu.br>>
---
<style>
img[alt~="center"] {
    display: block;
    margin: 0 auto;
}
</style>

<!-- _paginate: false -->
# **Introdução à Programação**

## Capítulo 13 - Interação com o Usuário

---

## Acentuação

- Codificação UTF-8 (Unicode)
  ```html 
  <meta charset="utf-8">
  ```
- Exemplo
  ```javascript
  <meta charset="utf-8">
  <script>
    document.write("Uma mensagem com a acentuação correta!");
  </script>
  ```

---

## Entrada de Dados

- Elementos de formulário HTML
  `input`, `label`, `select`, `textarea`, `button`, `fieldset`, `legend`, `datalist`, `output`, `option` e `optgroup`
- Referência
  https://www.w3schools.com/html/html_form_elements.asp

---

## Entrada de Dados

- Atributos
  `name`: Especifica o nome do elemento (apenas para alguns elementos)
  `id` : Especifica um único identificador para um elemento (global)
- Exemplo
  ```html
  <button id="soma">+</button>
  ```
- Referência
  https://www.w3schools.com/tags/ref_attributes.asp


---

## Entrada de Dados

- Input
  ```html
  <input />
  ```
- O padrão do input é o do tipo *text* (texto)
- Para ler o valor de um input `input.value`
- Para alterar o valor de um input `input.value = valor`

Observação: para ler/alterar o conteúdo de um elemento HTML usamos a propriedade `innerHTML`

---

## Entrada de Dados

- Existem diversos tipos de input, que variam de acordo com o atributo `type`. Exemplo:
  ```html
  <input type="password" />
  ```
- Tipos (type) de input
  
  `button`, `checkbox`, `color`, `date`, `datetime-local`, `email`, `file`, `hidden`, `image`, `month`, `number`, `password`, `radio`, `range`, `reset`, `search`, `submit`, `tel`, `text`, `time`, `url` e `week`
  
---

## Selecionando Elementos

- Seleciona o primeiro elemento no documento que casa com o seletor especificado
  ```javascript
  document.querySelector(seletor)
  ```
- Exemplo: seleciona o primeiro elemento `button` que encontrar
  ```javascript
  var button = document.querySelector("button");
  ```
- Referência
  https://www.w3schools.com/jsref/met_document_queryselector.asp

---

## Selecionando Elementos

- Seleciona o elemento no documento que casa com o `id` especificado

  ```javascript
  document.getElementbyId(id)
  ```
- Exemplo: seleciona o elemento com o `id` soma
  ```javascript
  var buttonSoma = document.getElementById("soma");
  ```
- Referência
  https://www.w3schools.com/jsref/met_document_getelementbyid.asp

---

## Eventos

- Associar um evento a um elemento `addEventListener()`
- Sintaxe
  ```javascript
  elemento.addEventListener(evento, função, captura);
  ```
  Em que:
    `evento` é o nome do evento a ser associado ao elemento
    `função` é o código da função JavaScript a ser executada quando o evento for disparado
    `captura` ordem de captura do evento (consulte as referências)

---

## Eventos

- Exemplo: associa o evento `click` a um `button`, fazendo ele abrir um `alert`
  ```javascript
  button.addEventListener(
    "click",
    function() {
        alert("Um botão foi pressionado");
    }
  );
  ```

---

## Eventos

- Um evento também pode ser associado via propriedade `on` + nome do evento
- Exemplo
  Evento: `click`
  Propriedade: `onclick`
  ```javascript
  button.onclick = function() {
    alert("Um botão foi pressionado");
  }
  ```

---

## Eventos

- Referências
  https://imasters.com.br/front-end/javascript-bubbling-e-capturing
  https://developer.mozilla.org/en-US/docs/Web/Events/Creating_and_triggering_events
  https://www.w3schools.com/jsref/dom_obj_event.asp
  https://www.w3schools.com/tags/ref_eventattributes.asp


---

## Exemplo: mostrar a cor escolhida

```javascript
<meta charset="utf-8"/>
<input type="color"/>
<p id="hex"></p>
<script>
    var color = document.querySelector("input");
    color.oninput = function() {
        document.getElementById("hex").innerHTML = color.value;
    }
</script>
  ```

---

## Saída de Dados

- Alert
  ```javascript
  alert(mensagem);
  ```

---

## Exemplos

- Jogo do adivinha o número
- Calculadora simples


