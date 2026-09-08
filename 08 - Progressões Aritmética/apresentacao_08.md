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
    font-size: 22px;
  }

  .center { text-align: center; }

---
<div class="center">

# Matemática Pré-Vestibular
## AULA 08 - Progressões Aritméticas (P.A.)

<br><br>
*(Aguardando o início da transmissão)*
</div>

---

# 1. Lei de Formação da P.A.

<div class="content-wrapper">
<div class="theory">

Sequência onde cada termo, após o 1º, é a soma do anterior com uma constante **razão ($r$)**.

**Fórmula Recursiva:**
$$a_n = a_{n-1} + r$$

* $r > 0 \implies$ Crescente.
* $r < 0 \implies$ Decrescente.
* $r = 0 \implies$ Constante.

<div class="example-box">

**Exemplo 01:** Dada a sequência $(5, 12, 19, \dots)$, encontre a razão e determine os dois próximos termos.
</div>

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 2. Fórmula do Termo Geral

<div class="content-wrapper">
<div class="theory">

Permite encontrar qualquer termo $a_n$ a partir do primeiro $a_1$ e da razão $r$.

$$\Large a_n = a_1 + (n - 1)r$$

* $a_n$: termo geral (posição $n$).
* $a_1$: primeiro termo.
* $n$: número de termos.
* $r$: razão.

<div class="example-box">

**Exemplo 02:** Determine o 20º termo da P.A. $(3, 10, 17, \dots)$.
</div>

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 3. Termos em P.A. (3 e 5 Termos)

<div class="content-wrapper">
<div class="theory">

Para facilitar cálculos de soma e produto, usamos uma representação simétrica:

* **3 Termos:** $(x - r, \; x, \; x + r)$
* **5 Termos:** $(x-2r, \; x-r, \; x, \; x+r, \; x+2r)$

*Propriedade:* A soma desses termos cancela a razão $r$.

<div class="example-box">

**Exemplo 03:** A soma de três números em P.A. é 24 e o produto é 440. Quais são eles?
</div>

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 4. Soma dos $n$ Primeiros Termos ($S_n$)

<div class="content-wrapper">
<div class="theory">

A soma dos termos de uma P.A. é o produto da média dos extremos pela quantidade de termos.

$$\Large S_n = \frac{(a_1 + a_n) \cdot n}{2}$$

* $a_1$: primeiro termo.
* $a_n$: último termo da soma.
* $n$: quantidade de termos.

<div class="example-box">

**Exemplo 04:** Calcule a soma dos 50 primeiros termos da P.A. $(2, 6, 10, \dots)$.
</div>

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 5. UFRGS 2017

<div class="content-wrapper">
<div class="theory" style="font-size: 20px;">

Quadrados iguais de lado 1 são justapostos, segundo padrão representado nas figuras abaixo. Mantido esse padrão, o número de quadrados de lado 1 na **etapa 100** é:

