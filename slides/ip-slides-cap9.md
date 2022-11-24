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

## Capítulo 9 - Arrays

---

## Array

- Estrutura utilizada para guardar e manipular diversos tipos de dados
- Conjunto *indexado* de elementos de diversos tipos de dados
  - Indexado porque cada elemento pode ser distinguido de outro por meio de um *índice*
  - O índice inicia com `0` (zero) e termina com `nomeDoArray.length - 1`

---

## Array

- Criar um array com três nomes
  ```javascript
  var nomes = ["Maria", "Jose", "Pedro"];
  document.write(nomes[0]); // Mostra apenas o nome "Maria"
  document.write(nomes); // Mostra os nomes "Maria,Jose,Pedro"
  ```

  ou

  ```javascript
  var nomes = [];
  nomes[0] = "Maria";
  nomes[1] = "Jose";
  nomes[2] = "Pedro";
  ```

---

## Array

- Criar um array com diversos tipos de dados
  ```javascript
  var dados = ["Maria", 1.2, 15, false];
  document.write(dados); // Maria,1.2,15,false
  ```

- Saber quantos elementos o array possui
  ```javascript
  var nomes = ["Maria", "Jose", "Pedro"];
  document.write(nomes.length); // 3
  ```

---

## Array

- Primeiro elemento do array
  ```javascript
  var nomes = ["Maria", "Jose", "Pedro"];
  document.write(nomes[0]); // Maria
  ```

- Último elemento do array
  ```javascript
  var nomes = ["Maria", "Jose", "Pedro"];
  document.write(nomes[nomes.length - 1]); // Pedro
  ```
---

## Array

- Percorrer cada elemento do array
  ```javascript
  var nomes = ["Maria", "Jose", "Pedro"];
  for (var i = 0; i < nomes.length; i++) {
    document.write(nomes[i] + "<br>");
  }
  ```
  ou
  ```javascript
  var nomes = ["Maria", "Jose", "Pedro"];
  for (var nome of nomes) {
    document.write(nome + "<br>");
  }
  ```

---

## Array

- Percorrer cada elemento do array
  ```javascript
  var nomes = ["Maria", "Jose", "Pedro"];
  nomes.forEach(function (item, indice, array) {
    document.write(item + " " + indice + " " + array + "<br>");
  });
  // Maria 0 Maria,Jose,Pedro
  // Jose 1 Maria,Jose,Pedro
  // Pedro 2 Maria,Jose,Pedro
  ```

---

## Array

- Adicionar um item ao final do array
  ```javascript
  var nomes = ["Maria", "Jose", "Pedro"];
  nomes.push("Ana");
  document.write(nomes); // Maria,Jose,Pedro,Ana
  ```

- Adicionar um item ao início do array
  ```javascript
  var nomes = ["Maria", "Jose", "Pedro"];
  nomes.unshift("Ana");
  document.write(nomes); // Ana,Maria,Jose,Pedro
  ```

---

## Array

- Remover um item ao final do array
  ```javascript
  var nomes = ["Maria", "Jose", "Pedro"];
  var ultimo = nomes.pop();
  document.write(nomes); // Maria,Jose
  ```

- Remover um item ao início do array
  ```javascript
  var nomes = ["Maria", "Jose", "Pedro"];
  var primeiro = nomes.shift();
  document.write(nomes); // Jose,Pedro
  ```

---

## Array

- Procurar o índice de um item no array
  ```javascript
  var nomes = ["Maria", "Jose", "Pedro"];
  var indice = nomes.indexOf("Jose"); // 1
  ```

- Combina os elementos de um array em uma string
  ```javascript
  var nomes = ["Maria", "Jose", "Pedro"];
  document.write(nomes.join("-")); // Maria-Jose-Pedro
  ```

---

## Array

- Combina dois arrays em um
  ```javascript
  var nomes1 = ["Maria", "Jose"];
  var nomes2 = ["Pedro", "Ana"];
  var combinados = nomes1.concat(nomes2); // ["Maria", "Jose", "Pedro", "Ana"]
  ```

- Divide uma string em um array de substrings
  ```javascript
  var nome = "Maria da Silva Sauro";
  var subs = nome.split(" "); // ["Maria", "da", "Silva", "Sauro"]
  ```

---

# Arrays Bidimensionais (Matrizes)

- Criar uma matriz 2x3
  ```javascript
  var matriz = [[1, 2, 3], [4, 5, 6]];
  document.write(matriz); // 1,2,3,4,5,6
  ```
  ou
  ```javascript
  var matriz = [];
  matriz[0] = [1, 2, 3];
  matriz[1] = [4, 5, 6];
  document.write(matriz); // 1,2,3,4,5,6
  ```

---

# Arrays Bidimensionais (Matrizes)

- Somar uma unidade a cada elemento da matriz
  ```javascript
  var matriz = [[1, 2, 3], [4, 5, 6]];
  for (var i = 0; i < matriz.length; i++) {
    for (var j = 0; j < matriz[0].length; j++) {
      matriz[i][j] = matriz[i][j] + 1;
    }
  }
  document.write(matriz); // [[2, 3, 4], [5, 6, 7]]
  ```
  
---

# Arrays Bidimensionais (Matrizes)

- Criar uma matriz 2x3 com números inteiros informados pelo usuário
  ```javascript
  var matriz = [];
  for (var i = 0; i < 2; i++) {
    matriz[i] = [];
    for (var j = 0; j < 3; j++) {
      matriz[i][j] = parseInt(prompt("Digite um numero inteiro"));
    }
  }
  document.write(matriz);
  ```
