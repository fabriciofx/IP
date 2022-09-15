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

## Capítulo 2 - Introdução ao Algoritmo

---

## Algoritmo

- Conjunto de instruções **ordenadas** e **não ambíguas** utilizadas para **resolver um determinado problema** em **tempo hábil**
  - Ordenada: a ordem das instruções pode influenciar no resultado
  - Não ambígua: as instruções têm de ser claras e objetivas; não podem dar margem a dúvidas ou incertezas
  - Resolver um determinado problema: de quê adianta um algoritmo que não resolve corretamente o problema proposto?
  - Tempo hábil: o algoritmo precisa encontrar a solução em um tempo finito. Não serve se demorar 100 anos para solucionar

---

## Utilização do Algoritmo

- O algoritmo deverá ser desenvolvido por um programador e este será executado pelo computador
- Imagine que as instruções do algoritmo são ordens que deverão ser dadas ao computador e ele (o computador) é que as executará

---

## Etapas do Desenvolvimento

1. **Análise**
   Estudo do problema e de como resolvê-lo (definição dos dados de entrada, processamento e saída dos dados)
2. **Elaboração do Algoritmo**
   Aplicação de ferramentas para descrição do problema e sua solução
3. **Verificação**
   Verificação se o algoritmo resultante soluciona o problema proposto

---

## Etapas do Desenvolvimento

4. **Codificação**
   Transformação do algoritmo em instruções de uma linguagem de programação

---

## Etapas do Desenvolvimento (Exemplo 1)

-  Problema: Um professor do Curso Técnico em Informática do IFPE deseja utilizar um computador para lhe auxiliar no cálculo da média de cada estudante em uma disciplina

---

## 1. Análise (Exemplo 1)

- A forma de calcular a média é a mesma para todos os estudantes e disciplinas?
  - Sim
- Que tipo de média é esta?
  - Média aritmética
- Quantas avaliações existem?
  - Duas – Unidade 1 e Unidade 2 (estamos simplificando!)
  - Uma nota para cada avaliação (estamos simplificando!)

---

## 1. Análise (Exemplo 1)

- Quais são os dados necessários para calcular a média?
  - A quantidade de notas (duas notas) e os seus respectivos valores (nota1 e nota2)

---

## 2. Elaboração do Algoritmo (Exemplo 1)

  1. Solicite na tela que o usuário digite a 1ª nota.
  2. Leia do teclado a 1ª nota que o usuário digitar e guarde-a.
  3. Solicite na tela que o usuário digite a 2ª nota.
  4. Leia do teclado a 2ª nota que o usuário digitar e guarde-a.
  5. Some as duas notas, divida por dois, e guarde este resultado.
  6. Mostre na tela o resultado obtido no passo 5.

---

## 3. Verificação (Exemplo 1)

- Se o usuário informar os valores (notas) 6,0 e 8,0 o resultado (média) será de 7,0?
- Se o usuário informar os valores (notas) 0,0 e 0,0 o resultado (média) será de 0,0
- Se o usuário informar os valores (notas) -6,0 e 8,0 o resultado (média) será de quanto?

---

## 4. Codificação (Exemplo 1)

```javascript
// 0. Declarar as variáveis
var nota1Str, nota2Str, nota1, nota2, media;
// 1. Solicite na tela que o usuário digite a 1ª nota.
// 2. Leia do teclado a 1ª nota que o usuário digitar e guarde-a.
nota1Str = prompt("Digite a 1a nota");
nota1 = parseFloat(nota1Str);
// 3. Solicite na tela que o usuário digite a 2ª nota.
// 4. Leia do teclado a 2ª nota que o usuário digitar e guarde-a.
nota2Str = prompt("Digite a 2a nota");
nota2 = parseFloat(nota2Str);
// 5. Some as duas notas, divida por dois, e guarde este resultado.
media = (nota1 + nota2) / 2;
// 6. Mostre na tela o resultado obtido no passo 5.
document.write("Media: " + media);
```

