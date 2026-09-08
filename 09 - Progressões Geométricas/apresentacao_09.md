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
## AULA 09 - Progressões Geométricas (P.G.)


*(Aguardando o início da transmissão)*
</div>

---

# 1. Lei de Formação da P.G.

<div class="content-wrapper">
<div class="theory">

Sequência numérica onde cada termo, a partir do segundo, é igual ao produto do termo anterior por uma constante chamada **razão ($q$)**.

**Fórmula Recursiva:**
$$a_n = a_{n-1} \cdot q$$

* $q > 1$ (com $a_1 > 0$) $\implies$ Crescente.
* $0 < q < 1$ (com $a_1 > 0$) $\implies$ Decrescente.
* $q < 0 \implies$ Alternante (ou Oscilante).

<div class="example-box">

**Exemplo 01:** Dada a sequência $(3, 6, 12, \dots)$, encontre a razão e determine os dois próximos termos.
</div>

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 2. Fórmula do Termo Geral

<div class="content-wrapper">
<div class="theory">

Ferramenta analítica que nos permite encontrar qualquer termo $a_n$ relacionando apenas o primeiro termo $a_1$, a razão $q$ e a posição $n$.

$$\Large a_n = a_1 \cdot q^{n-1}$$

* $a_n$: termo geral (posição $n$).
* $a_1$: primeiro termo.
* $n$: número de termos (ou posição).
* $q$: razão geométrica.

<div class="example-box">

**Exemplo 02:** Determine o 7º termo da P.G. $(2, 6, 18, \dots)$.
</div>

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 3. Soma dos $n$ Primeiros Termos (Soma Finita)

<div class="content-wrapper">
<div class="theory">

Para calcular a soma de uma quantidade restrita de termos de uma P.G. (onde $q \neq 1$), utilizamos a seguinte relação estrutural:

$$\Large S_n = \frac{a_1 \cdot (q^n - 1)}{q - 1}$$

*Caso particular:* Se $q = 1$, a sequência é constante e a soma é simplesmente $S_n = n \cdot a_1$.

<div class="example-box">

**Exemplo 03:** Calcule a soma dos 6 primeiros termos da P.G. $(5, 10, 20, \dots)$.
</div>

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 4. Soma dos Termos da P.G. Infinita (Limite)

<div class="content-wrapper">
<div class="theory">

Quando a razão está no intervalo estritamente entre $-1$ e $1$ (ou seja, $|q| < 1$), os termos tornam-se infinitamente pequenos. A série geométrica converge para um limite finito:

$$\Large S_{\infty} = \frac{a_1}{1 - q}$$

Essa é a essência do conceito de limite em séries convergentes, fundamental no Cálculo.

<div class="example-box">

**Exemplo 04:** Calcule o valor da soma infinita $\left(16 + 8 + 4 + 2 + \dots\right)$.
</div>

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 5. UFRGS 2025

<div class="content-wrapper">
<div class="theory" style="font-size: 22px;">

O valor da expressão $\frac{1}{\sqrt{2}} + \frac{1}{2\sqrt{2}} + \frac{1}{4\sqrt{2}} + \dots$ é

<br><br>

(A) $\frac{1}{2}$ <br>
(B) $1$ <br>
(C) $\sqrt{2}$ <br>
(D) $2\sqrt{2}$ <br>
(E) $3\sqrt{2}$

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 6. UFRGS 2024

<div class="content-wrapper">
<div class="theory" style="font-size: 22px;">

O valor da expressão $a + \frac{a}{4} + \frac{a}{16} + \dots$ para $a = 15$ é

<br><br>

(A) $20$ <br>
(B) $16$ <br>
(C) $15$ <br>
(D) $10$ <br>
(E) $8$

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 7. UFRGS 2020

<div class="content-wrapper">
<div class="theory" style="font-size: 18px;">

A figura é formada por quadrados de lados $\overline{P_1P_2}$, $\overline{P_2P_3}$, $\overline{P_3P_4} \dots$ A construção é tal que $P_1, P_2, \dots, B$ são colineares, e as bases medem $\overline{P_1P_2} = 1$, $\overline{P_2P_3} = \frac{1}{2}$, $\overline{P_3P_4} = \frac{1}{4}$ e assim por diante. O ponto $A$ é vértice do 1º quadrado. A medida de $\overline{AB}$ é:

<div style="text-align: center; margin-top: 10px;">
<svg viewBox="0 0 250 150" width="350">
  <rect x="20" y="20" width="100" height="100" fill="none" stroke="#E0E0E0" stroke-width="1.5"/>
  <rect x="120" y="70" width="50" height="50" fill="none" stroke="#E0E0E0" stroke-width="1.5"/>
  <rect x="170" y="95" width="25" height="25" fill="none" stroke="#E0E0E0" stroke-width="1.5"/>
  <rect x="195" y="107.5" width="12.5" height="12.5" fill="none" stroke="#E0E0E0" stroke-width="1.5"/>
  <line x1="20" y1="20" x2="220" y2="120" stroke="#8BE9FD" stroke-dasharray="4" stroke-width="1.5"/>
  <text x="20" y="135" fill="#8BE9FD" font-size="12" text-anchor="middle">P₁</text>
  <text x="120" y="135" fill="#8BE9FD" font-size="12" text-anchor="middle">P₂</text>
  <text x="170" y="135" fill="#8BE9FD" font-size="12" text-anchor="middle">P₃</text>
  <text x="225" y="135" fill="#8BE9FD" font-size="12" text-anchor="start">B</text>
  <text x="10" y="20" fill="#8BE9FD" font-size="12" text-anchor="end">A</text>