<div style="text-align: center; margin-top: 15px;">
<svg viewBox="0 0 500 120" width="400">
  <rect x="0" y="80" width="20" height="20" fill="none" stroke="#E0E0E0" />
  <rect x="0" y="60" width="20" height="20" fill="none" stroke="#E0E0E0" />
  <rect x="20" y="80" width="20" height="20" fill="none" stroke="#E0E0E0" />
  <text x="20" y="115" fill="#8BE9FD" font-size="12" text-anchor="middle">etapa 1</text>
  <rect x="100" y="80" width="20" height="20" fill="none" stroke="#E0E0E0" />
  <rect x="100" y="60" width="20" height="20" fill="none" stroke="#E0E0E0" />
  <rect x="100" y="40" width="20" height="20" fill="none" stroke="#E0E0E0" />
  <rect x="120" y="80" width="20" height="20" fill="none" stroke="#E0E0E0" />
  <rect x="120" y="60" width="20" height="20" fill="none" stroke="#E0E0E0" />
  <rect x="140" y="80" width="20" height="20" fill="none" stroke="#E0E0E0" />
  <text x="130" y="115" fill="#8BE9FD" font-size="12" text-anchor="middle">etapa 2</text>
  <rect x="220" y="80" width="20" height="20" fill="none" stroke="#E0E0E0" />
  <rect x="220" y="60" width="20" height="20" fill="none" stroke="#E0E0E0" />
  <rect x="220" y="40" width="20" height="20" fill="none" stroke="#E0E0E0" />
  <rect x="220" y="20" width="20" height="20" fill="none" stroke="#E0E0E0" />
  <rect x="240" y="80" width="20" height="20" fill="none" stroke="#E0E0E0" />
  <rect x="240" y="60" width="20" height="20" fill="none" stroke="#E0E0E0" />
  <rect x="240" y="40" width="20" height="20" fill="none" stroke="#E0E0E0" />
  <rect x="260" y="80" width="20" height="20" fill="none" stroke="#E0E0E0" />
  <rect x="260" y="60" width="20" height="20" fill="none" stroke="#E0E0E0" />
  <rect x="280" y="80" width="20" height="20" fill="none" stroke="#E0E0E0" />
  <text x="255" y="115" fill="#8BE9FD" font-size="12" text-anchor="middle">etapa 3</text>
</svg>
</div>

(A) 1331 &nbsp; (B) 3050 &nbsp; (C) 5050 &nbsp; (D) 5100 &nbsp; (E) 5151

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 6. UFRGS 2018

<div class="content-wrapper">
<div class="theory" style="font-size: 22px;">

Em uma escola, as turmas totalizam **231 estudantes**. Para uma atividade, eles foram dispostos em filas: 1 estudante na 1ª fila, 2 na 2ª, 3 na 3ª, e assim sucessivamente.

O número de filas formadas com todos os estudantes é:

<br>
(A) 19 <br>
(B) 21 <br>
(C) 22 <br>
(D) 23 <br>
(E) 25

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 7. UFRGS 2019

<div class="content-wrapper">
<div class="theory" style="font-size: 22px;">

O valor numérico da expressão abaixo é:

$$\left( \frac{1}{2} + 1 \right) \cdot \left( \frac{1}{3} + 1 \right) \cdot \left( \frac{1}{4} + 1 \right) \dots \left( \frac{1}{1000} + 1 \right)$$

<br>

(A) $\frac{1001}{4}$ &nbsp;&nbsp;&nbsp; (B) $\frac{1001}{3}$ &nbsp;&nbsp;&nbsp; (C) $500$ <br><br>
(D) $501$ &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; (E) $\frac{1001}{2}$

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 8. UFRGS 2019

<div class="content-wrapper">
<div class="theory" style="font-size: 20px;">

Desde a Grécia Antiga, sabe-se que a soma dos números ímpares consecutivos, a partir do 1, é sempre um quadrado perfeito. Como exemplo, tem-se:

$$
\begin{aligned}
1 &= 1^2 \\
1 + 3 &= 2^2 \\
1 + 3 + 5 &= 3^2 \\
1 + 3 + 5 + 7 &= 4^2
\end{aligned}
$$

Então, a soma de todos os números ímpares menores do que 100 é:

<br>

(A) $42^2$ &nbsp;&nbsp;&nbsp; (B) $49^2$ &nbsp;&nbsp;&nbsp; (C) $50^2$ &nbsp;&nbsp;&nbsp; (D) $99^2$ &nbsp;&nbsp;&nbsp; (E) $100^2$

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 9. UFRGS 2023

<div class="content-wrapper">
<div class="theory" style="font-size: 22px;">

O valor de

$$\left[ \left(1 + \frac{1}{2}\right) \cdot \left(1 + \frac{1}{3}\right) \cdot \left(1 + \frac{1}{4}\right) \dots \left(1 + \frac{1}{99}\right) \right]^2$$

é:

<br>
(A) múltiplo de 4. <br>
(B) múltiplo de 5. <br>
(C) múltiplo de 6. <br>
(D) múltiplo de 7. <br>
(E) múltiplo de 8.

</div>
<div class="resolution">Resolução:</div>
</div>

---

---