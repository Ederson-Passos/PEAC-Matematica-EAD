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

  table {
    border-collapse: collapse;
    margin: 15px auto;
    font-size: 20px;
    background-color: transparent !important;
  }

  table tr {
    background-color: transparent !important;
  }

  table tr:nth-child(2n) {
    background-color: rgba(255, 255, 255, 0.05) !important;
  }

  th, td {
    border: 1px solid #444444 !important;
    padding: 10px 25px;
    text-align: center;
    color: #E0E0E0 !important;
    background-color: transparent !important;
  }

  th {
    color: #8BE9FD !important;
    background-color: rgba(139, 233, 253, 0.1) !important;
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
---
<div class="center">

# Matemática Pré-Vestibular
## AULA 24 - Geometria Analítica

*(Aguardando o início da transmissão)*
</div>

---

# 1. O Plano Cartesiano: Ponto, Distância e Ponto Médio

<style scoped>
.theory { font-size: 19px; }
.example-box { font-size: 17px; padding: 12px 14px; margin-top: 6px; }
</style>

<div class="content-wrapper">
<div class="theory">

O plano cartesiano associa pares ordenados $(x, y)$ a pontos geométricos em quatro quadrantes.

- **Distância entre dois pontos:** Teorema de Pitágoras no triângulo formado por $\Delta x = x_B - x_A$ e $\Delta y = y_B - y_A$:
  $$ d(A, B) = \sqrt{(x_B - x_A)^2 + (y_B - y_A)^2} $$

- **Ponto Médio de um Segmento:** Média aritmética das coordenadas das extremidades:
  $$ M = \left(\frac{x_A + x_B}{2}, \; \frac{y_A + y_B}{2}\right) $$

- **Área de Triângulos no Plano:** Para vértices $A, B$ e $C$, a área é dada por $A = \frac{1}{2} |\det|$, ou por $\frac{\text{base} \cdot \text{altura}}{2}$ quando alinhado aos eixos.

<div class="example-box">

**Exemplo 01:** Considere os pontos $A(1, 2)$, $B(5, 5)$ e $C(1, 5)$.
a) Calcule a distância entre os pontos $A$ e $B$.
b) Determine as coordenadas do ponto médio $M$ do segmento $AB$.
c) Calcule a área do triângulo $ABC$.

</div>

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 2. Estudo da Reta: Coeficiente Angular e Equações

<style scoped>
.theory { font-size: 19px; }
.example-box { font-size: 17px; padding: 12px 14px; margin-top: 6px; }
</style>

<div class="content-wrapper">
<div class="theory">

A inclinação de uma reta determina sua declividade e taxa de variação.

- **Coeficiente Angular ($m$):** Tangente do ângulo de inclinação $\theta$ com o semi-eixo $x$ positivo:
  $$ m = \tan(\theta) = \frac{\Delta y}{\Delta x} = \frac{y_B - y_A}{x_B - x_A} $$
  - $m > 0$: reta crescente | $m < 0$: reta decrescente | $m = 0$: reta horizontal.

- **Equação Fundamental (Ponto e Declividade):**
  $$ y - y_0 = m(x - x_0) $$

- **Equação Reduzida:** $y = mx + n$, onde $n$ é o **coeficiente linear** (intercepto no eixo $y$, ponto $(0, n)$).
- **Equação Geral:** $Ax + By + C = 0$, com $m = -\frac{A}{B}$ e $n = -\frac{C}{B}$.

<div class="example-box">

**Exemplo 02:** Determine a equação reduzida da reta que passa pelos pontos $A(2, 1)$ e $B(6, 9)$. Em seguida, indique o coeficiente angular e o ponto onde a reta corta o eixo vertical $y$.

</div>

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 3. Posições Relativas entre Retas e Sistemas Lineares

<style scoped>
.theory { font-size: 19px; }
.example-box { font-size: 17px; padding: 12px 14px; margin-top: 6px; }
</style>

<div class="content-wrapper">
<div class="theory">

Dadas duas retas $r: y = m_1 x + n_1$ e $s: y = m_2 x + n_2$:

- **Retas Paralelas ($r \parallel s$):** Possuem a mesma inclinação:
  $$ m_1 = m_2 \quad (\text{e } n_1 \neq n_2 \text{ para paralelas distintas}) $$

- **Retas Concorrentes:** Inclinações diferentes ($m_1 \neq m_2$). O ponto de interseção $(x_0, y_0)$ é a solução do sistema linear:
  $$ \begin{cases} y = m_1 x + n_1 \\ y = m_2 x + n_2 \end{cases} $$

- **Retas Perpendiculares ($r \perp s$):** Formam ângulo reto ($90^\circ$):
  $$ m_1 \cdot m_2 = -1 \iff m_2 = -\frac{1}{m_1} $$
  *(A declividade de uma é o inverso do oposto da outra).*

<div class="example-box">

**Exemplo 03:** Dadas as retas $r: y = 2x - 1$ e $s: x + 2y - 8 = 0$:
a) Mostre que $r$ e $s$ são perpendiculares.
b) Determine o ponto de interseção $(x_0, y_0)$ entre as duas retas.