</svg>
</div>

(A) $1$ &nbsp;&nbsp;&nbsp; (B) $\sqrt{2}$ &nbsp;&nbsp;&nbsp; (C) $\sqrt{3}$ &nbsp;&nbsp;&nbsp; (D) $2$ &nbsp;&nbsp;&nbsp; (E) $\sqrt{5}$

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 8. UFRGS 2023

<div class="content-wrapper">
<div class="theory" style="font-size: 22px;">

Considere as seguintes afirmações sobre números e suas operações.

<br>

**I.** $1 + \frac{1}{2} + \frac{1}{4} + \frac{1}{8} \dots > 2 + \frac{2}{3} + \frac{2}{9} + \frac{2}{27} \dots$

**II.** $\sqrt{\sqrt{7} + 10} < \sqrt{\sqrt{7}} + \sqrt{10}$

**III.** $6 \cdot 5^{10} < 5 \cdot 6^{10}$

<br>
*(Analise quais das afirmações acima são verdadeiras)*

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 9. UFRGS 2020

<div class="content-wrapper">
<div class="theory" style="font-size: 22px;">

O valor de

$$\sqrt{\left(1 - \frac{1}{2}\right) \cdot \left(1 - \frac{1}{3}\right) \cdot \left(1 - \frac{1}{4}\right) \dots \left(1 - \frac{1}{100}\right)}$$

é

<br><br>

(A) $\frac{1}{10}$ &nbsp;&nbsp;&nbsp;&nbsp; (B) $\frac{1}{100}$ &nbsp;&nbsp;&nbsp;&nbsp; (C) $1$ <br><br>
(D) $2$ &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; (E) $3$

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 10. UFRGS 2017

<div class="content-wrapper">
<div class="theory" style="font-size: 16px;">

Na figura abaixo, encontram-se representados quadrados de maneira que o maior quadrado ($Q_1$) tem lado 1. O quadrado $Q_2$ está construído com vértices nos pontos médios dos lados de $Q_1$; o quadrado $Q_3$ está construído com vértices nos pontos médios dos lados de $Q_2$ e, assim, sucessiva e infinitamente.

<div style="text-align: center; margin-top: 10px; margin-bottom: 5px;">
<svg viewBox="0 0 300 300" width="280">
  <polygon points="30,270 150,270 30,150" fill="rgba(139, 233, 253, 0.5)" />
  <polygon points="150,270 210,210 90,210" fill="rgba(139, 233, 253, 0.5)" />
  <polygon points="210,210 210,150 150,210" fill="rgba(139, 233, 253, 0.5)" />
  <polygon points="210,150 180,120 180,180" fill="rgba(139, 233, 253, 0.5)" />
  <polygon points="180,120 150,120 180,150" fill="rgba(139, 233, 253, 0.5)" />
  <polygon points="150,120 135,135 165,135" fill="rgba(139, 233, 253, 0.5)" />
  <polygon points="135,135 135,150 150,135" fill="rgba(139, 233, 253, 0.5)" />
  <polygon points="135,150 142.5,157.5 142.5,142.5" fill="rgba(139, 233, 253, 0.5)" />

  <polygon points="30,30 270,30 270,270 30,270" fill="none" stroke="#E0E0E0" stroke-width="1.5"/>
  <polygon points="150,30 270,150 150,270 30,150" fill="none" stroke="#E0E0E0" stroke-width="1.5"/>
  <polygon points="90,90 210,90 210,210 90,210" fill="none" stroke="#E0E0E0" stroke-width="1.5"/>
  <polygon points="150,90 210,150 150,210 90,150" fill="none" stroke="#E0E0E0" stroke-width="1.5"/>
  <polygon points="120,120 180,120 180,180 120,180" fill="none" stroke="#E0E0E0" stroke-width="1.5"/>
  <polygon points="150,120 180,150 150,180 120,150" fill="none" stroke="#E0E0E0" stroke-width="1.5"/>
  <polygon points="135,135 165,135 165,165 135,165" fill="none" stroke="#E0E0E0" stroke-width="1.5"/>
  <polygon points="150,135 165,150 150,165 135,150" fill="none" stroke="#E0E0E0" stroke-width="1.5"/>
  <polygon points="142.5,142.5 157.5,142.5 157.5,157.5 142.5,157.5" fill="none" stroke="#E0E0E0" stroke-width="1.5"/>


</svg>
</div>

A soma das áreas da sequência infinita de triângulos sombreados na figura é

<br>

(A) $\frac{1}{2}$ &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; (B) $\frac{1}{4}$ &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; (C) $\frac{1}{8}$ &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; (D) $\frac{1}{16}$ &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; (E) $\frac{1}{32}$

</div>
<div class="resolution">Resolução:</div>
</div>

---