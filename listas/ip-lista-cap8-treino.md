
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
Atividade: Lista de Exercícios nº 06
      </td>
    </tr>
  </tbody>
</table>

# Lista de Exercícios 06 – Estruturas de Repetição

## Objetivo

O objetivo desta lista de exercícios é exercitar o estudante na linguagem de programação JavaScript.

## Exercícios

1. [Impares] Desenvolva um programa que solicite um número inteiro n e exiba em uma única linha, todos os números ímpares entre 1 até n e a soma destes números. Exemplo: se o usuário informar o número n = 10, o programa deverá exibir como resposta "1 + 3 + 5 + 7 + 9 = 25".

2. [Multiplos] Desenvolva um programa que solicite dois números inteiros a e b e mostre os números múltiplos de 3 e múltiplos de 5 entre a e b inclusive. Por exemplo, se forem informados os números a = 3 e b = 11, o programa deverá exibir que os múltiplos de 3 são 3, 6 e 9 e os múltiplos de 5 são 5 e 10.

3. [Somatorio] Desenvolva um programa que dado um número inteiro n, calcule o somatório de 1 até n (1 + 2 + 3 + .... + n). Exemplo, se o usuário informar o número 5, o programa calculará 1 + 2 + 3 + 4 + 5 e mostrará como resposta o número 15.

4. [Fatorial] Desenvolva um programa que dado um número inteiro n, calcule o fatorial de n (1 . 2 . 3 . ... . n). Exemplo, se o usuário informar o número 5, o programa calculará 1 . 2 . 3 . 4 . 5 e mostrará como resposta o número 120. Observação: lembrar que o fatorial de 0 é igual a 1.

5. [Pontuacao] Em um determinado jogo, a maior pontuação que uma pessoa pode obter são 100 pontos e a menor 0 ponto. Com base nesta informação, desenvolva um programa que solicite a pontuação de 200 jogadores e depois informe a maior e a menor pontuação obtidas entre estes jogadores.

6. [Potencia] Desenvolva um programa que calcule x<sup>n</sup>, sendo x e n dois números naturais (não usar funções matemáticas para isto). Exemplo: para x = 2 e n = 3, a saída deverá ser 8 (pois 2<sup>3</sup> = 8). Observação: lembre-se que x<sup>0</sup> = 1 e que 0<sup>0</sup> é uma indeterminação.

7. [Primo] Desenvolva um programa que um número inteiro não-negativo p, verificar se p é primo ou não. Observação: Um número é dito primo se este número só puder ser dividido por um número inteiro que seja 1 ou ele mesmo (o próprio p). Exemplo: 11 é primo (pois só é divisível por 1 e por 11), mas 12 não é (é divisível por 2, 3, 4 e 6).

8.  [Tabuada] Desenvolva um programa de computador que solicite um número inteiro e mostre a tabuada deste número. Observação: a solução dessa questão deve utilizar uma estrutura de repetição.

9.  [MenuNotas] Desenvolva um programa que exiba um menu com as opções: 1 - Média, 2 – Nota para a Final, 3 – Média Ponderada e 0 - Sair. Após o usuário escolher a opção, o programa deverá executar a operação escolhida, exibir o resultado desta operação e retornar novamente ao menu, para que o usuário possa escolher uma nova opção. No entanto, se o usuário escolha a opção 0 (Sair), o programa deverá ser encerrado. Observação: assuma que:
    - só há duas notas para calcular as médias;
    - a média do curso é 6,0;
    - no caso da média ponderada, os respectivos pesos de cada nota são 6 e 4.

10. [Palitinhos] O jogo dos palitinhos funciona da seguinte maneira:
    1.  cada jogador possui três palitinhos;
    2.  cada jogador apresenta numa mão fechada, uma quantidade aleatória entre zero e três palitos;
    3.  cada jogador deve informar, de maneira única, a soma de todos os palitos apresentados;
    4.  ganha quem acertar o soma dos palitos contidos nas mãos de todos os jogadores em três rodadas.

    De posse destas instruções, desenvolva o jogo dos palitinhos. Observação: para gerar um número aletaório entre `min` e `max` em JavaScript é feito seguindo a seguinte fórmula: `Math.floor(Math.random() * (max - min + 1)) + min`