---

## Pra Pensar em Casa depois da Novela!

- E se o professor quisesse calcular a média de uma disciplina que teve três avaliações?
- E se fossem 10 avaliações? E se fossem 50?
- E se eu não soubesse, previamente, a quantidade de notas?
- E se a forma de calcular a média mudasse (média ponderada, média harmônica, etc)?

---

## Etapas do Desenvolvimento (Exemplo 2)

- Um professor do Curso Técnico em Informática do IFPE deseja utilizar um computador para lhe auxiliar no cálculo da média de cada estudante em uma disciplina em que houve **três** avaliações

---

## 1. Análise (Exemplo 2)

- A forma de calcular a média é a mesma para todos os estudantes e disciplinas?
  - Sim (obviamente, estamos simplificando!)
- Que tipo de média é esta?
  - Média aritmética (estamos simplificando!)
- Quantas avaliações existem?
  - Três – Unidade 1, Unidade 2 e Unidade 3
  - Uma nota para cada avaliação (estamos simplificando!)

---

## 1. Análise (Exemplo 2)

- Quais são os dados necessários para calcular a média?
  - A quantidade de notas (três notas) e os seus respectivos valores (nota1, nota2 e nota3)

---

## 2. Elaboração do Algoritmo (Exemplo 2)

  1. Solicite na tela que o usuário digite a 1ª nota.
  2. Leia do teclado a 1ª nota que o usuário digitar e guarde-a.
  3. Solicite na tela que o usuário digite a 2ª nota.
  4. Leia do teclado a 2ª nota que o usuário digitar e guarde-a.
  5. Solicite na tela que o usuário digite a 3ª nota.
  6. Leia do teclado a 3ª nota que o usuário digitar e guarde-a.
  7. Some as três notas, divida por três, e guarde este resultado.
  8. Mostre na tela o resultado obtido no passo 7.

---

## 3. Verificação (Exemplo 2)

- Se o usuário informar os valores (notas) 6,0, 8,0 e 7,0 o resultado (média) será de 7,0?
- Se o usuário informar os valores (notas) 0,0, 0,0 e 3,0 o resultado (média) será de 1,0?
- Se o usuário informar os valores (notas) -6,0 e 8,0 e 7,0 o resultado (média) será de quanto?

---

## 4. Codificação (Exemplo 1)

```javascript
var nota1Str, nota2Str, nota3Str, nota1, nota2, nota3, media;
nota1Str = prompt("Digite a 1a nota");
nota1 = parseFloat(nota1Str);
nota2Str = prompt("Digite a 2a nota");
nota2 = parseFloat(nota2Str);
nota3Str = prompt("Digite a 3a nota");
nota3 = parseFloat(nota3Str);
media = (nota1 + nota2 + nota3) / 3;
document.write("Media: " + media);
```

---

## Etapas do Desenvolvimento (Exemplo 3)

Problema: Um professor do Curso Técnico em Informática do IFPE deseja utilizar um computador para lhe auxiliar a determinar se um estudante está aprovado ou reprovado em uma disciplina

---

## 1. Análise (Exemplo 3)

- Quando um estudante está aprovado ou reprovado
  - Um estudante está aprovado se a sua média for maior ou igual que a **média de aprovação** (estamos simplificando!)
  - A média de aprovação é 6,0
- Que tipo de média é esta?
  - Média aritmética (estamos simplificando!)

---

## 1. Análise (Exemplo 3)

- Quantas avaliações existem?
  - Duas – Unidade 1 e Unidade 2
  - Uma nota para cada avaliação (estamos simplificando!)
- Quais são os dados necessários para calcular a média?
  - A quantidade de notas (duas notas) e os seus respectivos valores (nota1 e nota2) e a média de aprovação (6,0)

---

