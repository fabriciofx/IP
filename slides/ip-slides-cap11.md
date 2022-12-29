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

## Capítulo 11 - Módulos

---

## Módulo

- Conjunto de funções ou procedimentos organizados em arquivos que permitem aumentar a capacidade de uma linguagem de programação
- A linguagem JavaScript possui várias maneiras de se criar módulos, mas a mais simples é adicionar as funções e procedimentos em um arquivo com a extensão .js e carregá-lo no arquivo html, utilizando a tag `<script>` para isto

---

## Sintaxe

`<script src="arquivo.js"></script>`

Em que: `arquivo.js` é o arquivo que contém as funções e procedimentos a serem utilizados

**Observação**: vários módulos podem ser utilizados, basta adicionar uma tag `<script src="..."></script>` para cada arquivo

---

## Exemplo
  
- Colocar as funções e procedimentos relativos a arrays no arquivo `array.js`
- Adicionar com `<script src="array.js"></script>`
- Adicionar um `<script></script>` para colocar código que invoque as funções e procedimentos contidos em `array.js`
