
<table>
  <thead>
  </thead>
  <tbody>
    <tr>
      <td>
        <img src="logotipo-ead-mini.png">
      </td>
      <td>
IFPE – Instituto Federal de Pernambuco | Campus Paulista<br/>
Curso: Análise e Desenvolvimento de Sistemas<br/>
Professor: Fabrício Cabral <fabricio.cabral@ead.ifpe.edu.br><br/>
Disciplina: Introdução à Programação<br/>
Atividade: Lista de Exercícios nº 05
      </td>
    </tr>
  </tbody>
</table>

# Lista de Exercícios 05 – Operadores Lógicos

## Objetivo

O objetivo desta lista de exercícios é exercitar o estudante na linguagem de programação JavaScript.

## Exercícios

1. [RevendaPneus] Para estimular as vendas por parte dos seus vendedores, uma revenda de pneus da cidade está oferecendo o seguinte estímulo: se um vendedor, durante o mês, vender até 15 pneus, ganhará um bônus de 6% do salário; se vender entre 16 a 25 pneus, ganhará um bônus de 9% do salário, se vender entre 26 e 45 pneus, ganhará um bônus de 15% do salário e se vender acima de 45 pneus, ganhará, além de um bônus de 20% do salário, mais R$ 300,00. Assim, desenvolva um programa que informado o salário de um vendedor e a quantidade de pneus vendidos por este durante o mês, mostre quanto ele irá ganhar no final do mês.

2. [PromocaoPosto] Um posto está vendendo combustíveis com a seguinte tabela de descontos:
   
   | Combustível | Preços  | Descontos                                                                            |
   |-------------|---------|--------------------------------------------------------------------------------------|
   | Álcool      | R$ 4,75 | Até 20 litros, desconto de 3% por litro acima de 20 litros, desconto de 5% por litro |
   | Gasolina    | R$ 5,45 | Até 20 litros, desconto de 4% por litro acima de 20 litros, desconto de 6% por litro |
   
   De posse destas informações, escreva um programa que solicite ao usuário que tipo de combustível (sugestão: faça o usuário digitar o número 1 para o álcool e 2 para a gasolina) e a quantidade de combustível (em litros) e exiba o valor total a ser pago.

3. [DescontoLoja] Uma loja de Garanhuns-PE está oferecendo para os seus clientes a seguinte promoção: se o valor em compras for de até R$ 150,00, será oferecido um desconto de 3%; se o valor for maior que R$ 150,00 e menor ou igual a R$ 250,00 o desconto será de 5%; se o valor for acima de R$ 250,00 e menor ou igual a R$ 350,00 o desconto será de 10%; e se o valor for acima de R$ 350,00 o desconto será de 15%. Assim, desenvolva um programa que mostre o valor (em reais) da compra, o valor (em reais) deste desconto, e o valor final (em reais) que o cliente deverá pagar.

4. [Conceito] Em uma universidade, as médias são atribuídas por conceitos, de acordo com a tabela abaixo:
   
   | Conceito | Faixa de média correspondente |
   |----------|-------------------------------|
   |    A     | Entre 9,0 e 10,0              |
   |    B     | Entre 7,0 e 8,9               |
   |    C     | Entre 5,0 e 6,9               |
   |    D     | Abaixo de 5,0                 |

   Assim, sabendo que em qualquer disciplina há duas avaliações e que a média é calculada utilizando-se média aritmética simples, desenvolva um programa que informe qual o conceito a ser atribuído a um estudante desta universidade, em uma disciplina qualquer.

5. [DescontoIR] Desenvolva um programa para efetuar o cálculo do salário líquido de um funcionário, que incide um desconto do Imposto de Renda (IR), que depende do valor do salário bruto, conforme tabela abaixo:
   
   | Desconto do IR                     | Porcentagem de desconto|
   |------------------------------------|------------------------|
   | Salário bruto de até R$ 1.212,00   | Isento                 |
   | Salário bruto de até R$ 1.700,00   | 5%                     |
   | Salário bruto de até R$ 3.500,00   | 10%                    |
   | Salário bruto acima de R$ 3.500,00 | 20%                    |

6. [IMC] O Índice de Massa Corpórea (IMC) é uma medida para determinar o peso saudável do corpo. Sabendo-se que para calcular o IMC de uma pessoa, basta dividir o seu peso (em quilogramas) por sua altura (em metros) ao quadrado, desenvolva um programa que calcule e informe o IMC de uma determinada pessoa e se ela está abaixo do peso, normal, com excesso de peso ou obesa, conforma a tabela abaixo:
   
   | IMC                    | Situação             |
   |------------------------|----------------------|
   | Inferior a 18,5        | Abaixo do peso ideal |
   | 18,5 a 24,9            | Peso normal          |
   | 25,0 a 29,9            | Excesso de peso      |
   | Igual ou superior a 30 | Obeso                |

7. [AlcoolOuGasolina] Com o surgimento dos carros bicombustíveis é possível escolher qual combustível utiliza, de acordo com o custo na bomba. Em geral é mais econômico abastecer o veículo com álcool quando o preço do litro for inferior a 70% do valor da gasolina. Sabendo desta informação, desenvolva um programa que solicite o preço do litro da gasolina e o preço do litro do álcool e informe qual combustível é mais econômico na hora de abastecer.

8. De acordo com as variáveis abaixo, desenvolva cada sentença (informando como chegou no resultado) abaixo e informe se o resultado será true (verdadeira) ou false (falsa):
   
   ```javascript
   var a = false, b = true, c = true, d = false, e = false, f = false, g = true;
   i.   (a && e) || (!d || !f)
   ii.  a && !b && c && !d && e && !f
   iii. !(!(a && b) || (!c || !d))
   iv.  !a || a && (b || c) && d || e && f
   v.   a || !b || !c || !d || !e && f
   ```

9. [Estacionamento] Construa um programa para calcular o valor a ser pago pelo período de estacionamento do automóvel. O usuário entra com os seguintes dados: hora e minuto de entrada, hora e minuto de saída. Sabe-se que este estacionamento cobra hora cheia, ou seja, se passar um minuto ele cobra a hora inteira. O valor cobrado pelo estacionamento é:
    - R$ 4,00 para 1 hora de estacionamento
    - R$ 6,00 para 2 horas de estacionamento
    - R$ 1,00 por hora adicional (acima de 2 horas)

10. [Calculadora] Desenvolva um programa que implemente uma calculadora capaz de realizar as 4 operações básicas (adição, subtração, multiplicação e divisão) entre dois números.