</div>

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 4. Distância de Ponto a Reta e Condição de Tangência

<style scoped>
.theory { font-size: 19px; }
.example-box { font-size: 17px; padding: 12px 14px; margin-top: 6px; }
</style>

<div class="content-wrapper">
<div class="theory">

A menor distância entre um ponto $P(x_0, y_0)$ e uma reta $r: Ax + By + C = 0$ ocorre sobre o segmento perpendicular:
$$ d(P, r) = \frac{|A x_0 + B y_0 + C|}{\sqrt{A^2 + B^2}} $$

**Aplicações fundamentais no vestibular:**
- **Altura de Triângulos:** É a distância de um vértice até a reta suporte da base oposta.
- **Tangência à Circunferência:** Uma reta tangencia uma circunferência de centro $C$ e raio $R$ se, e somente se, a distância do centro à reta for igual ao raio:
  $$ d(C, r) = R $$
  *(Se $d < R$, a reta é secante; se $d > R$, a reta é externa).*

<div class="example-box">

**Exemplo 04:**
a) Calcule a distância do ponto $P(2, 3)$ à reta $r: 3x + 4y - 8 = 0$.
b) Uma circunferência tem centro em $C(2, 3)$ e tangencia a reta $r$. Qual é o raio dessa circunferência?

</div>

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 5. A Circunferência no Plano Cartesiano

<style scoped>
.theory { font-size: 19px; }
.example-box { font-size: 17px; padding: 12px 14px; margin-top: 6px; }
</style>

<div class="content-wrapper">
<div class="theory">

A circunferência é o lugar geométrico dos pontos $P(x, y)$ equidistantes de um ponto fixo $C(x_0, y_0)$ (centro):

- **Equação Reduzida:**
  $$ (x - x_0)^2 + (y - y_0)^2 = R^2 $$

- **Equação Geral:** Expandindo os quadrados perfeitos:
  $$ x^2 + y^2 - 2x_0 x - 2y_0 y + (x_0^2 + y_0^2 - R^2) = 0 $$
  *Dica rápida:* Divida os coeficientes lineares de $x$ e $y$ por $-2$ para obter as coordenadas do centro $(x_0, y_0)$.

- **Distância entre Circunferências:** Sendo $d = d(C_1, C_2)$ a distância entre os centros, a menor distância entre duas circunferências exteriores é:
  $$ d_{\min} = d(C_1, C_2) - (R_1 + R_2) $$

<div class="example-box">

**Exemplo 05:** Dada a circunferência de equação $x^2 + y^2 - 6x + 8y = 0$:
a) Determine as coordenadas do centro $C$ e o raio $R$.
b) Determine os pontos em que a circunferência intercepta o eixo $x$ ($y=0$).

</div>

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 6. Regiões do Plano, Inequações e Noções de Cônicas (A Elipse)

<style scoped>
.theory { font-size: 19px; }
.example-box { font-size: 17px; padding: 12px 14px; margin-top: 6px; }
</style>

<div class="content-wrapper">
<div class="theory">

- **Inequações no Plano:**
  - $y > mx + n$: semiplano **acima** da reta (e $y < mx + n$ abaixo).
  - $(x - x_0)^2 + (y - y_0)^2 \le R^2$: representa o **círculo** (borda e interior).
  - A interseção de semiplanos e círculos gera setores ou segmentos circulares (se o ângulo central for $90^\circ$, a área é $\frac{\pi R^2}{4}$).

- **A Elipse no Vestibular:**
  - Equação reduzida com centro na origem: $\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1$.
  - Vértices nos eixos: $(\pm a, 0)$ e $(0, \pm b)$.
  - A área do losango formado pelos 4 vértices é $A = \frac{(2a)(2b)}{2} = 2ab$.

<div class="example-box">

**Exemplo 06:**
a) Qual é a área da região definida por $\begin{cases} x^2 + y^2 \le 16 \\ x \ge 0 \\ y \ge 0 \end{cases}$?
b) Dada a elipse $\frac{x^2}{4} + \frac{y^2}{9} = 1$, determine os seus 4 vértices e a área do quadrilátero determinado por eles.

</div>

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# Questão 01 - UFRGS 2025

<style scoped>
.theory { font-size: 17px; }
</style>

<div class="content-wrapper">
<div class="theory">

O gráfico da função $f(x) = x^2 - 2x + 3$ está representado no sistema de coordenadas cartesianas da figura abaixo. O vértice A do triângulo isósceles ABC está posicionado no vértice da parábola, e o vértice B está posicionado na origem do sistema de coordenadas cartesianas.

