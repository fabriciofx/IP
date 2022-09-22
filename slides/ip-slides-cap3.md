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

## Capítulo 3 - Introdução à Linguagem JavaScript (JS)

---

## Características (algumas) de JavaScript

- Umas das tecnologias fundamentais da WWW (junto com HTML e CSS)
- Linguagem de alto nível e multi-paradigma
- Sintaxe semelhante a linguagem C
- Interpretada (na verdade compilada Just-in-Time (JIT))
- Tipagem dinâmica
- Não confundir as linguagens JavaScript com Java

---

## Como Criar um Programa em JavaScript

- Programas necessários
  - Um navegador (browser) qualquer
    - Google Chrome: https://www.google.com/intl/pt-BR/chrome/
    - Mozilla Firefox: https://www.mozilla.org/pt-BR/firefox/
    - Microsoft Edge: https://www.microsoft.com/pt-br/edge
  - Um editor de textos simples
    - Bloco de notas (Windows)
    - Visual Studio Code (vscode): https://code.visualstudio.com/ 

---

## Como Criar um Programa em JavaScript

- Para criar um programa JavaScript, crie um arquivo com a extensão `.html` e com a as tags `<script>`e `</script>`
  Exemplo:
  ```javascript
  <script>
    document.write("Olá mundo!");
  </script>
  ```
---

## Entrada de Dados

- Existem muitas maneiras de fazer a entrada de dados, mas usaremos a mais simples, que é solicitar que o usuário informe o dado
- Na linguagem JavaScript utilizaremos a instrução `prompt()`
  Exemplo:
  ```javascript
  prompt("Informe o seu nome");
  ```

---

## Saída de Dados

- Existem muitas maneiras de fazer a saída de dados, mas usaremos a mais simples, que é escrever na tela
- Na linguagem JavaScript utilizaremos a instrução `document.write()`
  Exemplo:
  ```javascript
  document.write("Ana");
  ```

---

## Tipos de Dados

- String
  - Sequência de caracteres (letras, números e outros símbolos)
  - Podem aparecer entre aspas* (`"` `"`) 
  - Exemplos:
    "José", "27", ".", ",", " ", ""
- Números Inteiros
  - Exemplos:
  - 10, 0, -1, 23723, etc.

---

## Tipos de Dados

- Números Reais (ou Ponto-Flutuante)
- Exemplos:
  0.0, 10.0, -100.0, 3.1415, 12345.7890, etc.

---

## Convertendo entre Tipos

- De String para Número Inteiro
  - Utilize a instrução `parseInt()`
  - Exemplo:
    `parseInt("123")`
- De String para Número Real
  - Utilize a instrução `parseFloat()`
  - Exemplo:
    `parseFloat("123.456")`

---

## Variável

- Representação da memória RAM
- Na linguagem JavaScript é represntada por meio da instrução `var`
- Podemos declarar mais de uma variável na mesma linha
  Exemplos:
  ```javascript
  var nota1;
  var nota2, nota3;
  ```

---

## Armazenando um Valor em uma Variável

- Utilize o operador de atribuição `=`
- Exemplos:
  ```javascript
  var nota1 = 8.5;
  var nome = "Ana Beatriz";
  var idade;
  idade = 32;
  ```

---

## Operadores Aritméticos

| Operador | Operação             |
|----------|----------------------|
|  + ou -  | Mais / Menos unários |
|    +     | Adição               |
|    -     | Subtração            |
|    /     | Divisão              |
|    *     | Multiplicação        |
|    %     | Resto da divisão     |
|    **    | Exponenciação        |

---

## Precedência dos Operadores Aritméticos

- Qual operação é realizada primeiro? 
- `-` ou `+` (unários), `*` ou `/` ou `%`, `+` ou `-` (binários)
- Exemplos:
  4 + 4 / 2
  4 / 4 + 2

---

## Associatividade dos Operadores Aritméticos

- Dados dois operadores de mesma precedência, qual operação é realizada primeiro?
- Exemplo:
  - 8 / 4 / 2
- Unários: não aplicável
- Binários: esquerda para a direita, exceto a `**` que é direita para esquerda
- Parênteses (`(` e `)`) alteram a precedência 

---

## Maiores Detalhes sobre Precedência e Associatividade

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Operator_Precedence

---

## Exemplos de Programação

- Revisitando o problema de calcular a média de uma discipina:
  
  *Problema: Um professor do Curso Técnico em Informática do IFPE deseja utilizar um computador para lhe auxiliar no cálculo da média de cada estudante em uma disciplina*

---

## Exemplos de Programação

```javascript
var nota1Str, nota2Str, nota1, nota2, media;
nota1Str = prompt("Digite a 1a nota");
nota1 = parseFloat(nota1Str);
nota2Str = prompt("Digite a 2a nota");
nota2 = parseFloat(nota2Str);
media = (nota1 + nota2) / 2;
document.write("Media: " + media);
```

---

## Exemplos de Programação (Melhorado)

```javascript
var nota1, nota2, media;
nota1 = parseFloat(prompt("Digite a 1a nota"));
nota2 = parseFloat(prompt("Digite a 2a nota"));
media = (nota1 + nota2) / 2;
document.write("Media: " + media);
```



