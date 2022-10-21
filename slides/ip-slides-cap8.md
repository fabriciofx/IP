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

## Capítulo 8 - Estruturas de Repetição

---

## Estruturas de Repetição

- Também conhecidos como laço ou loop
- Instruções utilizadas para repetir um conjunto de instruções
  - `for`
  - `while`
  - `do-while`

---

## For

```javascript
for (inicial; condicao; incremento) {
  instruções;
}
```

1. A expressão `inicial` é inicializada e, caso possível, é executada
2. A expressão `condicao` é avaliada. Caso o resultado de `condicao` seja verdadeiro, o laço é executado
3. As `instruções` são executadas
4. A atualização da expressão `incremento`, se houver, executa, e retorna para o passo 2.

---

## For

- Mostrar na tela 10 vezes o seu nome

```javascript
for (var contador = 0; contador < 10; contador++) {
  document.write("Fabricio<br>");
}
```

- Mostrar na tela todos os números pares de 2 a 100

```javascript
for (var numero = 2; numero <= 100; numero = numero + 2) {
  document.write(numero + "<br>");
}
```

---

## For

- Mostrar na tela a soma de 1 até n, em que n é informado pelo usuário

```javascript
var n, soma = 0;
n = parseInt(prompt("Digite o número n"));
for (var i = 1; i <= n; i++) {
  soma = soma + i;
}
document.write("Soma: " + soma);
```

---

## While

```javascript
while (condicao) {
  instrucoes;
}
```
- Enquanto a `condicao` for avaliada como verdadeira, execute as `instrucoes`

---

## While

- Mostrar na tela 10 vezes o seu nome

```javascript
var contador = 0;
while (contador < 10) {
  document.write("Fabricio<br>");
  contador++;
}
```

---

## While

- Mostrar na tela todos os números pares de 2 a 100

```javascript
var numero = 2;
while (numero <= 100) {
  document.write("Fabricio<br>");
  numero = numero + 2;
}
```

---

## While

- Mostrar na tela a soma de 1 até n, em que n é informado pelo usuário

```javascript
var n, i = 1, soma = 0;
n = parseInt(prompt("Digite o número n"));
while (i <= n) {
  soma = soma + i;
  i++;
}
document.write("Soma: " + soma);
```

- Por sua atuação, `soma` pode também ser chamada de **acumuladora**

---

## Do-while

- Semelhante ao `while`, mas executa as instruções uma vez antes de avaliar a `condicao`

```javascript
do {
  instruções;
} while (condicao);
```

---

## Do-While

- Fazer o usuário digitar um valor entre 1 e 6

```javascript
var num;
do {
  num = parseInt(prompt("Digite um valor entre 1 e 6"));
} while (num < 1 || num > 6);
document.write(num);
```

---

## Interrompendo uma Estrutura de Repetição

- Uma estrutura de repetição pode ser interrompida a qualquer momento utilizando-se as instruções `break` ou `return`
- Exemplo: saber se um determinado número é primo
```javascript
var num = parseInt(prompt("Digite um número"));
for (var i = 2; i < num; i++) {
  if (num % i == 0) {
    document.write("O número " + num + " não é primo!");
    break;
  }
}
```

---

## Reiniciando uma Estrutura de Repetição

- A instrução `continue` permite reiniciar uma estrutura de repetição, seja ela um `for`, `while` ou `do-while`
- Exemplo: exibir apenas os números pares de 1 a 10
```javascript
for (var num = 1; num <= 10; num++) {
  if (num % 2 == 1) {
    continue;
  }
  document.write(num + "<br>");
}
```

