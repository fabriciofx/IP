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

## Capítulo 5 - Estruturas de Decisão

---

## if...*else*

- Executa uma (ou mais) instrução(ções) se a especificada condicão for **truthy**. If a condição for **falsy** outra(s) instrução(ções) será(ão) executada(s) se o opcional *else* for declarado
- Todos os valores são considerados truthy, exceto os falsy que são o `false`, `0`, `-0`, `0n` (BigInt), `""`, `''`, ` `` `, (String vazia) `null`, `undefined` e `NaN` (Not a Number)

---

## if...*else*

```javascript
if (condição)
   instrução1;
```

```javascript
if (condição)
   instrução1;
else
   instrução2;
```
---

## if...*else*

```javascript
if (condição) {
   instrução1;
   instrução2;
   ...
   instruçãoN;
} else {
   instrução1;
   instrução2;
   ...
   instruçãoN;
}
```

---

## if...*else*

```javascript
var nota1, nota2, media;
nota1 = parseFloat(prompt("Digite a 1a nota"));
nota2 = parseFloat(prompt("Digite a 2a nota"));
media = (nota1 + nota2) / 2;
if (media >= 6.0) {
  document.write("O estudante esta aprovado");
} else {
  document.write("O estudante esta reprovado");
}
```

---

## if...*else* Aninhado

- if...*else* como instrução de outro if...*else*

```javascript
if (condição1) {
  if (condição2) {
    // Instruções executadas se a condição1 e a condição2 forem verdadeiras
  }
  // Instruções executadas se a condição1 for verdadeira
} else {
  // Instruções executadas se a condição1 for falsa
}
```

---

## if...*else* Aninhado

```javascript
var nota1, nota2, faltas, media;
nota1 = parseFloat(prompt("Digite a 1a nota"));
nota2 = parseFloat(prompt("Digite a 2a nota"));
faltas = parseInt(prompt("Digite a quantidade de faltas"));
media = (nota1 + nota2) / 2;
if (faltas <= 15) {
  if (media >= 6.0) {
    document.write("O estudante esta aprovado");
  } else {
    document.write("O estudante esta reprovado");
  }
} else {
    document.write("O estudante esta reprovado por falta");
}
```

---

## If...else if...*else*

```javascript
if (condição1) {
   instrução1;
   ...
   instruçãoN;
} else if (condição2) {
   instrução1;
   ...
   instruçãoN;
}
...
} else {
   instrução1;
   ...
   instruçãoN;
} 
```

---

## If...else if...*else*

```javascript
var dia;
dia = parseInt(prompt("Digite o dia da semana"));
if (dia == 1) {
    document.write("Segunda-feira");
} else if (dia == 2) {
    document.write("Terça-feira");
...
} else if (dia == 7) {
  document.write("Domingo");
} else {
  document.write("Dia inválido!");
}
```

---

## switch...case...*default*

- Avalia uma expressão, combinando o valor da expressão com uma cláusula case, executando as instruçõe cujo case casou com a expressão

---

## switch...case...*default*

```javascript
switch(expressão) {
  case valor1:
    // Instruções executadas quando o resultado da expressão for valor1
    break;
  case valor2:
    // Instruções executadas quando o resultado da expressão for valor2
    break;
  ...
  case valorN:
    // Instruções executadas quando o resultado da expressão for valorN
    break;
  default:
    // Instruções executadas quando o resultado da expressão não casar
    // com nenhum dos valores anteriores
}
```

---

## switch...case...*default*

```javascript
var dia;
dia = parseInt(prompt("Digite o dia da semana"));
switch(dia) {
  case 1:
    document.write("Segunda-feira");
    break;
  case 2:
    document.write("Terça-feira");
    break;
  ...
  case 7:
    document.write("Domingo");
    break;
  default:
    document.write("Dia inválido!");
}
```