<div style="text-align: center; margin: 4px 0;">
<svg width="220" height="135" viewBox="-20 -15 220 150">
  <!-- Eixos -->
  <line x1="0" y1="120" x2="190" y2="120" stroke="#8BE9FD" stroke-width="1.5" />
  <line x1="40" y1="130" x2="40" y2="10" stroke="#8BE9FD" stroke-width="1.5" />
  <text x="185" y="135" fill="#8BE9FD" font-size="12">x</text>
  <text x="28" y="15" fill="#8BE9FD" font-size="12">y</text>
  <!-- Triângulo -->
  <polygon points="40,120 120,120 80,40" fill="rgba(139,233,253,0.3)" stroke="#F8F8F2" stroke-width="1.5" />
  <!-- Parábola -->
  <path d="M 20,5 Q 80,75 140,5" fill="none" stroke="#F1FA8C" stroke-width="2" />
  <!-- Vértices -->
  <circle cx="80" cy="40" r="3.5" fill="#FF79C6" />
  <circle cx="40" cy="120" r="3.5" fill="#FF79C6" />
  <circle cx="120" cy="120" r="3.5" fill="#FF79C6" />
  <text x="80" y="32" fill="#F8F8F2" font-size="12" font-weight="bold" text-anchor="middle">A</text>
  <text x="30" y="132" fill="#F8F8F2" font-size="12" font-weight="bold">B</text>
  <text x="125" y="132" fill="#F8F8F2" font-size="12" font-weight="bold">C</text>
</svg>
</div>

A área do triângulo ABC é

(A) 1.
(B) 2.
(C) 4.
(D) 6.
(E) 8.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# Questão 02 - UFRGS 2019

<style scoped>
.theory { font-size: 16px; }
</style>

<div class="content-wrapper">
<div class="theory">

Considere os pontos A, B e C, de coordenadas inteiras, que determinam os vértices do triângulo ABC, representado no sistema de coordenadas cartesianas abaixo.

A revolução do triângulo ABC, em torno do eixo x, gera o sólido P, e a revolução do triângulo ABC, em torno do eixo y, gera o sólido Q.

<div style="text-align: center; margin: 4px 0;">
<svg width="220" height="130" viewBox="-15 -10 215 140">
  <!-- Eixos -->
  <line x1="10" y1="110" x2="190" y2="110" stroke="#8BE9FD" stroke-width="1.5" />
  <line x1="30" y1="125" x2="30" y2="10" stroke="#8BE9FD" stroke-width="1.5" />
  <text x="185" y="125" fill="#8BE9FD" font-size="11">x</text>
  <text x="18" y="15" fill="#8BE9FD" font-size="11">y</text>
  <!-- Ticks x -->
  <text x="25" y="122" fill="#888" font-size="10">0</text>
  <line x1="65" y1="107" x2="65" y2="113" stroke="#888" /><text x="63" y="122" fill="#888" font-size="9">2</text>
  <line x1="100" y1="107" x2="100" y2="113" stroke="#888" /><text x="98" y="122" fill="#888" font-size="9">4</text>
  <!-- Ticks y -->
  <line x1="27" y1="20" x2="33" y2="20" stroke="#888" /><text x="18" y="23" fill="#888" font-size="9">6</text>
  <!-- Triângulo ABC -->
  <polygon points="30,20 65,110 100,110" fill="rgba(139,233,253,0.3)" stroke="#F8F8F2" stroke-width="1.5" />
  <circle cx="30" cy="20" r="3" fill="#FF79C6" />
  <circle cx="65" cy="110" r="3" fill="#FF79C6" />
  <circle cx="100" cy="110" r="3" fill="#FF79C6" />
  <text x="35" y="18" fill="#F8F8F2" font-size="11" font-weight="bold">A</text>
  <text x="60" y="103" fill="#F8F8F2" font-size="11" font-weight="bold">B</text>
  <text x="105" y="105" fill="#F8F8F2" font-size="11" font-weight="bold">C</text>
</svg>
</div>

A razão entre os volumes de P e Q é

(A) $\dfrac{2}{3}$.
(B) $1$.
(C) $\dfrac{3}{2}$.
(D) $18$.
(E) $36$.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# Questão 03 - UFRGS 2019

<style scoped>
.theory { font-size: 18px; }
</style>

<div class="content-wrapper">
<div class="theory">

A área da região determinada pela interseção das desigualdades
$$ y > \frac{3}{2}x - \frac{3}{2}, $$
$$ y > -\frac{2}{3}x + 5 $$
e
$$ (x - 3)^2 + (y - 3)^2 < 9 $$
é

(A) $\dfrac{3\pi}{4}$.
(B) $\dfrac{3\pi}{2}$.
(C) $\dfrac{9\pi}{4}$.
(D) $\dfrac{9\pi}{2}$.
(E) $9\pi$.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# Questão 04 - UFRGS 2019

<style scoped>
.theory { font-size: 18px; }
</style>

<div class="content-wrapper">
<div class="theory">

A área do quadrilátero formado pelos pontos de interseção da circunferência de equação
$$ (x + 1)^2 + y^2 = 4 $$
com os eixos coordenados é

(A) $\sqrt{3}$.
(B) $2\sqrt{3}$.
(C) $3\sqrt{3}$.
(D) $4\sqrt{3}$.
(E) $12$.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>