## 2. Elaboração do Algoritmo (Exemplo 3)

  1. Solicite na tela que o usuário digite a 1ª nota.
  2. Leia do teclado a 1ª nota que o usuário digitar e guarde-a.
  3. Solicite na tela que o usuário digite a 2ª nota.
  4. Leia do teclado a 2ª nota que o usuário digitar e guarde-a.
  5. Some as duas notas, divida por dois, e guarde este resultado na média.
  6. *Se* a média obtida for maior ou igual a 6,0
  6.1. *Então* informe na tela que o estudante está aprovado.
  6.2. *Senão* informe na tela que o estudante está reprovado.

---

## 3. Verificação (Exemplo 3)

- Se o usuário informar os valores (notas) 6,0 e 6,0 o estudante está aprovado ou reprovado?
- Se o usuário informar os valores (notas) 0,0 e 0,0 o estudante está aprovado ou reprovado?
- Se o usuário informar os valores (notas) 6,0 e 5,0 o estudante está aprovado ou reprovado?
- Se o usuário informar os valores (notas) 6,0 e 8,0 o estudante está aprovado ou reprovado?

---

## 3. Verificação (Exemplo 3)

- Se o usuário informar os valores (notas) 5,0 e 8,0 o estudante está aprovado ou reprovado?
- Se o usuário informar os valores (notas) -8,0 e 6,0 o estudante está aprovado ou reprovado?

---

## 4. Codificação (Exemplo 3)

```javascript
var nota1Str, nota2Str, nota1, nota2, media;
nota1Str = prompt("Digite a 1a nota");
nota1 = parseFloat(nota1Str);
nota2Str = prompt("Digite a 2a nota");
nota2 = parseFloat(nota2Str);
media = (nota1 + nota2) / 2;
if (media >= 6.0) {
  document.write("O estudante esta aprovado");
} else {
  document.write("O estudante esta reprovado");
}
```

---

# Símbolos Aritméticos

- Operações aritméticas básicas

| Operador | Operação         |
|----------|------------------|
|    +     | Adição           |
|    -     | Subtração        |
|    *     | Multiplicação    |
|    /     | Divisão          |
|    %     | Resto da divisão |

---

## Etapas do Desenvovimento (Exemplo 4)

- Problema: Uma loja de venda de computadores deseja utilizar o computador para lhe auxiiar no cálculo do preço final de um computador. Para efetuar este cálculo, assuma que 45% é relativo ao imposto e o lucro na área é de 15%.
  - Observação: no Brasil, paga-se o imposto ANTES de vender o produto. Assim o lucro deve ser calculado com base no preço de compra e do imposto pago.

---

## 1. Análise (Exemplo 4)

- O que é o preço de fábrica?
  - É quanto custa o computador quando a loja adquire da fábrica
- Como calcular o imposto?
  - O imposto é calculado em 45% com relação ao preço de fábrica
- Como calcular o lucro?
  - No Brasil, como o imposto é pago ANTES da venda, então deve-se calcular os 15% do lucro com relação ao preço de fábrica E do imposto

---

## 1. Análise (Exemplo 4)

- Como eu calculo uma porcentagem?
  - Diferente de uma calculadora, não existe a operação “%”. Esta deve ser calculada da seguinte forma:
    - ValorDoPercentual = Valor * Percentual / 100
    - ValorDoPercentual = Valor * 0.Percentual
  - Também é possível já calcular um determinado valor acrescido de um percentual
    - ValorFinal = Valor + Valor * 0.Percentual
    - ValorFinal = Valor * 1.Percentual

---

## 1. Análise (Exemplo 4)

- Como eu calculo uma porcentagem?
  - Também é possível já calcular um determinado valor descontado um valor percentual
    - ValorFinal = Valor - Valor * 0.Percentual
    - ValorFinal = Valor * (1 - 0.Percentual)

---

## 2. Elaboração do Algoritmo (Exemplo 4)

