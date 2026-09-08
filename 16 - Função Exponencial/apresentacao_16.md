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
    background-color: rgba(255, 255, 255, 0.03);
    border-radius: 8px;
    padding: 15px;
  }

  .resolution h3 {
    color: #AAAAAA;
    font-size: 20px;
    margin-top: 0;
    border-bottom: 1px dashed #444444;
    padding-bottom: 5px;
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

  .alt-table td {
    border: none !important;
    background: transparent !important;
    text-align: center;
    vertical-align: middle;
  }

  .svg-box {
    background: rgba(255,255,255,0.05);
    border-radius: 8px;
    padding: 10px;
    display: inline-block;
  }
  .flex-around {
    display: flex;
    justify-content: space-around;
    margin-top: 15px;
  }
  .crescente-text { color: #50fa7b; font-weight: bold; }
  .decrescente-text { color: #ff79c6; font-weight: bold; }
---
<div class="center">

# Matemática Pré-Vestibular
## AULA 16 - Equação Exponencial e Função Exponencial

*(Aguardando o início da transmissão)*
</div>

---

# 1. O que é uma Equação Exponencial?

<div class="content-wrapper">
<div class="theory" style="font-size: 20px;">

Uma equação é chamada de **exponencial** quando a nossa incógnita (o famoso $x$) está no expoente de pelo menos uma potência.

O princípio fundamental para resolver a esmagadora maioria dessas equações é a **Igualdade de Bases**. Se conseguirmos escrever ambos os lados da igualdade com a mesma base, os expoentes obrigatoriamente devem ser iguais:

$$
a^x = a^y \implies x = y \quad \text{(para } a > 0 \text{ e } a \neq 1\text{)}
$$

**Dica de Ouro:** A fatoração é a sua melhor amiga! Se você ver um $8$, transforme em $2^3$. Se ver um $81$, transforme em $3^4$. O objetivo é padronizar as bases.

</div>
<div class="resolution">
<h3> </h3>
</div>
</div>

---

# 1.1 Exemplo: Desmembrando Expoentes

<div class="content-wrapper">
<div class="theory">

Existem situações onde a base é a mesma, mas temos somas ou subtrações separando as potências. Nesses casos, usamos propriedades de potenciação (como desmembrar o expoente) e **colocamos o termo comum em evidência**.

<div class="example-box">

**Exemplo 01:** A equação abaixo exige que você aplique a propriedade $a^{m+n} = a^m \cdot a^n$ antes de fatorar. Resolva matematicamente:
$$2^{x+2} + 2^x = 20$$
Qual é o valor da incógnita $x$?

</div>

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 2. A Função Exponencial e a Análise da Base

<div class="content-wrapper">
<div class="theory" style="font-size: 21px;">

A **Função Exponencial** tem o formato $f(x) = a^x$ (com $a > 0$ e $a \neq 1$). Diferente de uma reta ou parábola, ela cresce ou decresce de forma vertiginosa. A curva sempre passa pelo ponto $(0, 1)$ e nunca toca o eixo $x$ (que atua como uma assíntota).

O comportamento gráfico depende exclusivamente do valor da **base ($a$)**:

<div class="flex-around">

<div class="center crescente-text">

Crescente ($a > 1$)

<div class="svg-box">
<img src="data:image/svg+xml;utf8,%3Csvg%20viewBox=%220%200%20200%20150%22%20width=%22180%22%20height=%22135%22%20xmlns=%22http://www.w3.org/2000/svg%22%3E%3Cdefs%3E%3Cmarker%20id=%22arrow1%22%20markerWidth=%2210%22%20markerHeight=%2210%22%20refX=%229%22%20refY=%223%22%20orient=%22auto%22%20markerUnits=%22strokeWidth%22%3E%3Cpath%20d=%22M0,0%20L0,6%20L9,3%20z%22%20fill=%22%23E0E0E0%22/%3E%3C/marker%3E%3C/defs%3E%3Cline%20x1=%2210%22%20y1=%22120%22%20x2=%22190%22%20y2=%22120%22%20stroke=%22%23E0E0E0%22%20stroke-width=%222%22%20marker-end=%22url(%23arrow1)%22/%3E%3Cline%20x1=%22100%22%20y1=%22140%22%20x2=%22100%22%20y2=%2210%22%20stroke=%22%23E0E0E0%22%20stroke-width=%222%22%20marker-end=%22url(%23arrow1)%22/%3E%3Cpath%20d=%22M%2010%20119.5%20C%2050%20118,%2080%20115,%20100%20100%20C%20120%2080,%20130%2050,%20140%2010%22%20fill=%22none%22%20stroke=%22%2350fa7b%22%20stroke-width=%223%22/%3E%3Ctext%20x=%22105%22%20y=%22105%22%20fill=%22%23E0E0E0%22%20font-size=%2212%22%3E1%3C/text%3E%3C/svg%3E">
</div>
</div>

<div class="center decrescente-text">

Decrescente ($0 < a < 1$)

<div class="svg-box">
<img src="data:image/svg+xml;utf8,%3Csvg%20viewBox=%220%200%20200%20150%22%20width=%22180%22%20height=%22135%22%20xmlns=%22http://www.w3.org/2000/svg%22%3E%3Cdefs%3E%3Cmarker%20id=%22arrow2%22%20markerWidth=%2210%22%20markerHeight=%2210%22%20refX=%229%22%20refY=%223%22%20orient=%22auto%22%20markerUnits=%22strokeWidth%22%3E%3Cpath%20d=%22M0,0%20L0,6%20L9,3%20z%22%20fill=%22%23E0E0E0%22/%3E%3C/marker%3E%3C/defs%3E%3Cline%20x1=%2210%22%20y1=%22120%22%20x2=%22190%22%20y2=%22120%22%20stroke=%22%23E0E0E0%22%20stroke-width=%222%22%20marker-end=%22url(%23arrow2)%22/%3E%3Cline%20x1=%22100%22%20y1=%22140%22%20x2=%22100%22%20y2=%2210%22%20stroke=%22%23E0E0E0%22%20stroke-width=%222%22%20marker-end=%22url(%23arrow2)%22/%3E%3Cpath%20d=%22M%2060%2010%20C%2070%2050,%2080%2080,%20100%20100%20C%20120%20115,%20150%20118,%20190%20119.5%22%20fill=%22none%22%20stroke=%22%23ff79c6%22%20stroke-width=%223%22/%3E%3Ctext%20x=%2285%22%20y=%22105%22%20fill=%22%23E0E0E0%22%20font-size=%2212%22%3E1%3C/text%3E%3C/svg%3E">
</div>
</div>

</div>
</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 3. Aplicações: O Crescimento Exponencial na Prática

<div class="content-wrapper">
<div class="theory" style="font-size: 20px;">

A função exponencial é o modelo perfeito para fenômenos que se multiplicam ao longo do tempo. É amplamente utilizada para calcular juros compostos, decaimento radioativo, desintegração de medicamentos e proliferação de bactérias.

O formato estrutural aplicado à ciência geralmente é:
$$N(t) = N_0 \cdot a^t$$
*(Onde $N_0$ é o valor inicial, $a$ é a taxa de crescimento/decaimento, e $t$ é o tempo).*

<div class="example-box">

**Exemplo 02 (Aplicação Matemática):** Uma colônia inicia com $100$ bactérias e seu número dobra a cada hora. O modelo matemático para a população é dado por $N(t) = 100 \cdot 2^t$. Em quanto tempo a colônia alcançará a marca de $3200$ bactérias?

</div>

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 4. UFRGS 2025:

<div class="content-wrapper">
<div class="theory" style="font-size: 19px;">

Considere as seguintes afirmações sobre números racionais.

**I.** Se $0 < a \le b$, então $b^a$ é sempre um número irracional.
**II.** Se $0 < a \le b$, então $0 < a \le \dfrac{a+b}{2} \le b$.
**III.** Se $0 < a < b < 1$, então $\log(a) < \log(b) < 0$.

Quais estão corretas?

(A) Apenas I.
(B) Apenas II.
(C) Apenas I e III.
(D) Apenas II e III.
(E) I, II e III.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 5. UFRGS 2025:

<div class="content-wrapper">
<div class="theory" style="font-size: 20px;">

A soma das raízes da equação $2^{x^2-3x-10} = 1$ é:

(A) $-3$.
(B) $-2$.
(C) $0$.
(D) $2$.
(E) $3$.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 6. UFRGS 2019:

<div class="content-wrapper">
<div class="theory" style="font-size: 19px;">

A concentração de alguns medicamentos no organismo está relacionada com a meia-vida, ou seja, o tempo necessário para que a quantidade inicial do medicamento no organismo seja reduzida pela metade.

Considere que a meia-vida de determinado medicamento é de 6 horas. Sabendo que um paciente ingeriu 120 mg desse medicamento às 10 horas, assinale a alternativa que representa a melhor aproximação para a concentração desse medicamento, no organismo desse paciente, às 16 horas do dia seguinte.

(A) 2,75 mg.
(B) 3 mg.
(C) 3,75 mg.
(D) 4 mg.
(E) 4,25 mg.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 7. UFRGS 2024:

<div class="content-wrapper">
<div class="theory" style="font-size: 19px;">

Considere as seguintes afirmações sobre números e suas operações.

**I.** A soma de dois números naturais consecutivos é sempre um número ímpar.
**II.** A soma de dois números irracionais é sempre um número irracional.
**III.** Se $a > 1$, então, para qualquer valor inteiro de $n$, $0 < \dfrac{1}{a^n} < 1$.

Quais estão corretas?

(A) Apenas I.
(B) Apenas III.
(C) Apenas I e II.
(D) Apenas II e III.
(E) I, II e III.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 8. UFRGS 2018:

<div class="content-wrapper">
<div class="theory" style="font-size: 17px;">

Considere a função real de variável real $f(x) = 2^{x-1}$. Com relação à $f(x)$, é correto afirmar que:

(A) se $x < 1$, então $f(x) < 0$.
(B) se $x \ge 1$, então $f(x) \le 1$.
(C) a função $f(x)$ é decrescente para $x < 0$ e crescente para $x \ge 0$.
(D) os valores das imagens de $f(x): A \rightarrow \mathbf{R}$, em que $A = \{x \in \mathbf{N} \mid x \ge 0\}$, formam uma progressão aritmética.
(E) os valores das imagens de $f(x): A \rightarrow \mathbf{R}$, em que $A = \{x \in \mathbf{N} \mid x \ge 0\}$, formam uma progressão geométrica.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 9. UFRGS 2016:

<div class="content-wrapper">
<div class="theory" style="font-size: 19px;">

No estudo de uma população de bactérias, identificou-se que o número $N$ de bactérias, $t$ horas após o início do estudo, é dado por $N(t) = 20 \cdot 2^{1{,}5t}$.

Nessas condições, em quanto tempo a população de mosquitos duplicou?

(A) 15 min.
(B) 20 min.
(C) 30 min.
(D) 40 min.
(E) 45 min.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>