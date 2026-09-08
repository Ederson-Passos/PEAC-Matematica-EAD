---
marp: true
theme: default
math: mathjax
size: 16:9
style: |
  @import url('https://fonts.googleapis.com/css2?family=Libre+Baskerville&display=swap');

  section {
    background-color: #000000;
    color: #E0E0E0;
    font-family: 'Libre Baskerville', serif;
    font-size: 26px;
    padding: 30px 50px;
    background-image: radial-gradient(#444444 1px, transparent 1px);
    background-size: 30px 30px;
    background-position: 0 0;
  }

  section::after {
    content: "";
    display: block;
    position: absolute;
    bottom: 20px;
    right: 30px;
    width: 100px;
    height: 50px;
    background-image: url('logo-peac.png');
    background-size: contain;
    background-repeat: no-repeat;
    background-position: right bottom;
    opacity: 0.6;
  }

  h1 {
    color: #8BE9FD;
    font-size: 30px;
    margin-bottom: 5px;
    border-bottom: 1px solid #444444;
    padding-bottom: 5px;
  }

  h2 {
    color: #F8F8F2;
    font-size: 22px;
    font-weight: normal;
  }

  .content-wrapper {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    gap: 20px;
    margin-top: 5px;
  }

  .theory {
    flex: 1.3;
    line-height: 1.3;
  }

  .resolution {
    flex: 1;
    border-left: 1px solid #444444;
    height: 520px;
    padding-left: 20px;
    color: #444444;
    font-size: 18px;
  }

  .example-box {
    background-color: rgba(139, 233, 253, 0.05);
    border-left: 3px solid #8BE9FD;
    padding: 10px 15px;
    margin-top: 10px;
    font-size: 20px;
  }

  .center { text-align: center; }
  
  table {
    width: 100%;
    border-collapse: collapse;
    margin-top: 15px;
    color: #E0E0E0;
  }
  th, td {
    border: 1px solid #444444;
    padding: 8px;
    text-align: left;
  }
  th {
    background-color: #1a1a1a;
    color: #8BE9FD;
  }

---
<div class="center">

# Matemática Pré-Vestibular
## AULA 12 - Probabilidade e Estatística


*(Aguardando o início da transmissão)*
</div>

---

# 1. Probabilidade Clássica

<div class="content-wrapper">
<div class="theory">

A Probabilidade clássica mede a chance de ocorrência de um evento em um cenário onde todos os resultados possíveis têm a mesma probabilidade de acontecer (espaço amostral equiprovável).

A fórmula fundamental, proposta por Laplace, é a razão entre o número de resultados favoráveis e o número total de resultados possíveis:

$$\Large P(E) = \frac{n(E)}{n(\Omega)} = \frac{\text{casos favoráveis}}{\text{casos possíveis}}$$

* $P(E)$: Probabilidade de ocorrer o evento $E$.
* $n(\Omega)$: Número de elementos do espaço amostral $\Omega$.

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 1.1 Exemplo: Probabilidade Clássica

<div class="content-wrapper">
<div class="theory">

Lembre-se: A probabilidade sempre será um valor entre $0$ (evento impossível) e $1$ (evento certo), ou de $0\%$ a $100\%$.

<div class="example-box">

**Exemplo 01:** Lançando um dado perfeito não viciado de 6 faces, qual a probabilidade de obtermos um número maior ou igual a 5?
</div>

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 2. Probabilidade Condicional e Eventos Independentes

<div class="content-wrapper">
<div class="theory">

**Eventos Independentes:** A ocorrência de um evento não afeta a probabilidade do outro. Quando precisamos que dois eventos ocorram **simultaneamente** (regra do "E"), multiplicamos suas probabilidades.
$$\Large P(A \cap B) = P(A) \cdot P(B)$$

**Probabilidade Condicional:** Trata-se da probabilidade de um evento $A$ ocorrer sabendo que um evento $B$ já ocorreu. Isso significa que o espaço amostral original ($\Omega$) é reduzido para o conjunto $B$.

$$\Large P(A|B) = \frac{P(A \cap B)}{P(B)}$$

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 2.1 Exemplo: Probabilidade Condicional

<div class="content-wrapper">
<div class="theory">

Reduzir o espaço amostral é a chave para a probabilidade condicional. Ao invés de olhar para todas as possibilidades, olhamos apenas para as possibilidades que satisfazem a condição dada.

<div class="example-box">

**Exemplo 02:** De um baralho com 52 cartas, retira-se uma carta. Sabendo que a carta retirada é de paus, qual a probabilidade de que seja um "Ás"?
</div>

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 3. Estatística: Média Aritmética Simples e Ponderada

<div class="content-wrapper">
<div class="theory">

A estatística descritiva resume conjuntos de dados. A principal medida de tendência central é a média.

**Média Aritmética Simples ($\bar{x}$):** É o quociente entre a soma de todos os valores de um conjunto e a quantidade total de valores.
$$\Large \bar{x} = \frac{x_1 + x_2 + \dots + x_n}{n}$$

**Média Aritmética Ponderada ($\bar{x}_p$):** Utilizada quando os valores possuem "pesos" diferentes.
$$\Large \bar{x}_p = \frac{x_1 p_1 + x_2 p_2 + \dots + x_n p_n}{p_1 + p_2 + \dots + p_n}$$

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 3.1 Exemplo: Média Aritmética Ponderada

<div class="content-wrapper">
<div class="theory">

Muitas vezes, lidamos com dados que estão agrupados em tabelas de frequência. Nesses casos, a frequência funciona como um "peso" para cada valor.

<div class="example-box">

**Exemplo 03:** Um aluno tirou notas 6 e 8 em duas provas com pesos 2 e 3, respectivamente. Qual a média final dele?
</div>

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 4. Estatística: Mediana e Moda

<div class="content-wrapper">
<div class="theory">

**Mediana (Md):** É o valor central de um conjunto de dados ordenados (em ordem crescente ou decrescente). Ela divide o conjunto exatamente ao meio.
* Se a quantidade de dados for **ímpar**, a mediana é o elemento central.
* Se a quantidade de dados for **par**, a mediana é a média aritmética dos dois elementos centrais.

**Moda (Mo):** É o valor (ou valores) que aparece com maior frequência no conjunto de dados. Um conjunto pode ser amodal (não tem moda) ou multimodal (várias modas).

<div class="example-box">

**Exemplo 04:** Encontre a mediana e a moda das idades de um grupo de jovens: $\{15, 17, 15, 18, 20\}$.
</div>

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 5. UFRGS 2025

<div class="content-wrapper">
<div class="theory" style="font-size: 19px;">

Doze pontos estão dispostos de modo equidistante em uma circunferência, como mostrado na figura abaixo. A probabilidade de escolher aleatoriamente três pontos distintos, os quais sejam vértices de um triângulo equilátero, é:

<div style="text-align: center; margin-top: 10px; margin-bottom: 5px;">
<svg viewBox="-50 -50 100 100" width="180">
  <circle cx="0" cy="0" r="40" stroke="#E0E0E0" stroke-width="1.5" fill="none" />
  <circle cx="0" cy="40" r="2.5" fill="#8BE9FD" />
  <circle cx="20" cy="34.64" r="2.5" fill="#8BE9FD" />
  <circle cx="34.64" cy="20" r="2.5" fill="#8BE9FD" />
  <circle cx="40" cy="0" r="2.5" fill="#8BE9FD" />
  <circle cx="34.64" cy="-20" r="2.5" fill="#8BE9FD" />
  <circle cx="20" cy="-34.64" r="2.5" fill="#8BE9FD" />
  <circle cx="0" cy="-40" r="2.5" fill="#8BE9FD" />
  <circle cx="-20" cy="-34.64" r="2.5" fill="#8BE9FD" />
  <circle cx="-34.64" cy="-20" r="2.5" fill="#8BE9FD" />
  <circle cx="-40" cy="0" r="2.5" fill="#8BE9FD" />
  <circle cx="-34.64" cy="20" r="2.5" fill="#8BE9FD" />
  <circle cx="-20" cy="34.64" r="2.5" fill="#8BE9FD" />
</svg>
</div>

(A) $\dfrac{1}{12}$ &nbsp;&nbsp;&nbsp;&nbsp; (B) $\dfrac{1}{39}$ &nbsp;&nbsp;&nbsp;&nbsp; (C) $\dfrac{1}{55}$ &nbsp;&nbsp;&nbsp;&nbsp; (D) $\dfrac{1}{110}$ &nbsp;&nbsp;&nbsp;&nbsp; (E) $\dfrac{1}{220}$

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 6. UFRGS 2024

<div class="content-wrapper">
<div class="theory" style="font-size: 20px;">

Em uma urna, estão depositados cartões retangulares de papel com todos os anagramas possíveis de serem formados com quatro letras, considerando as letras R, O, M, A, utilizando todas exatamente uma vez. Cada cartão contém um único anagrama e todos os cartões são do mesmo tamanho e peso. Retirando de forma aleatória um cartão da urna, considere $p$ a probabilidade de estar escrito nesse cartão o anagrama AMOR.

Dadas essas condições, pode-se afirmar que:

<br><br>

(A) $p \le 5\%$ <br>
(B) $5\% < p \le 20\%$ <br>
(C) $20\% < p \le 25\%$ <br>
(D) $25\% < p \le 30\%$ <br>
(E) $p > 30\%$

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 7. UFRGS 2021

<div class="content-wrapper">
<div class="theory" style="font-size: 18px;">

A tabela a seguir mostra o tempo de uso diário de um dispositivo eletrônico por um aluno, durante cinco dias da semana com aulas a distância, em sua escola, no ano de 2021.

| Dia da semana | Tempo (em minutos) |
| :--- | :---: |
| Segunda-feira | 240 |
| Terça-feira | 180 |
| Quarta-feira | 180 |
| Quinta-feira | 240 |
| Sexta-feira | 120 |

Nessas condições, o tempo médio diário de uso do dispositivo eletrônico por esse aluno é:

<br>

(A) superior a três horas. <br>
(B) superior a quatro horas. <br>
(C) superior a cinco horas. <br>
(D) inferior a duas horas. <br>
(E) inferior a três horas.

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 8. UFRGS 2023

<div class="content-wrapper">
<div class="theory" style="font-size: 22px;">

Considere uma moeda não viciada tendo uma face cara e uma face coroa. Ao lançar essa moeda cinco vezes, a probabilidade de se obter **pelo menos** três faces coroa é:

<br>

(A) $\dfrac{1}{8}$ <br>
(B) $\dfrac{1}{6}$ <br>
(C) $\dfrac{1}{5}$ <br>
(D) $\dfrac{1}{4}$ <br>
(E) $\dfrac{1}{2}$

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 9. UFRGS 2024

<div class="content-wrapper">
<div class="theory" style="font-size: 21px;">

A média harmônica de dois números positivos $a$ e $b$ é calculada pela relação $M_H = \dfrac{2}{\frac{1}{a} + \frac{1}{b}}$.

Considerando essa informação, a média harmônica ($M_H$) das raízes da equação $x^2 - 5x + 6 = 0$ é:

<br><br>

(A) 1,6. <br>
(B) 2,0. <br>
(C) 2,4. <br>
(D) 2,8. <br>
(E) 3,2.

</div>
<div class="resolution">Resolução:</div>
</div>

---