1. Solicite na tela para que o usuário digite o preço de fábrica.
2. Leia do teclado o preço de fábrica que o usuário digitar e guarde-o.
3. Pegue o preço de fábrica, multiplique por 0.45 (45%) e guarde o resultado.
4. Pegue o preço de fábrica, some com o resultado do passo 3 e multiplique por 0.15 (15%) e guarde o resultado.
5. Some ao preço de fábrica os resultados obtidos nos passo 3 e 4 e guarde este resultado.
6. Mostre na tela o resultado obtido no passo 5.

---

## 3. Verificação (Exemplo 4)

- Se o preço de fábrica do computador for de R$ 1.000,00, o preço final será de R$ 1.667,50?
- Se o preço de fábrica do computador for de R$ 1.500,00, o preço final será de R$ 2.501,25?

---

## 4. Codificação (Exemplo 4)

```javascript
var precoFabricaStr, precoFabrica, imposto, lucro, precoFinal;
precoFabricaStr = prompt("Digite o preço de fábrica");
precoFabrica = parseFloat(precoFabricaStr);
imposto = precoFabrica * 0.45;
lucro = (precoFabrica + imposto) * 015;
precoFinal = precoFabrica + imposto + lucro;
document.write("Preço Final:" + precoFinal);
```

---

## 1. Análise (Exemplo 5)

- Problema: em um jogo de computador o personagem recolhe vários itens que aumentam a pontuação no final de cada fase. Cada item A aumenta a pontuação em 35%, o item B em 20%, e o item C em 10%. Com esta informação, desenvolva um algoritmo e compute a pontuação final de acordo com a quantidade de itens recolhidos

---

## 2. Elaboração do Algoritmo (Exemplo 5)

1. Solicite na tela para que o usuário digite a pontuação da fase
2. Leia do teclado a pontuação da fase que o usuário digitar e guarde-a
3. Solicite na tela a quantidade de itens do tipo A
4. Leia do teclado a quantidade de itens do tipo A que o usuário digitar e guarde-a
5. Solicite na tela a quantidade de itens do tipo B
6. Leia do teclado a quantidade de itens do tipo B que o usuário digitar e guarde-a

---

## 2. Elaboração do Algoritmo (Exemplo 5)

7. Solicite na tela a quantidade de itens do tipo C
8. Leia do teclado a quantidade de itens do tipo C que o usuário digitar e guarde-a
9. Multiplique a pontuação da fase com 0.35 (35%) e multiplique pela quantidade de itens do tipo A e guarde este resultado
10. Multiplique a pontuação da fase com 0.20 (20%) e multiplique pela quantidade de itens do tipo B e guarde este resultado
11. Multiplique a pontuação da fase com 0.10 (10%) e multiplique pela quantidade de itens do tipo C e guarde este resultado

---

## 2. Elaboração do Algoritmo (Exemplo 5)

12. Some a pontuação da fase como resultado dos passos 9, 10 e 11
13. Mostre na tela o resultado obtido do passo 12

---

## 3. Verificação (Exemplo 5)

- Se a pontuação da fase for 100 pontos, e o personagem tiver recolhido 2 itens do tipo A, 1 item do tipo B e 0 item do tipo C, a pontuação total da fase será de 190 pontos?

---

## 4. Codificação (Exemplo 5)


```javascript
var PFStr, AStr, BStr, CStr, PF, A, B, C, PT, PIA, PIB, PIC;
PFStr = prompt("Digite a pontuação da fase");
PF = parseFloat(PFStr);
AStr = prompt("Digite a quant. de itens A");
A = parseFloat(AStr);
BStr = prompt("Digite a quant. de itens B");
B = parseFloat(BStr);
CStr = prompt("Digite a quant. de itens C");
C = parseFloat(CStr);
PIA = PF * 0.35 * A;
PIB = PF * 0.20 * B;
PIC = PF * 0.10 * C;
PT = PF + PIA + PIB + PIC;
document.write(”Pontuação Total da Fase: " + PT);
```



