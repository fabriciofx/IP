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

## Capítulo 7 - Operadores de Incremento e Decremento

---

## Operador de Incremento

- Símbolo: `++`
- Adiciona um ao seu operando
- Operador unário
- Exemplo:

  ```javascript
  var x = 1;
  document.write(x + "<br>");
  x++;
  document.write(x + "<br>");
  ```

---

## Operador de Decremento

- Símbolo: `--`
- Subtrai um ao seu operando
- Operador unário
- Exemplo:

  ```javascript
  var x = 1;
  document.write(x + "<br>");
  x--;
  document.write(x + "<br>");
  ```

---

## Modos Pós-fixado e Prefixado

- Os operadores de incremento e decremento podem apresentar-se de dois modos distintos: pós-fixado e prefixado
- A diferença entre eles é **quando** a operação de incremento ou decremento ocorre
- No pós-fixado, retorna o valor do operando **antes** da operação
- No prefixado, retorna o valor **depois** da operação

---

## Modo Pós-fixado

```javascript
  var y, x = 1;
  document.write(x + "<br>");
  y = x++;
  document.write(x + "<br>");
  document.write(y + "<br>");
```

---

## Modo Prefixado

```javascript
  var y, x = 1;
  document.write(x + "<br>");
  y = ++x;
  document.write(x + "<br>");
  document.write(y + "<br>");
```

---

## Modo Pós-fixado

```javascript
  var y, x = 1;
  document.write(x + "<br>");
  y = x-- + 2;
  document.write(x + "<br>");
  document.write(y + "<br>");
```

---

## Modo Prefixado

```javascript
  var y, x = 1;
  document.write(x + "<br>");
  y = --x + 2;
  document.write(x + "<br>");
  document.write(y + "<br>");
```
