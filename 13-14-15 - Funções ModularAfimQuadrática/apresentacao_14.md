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
    color: #FF79C6;
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
---
<div class="center">

# Matemática Pré-Vestibular
## AULA 14 - Função Quadrática: Conceitos, Gráficos e Otimização

*(Aguardando o início da transmissão)*
</div>

---

# 1. A Função Quadrática: Forma Geral

<div class="content-wrapper">
<div class="theory" style="font-size: 21px;">

A **função quadrática** (ou de 2º grau) é definida por um polinômio de grau 2. Seu gráfico é sempre uma parábola e ela é a ferramenta perfeita para modelar áreas, trajetórias e otimizações.

* **Fórmula Geral:** $f(x) = ax^2 + bx + c$, com $a \neq 0$.
O formato mais comum nos exercícios. Expõe diretamente a concavidade ($a$) e a intersecção com o eixo $y$ ($c$).

<div class="center" style="margin-top: 15px;">
  <div class="svg-box">
  <svg viewBox="0 0 300 200" width="250" height="160">
    <defs>
      <marker id="arrow-gen" markerWidth="10" markerHeight="10" refX="9" refY="3" orient="auto" markerUnits="strokeWidth">
        <path d="M0,0 L0,6 L9,3 z" fill="#E0E0E0" />
      </marker>
    </defs>
    <line x1="20" y1="150" x2="280" y2="150" stroke="#E0E0E0" stroke-width="2" marker-end="url(#arrow-gen)"/>
    <line x1="150" y1="180" x2="150" y2="20" stroke="#E0E0E0" stroke-width="2" marker-end="url(#arrow-gen)"/>
    <path d="M 60 40 Q 150 250 240 40" fill="none" stroke="#8BE9FD" stroke-width="3"/>
    <text x="285" y="145" fill="#E0E0E0" font-size="14">x</text>
    <text x="135" y="25" fill="#E0E0E0" font-size="14">y</text>
    <circle cx="150" cy="144" r="4" fill="#FF79C6"/>
    <text x="165" y="155" fill="#FF79C6" font-size="14">Vértice</text>
  </svg>
  </div>
</div>

</div>
<div class="resolution">

</div>
</div>

---

# 1.1 Exemplo: Identificação

<div class="content-wrapper">
<div class="theory">

Compreender a estrutura algébrica da função é o primeiro passo para qualquer análise gráfica ou resolução de problemas.

<div class="example-box">

**Exemplo 01:** Dada a função quadrática $f(x) = x^2 - 6x + 5$:
a) Identifique os coeficientes $a$, $b$ e $c$.
b) Determine o valor da função para $x = 0$ e $x = 1$.

</div>

</div>
<div class="resolution">

</div>
</div>

---

# 2. A Concavidade e o Eixo y

<div class="content-wrapper">
<div class="theory" style="font-size: 20px;">

A geometria fundamental da parábola é governada pelos coeficientes $a$ e $c$:

* **Coeficiente Principal ($a$):** Define a "boca" da parábola.
  * $a > 0$: Concavidade para **cima** (formato de sorriso). Possui um ponto de **mínimo**.
  * $a < 0$: Concavidade para **baixo** (formato de tristeza). Possui um ponto de **máximo**.

* **Termo Independente ($c$):** É a ordenada do ponto exato onde a parábola corta o eixo vertical ($y$). Ocorre quando $x = 0$, resultando no ponto $(0, c)$.

<div class="center" style="margin-top: 10px;">
  <div class="svg-box">
  <svg viewBox="0 0 400 130" width="350" height="110">
    <path d="M 40 40 Q 100 130 160 40" fill="none" stroke="#8BE9FD" stroke-width="3"/>
    <text x="100" y="125" fill="#E0E0E0" font-size="16" text-anchor="middle" font-family="sans-serif">a &gt; 0</text>
    <path d="M 240 100 Q 300 10 360 100" fill="none" stroke="#FF79C6" stroke-width="3"/>
    <text x="300" y="125" fill="#E0E0E0" font-size="16" text-anchor="middle" font-family="sans-serif">a &lt; 0</text>
  </svg>
  </div>
</div>

</div>
<div class="resolution">

</div>
</div>

---

# 2.1 Exemplo: Análise de Gráfico

<div class="content-wrapper">
<div class="theory">

Vamos aplicar a relação entre os coeficientes e a representação geométrica.

<div class="example-box">

**Exemplo 02:** Seja a função quadrática $f(x) = (2m - 6)x^2 + 4x - 10$.
a) Para quais valores reais de $m$ a parábola terá sua concavidade voltada para baixo?
b) Em qual ponto exato do plano cartesiano o gráfico desta função intercepta o eixo das ordenadas ($y$)?

</div>

</div>
<div class="resolution">

</div>
</div>

---

# 3. Zeros (Raízes) e o Discriminante ($\Delta$)

<div class="content-wrapper">
<div class="theory" style="font-size: 21px;">

Os **zeros** são os pontos de travessia geométrica no eixo horizontal ($f(x) = 0$). Calculamos via Fórmula de Bhaskara: $x = \frac{-b \pm \sqrt{\Delta}}{2a}$.

O valor do discriminante ($\Delta = b^2 - 4ac$) dita o comportamento da função em relação ao eixo $x$:

* **$\Delta > 0$:** Duas raízes reais e distintas. A parábola corta o eixo $x$ em dois pontos diferentes.
* **$\Delta = 0$:** Duas raízes reais e iguais. A parábola tangencia (encosta) no eixo $x$ em um único ponto.
* **$\Delta < 0$:** Não existem raízes reais. A parábola "flutua", não tocando o eixo $x$ em nenhum momento.

</div>
<div class="resolution">

</div>
</div>

---

# 3.1 Exemplo: Encontrando os Zeros

<div class="content-wrapper">
<div class="theory">

<div class="example-box">

**Exemplo 03:** Determine a quantidade de raízes reais (intersecções com o eixo $x$) e calcule os seus valores, caso existam, para as seguintes funções:

a) $f(x) = x^2 - 6x + 9$

b) $g(x) = -2x^2 + 5x - 4$

</div>

</div>
<div class="resolution">

</div>
</div>

---

# 4. Relações de Girard (Soma e Produto)

<div class="content-wrapper">
<div class="theory" style="font-size: 21px;">

As Relações de Girard conectam as raízes $x_1$ e $x_2$ diretamente aos coeficientes $a, b$ e $c$, permitindo encontrar as raízes por dedução lógica sem depender da Fórmula de Bhaskara.

* **Soma das Raízes ($S$):** $x_1 + x_2 = -\frac{b}{a}$
* **Produto das Raízes ($P$):** $x_1 \cdot x_2 = \frac{c}{a}$

**Dica de Ouro:** Quando o coeficiente $a = 1$, a função pode ser lida mentalmente no formato $f(x) = x^2 - Sx + P$. 

</div>
<div class="resolution">

</div>
</div>

---

# 4.1 Exemplo: Aplicando Girard

<div class="content-wrapper">
<div class="theory">

A técnica de soma e produto economiza minutos preciosos em provas longas como as da UFRGS.

<div class="example-box">

**Exemplo 04:** 
a) Utilizando o método da soma e produto, determine as raízes da função $f(x) = x^2 - 8x + 15$.
b) Monte a lei de formação geral de uma função quadrática cujas raízes sejam $4$ e $-2$, assumindo $a=1$.

</div>

</div>
<div class="resolution">

</div>
</div>

---

# 5. Coordenadas do Vértice

<div class="content-wrapper">
<div class="theory" style="font-size: 21px;">

O vértice $V(x_v, y_v)$ é o "bico" da parábola. É o ponto que define a mudança de comportamento da função (de crescente para decrescente, ou vice-versa).

* **Coordenada $x_v$:** É o Eixo de Simetria. É exatamente a média aritmética das raízes.
  $$x_v = -\frac{b}{2a}$$
* **Coordenada $y_v$:** É o valor extremo da função. Calcula-se aplicando $x_v$ na função, ou pela fórmula direta:
  $$y_v = -\frac{\Delta}{4a}$$

</div>
<div class="resolution">

</div>
</div>

---

# 5.1 Exemplo: Máximos e Mínimos

<div class="content-wrapper">
<div class="theory">

<div class="example-box">

**Exemplo 05:** Dada a função quadrática $f(x) = -x^2 + 4x + 5$:
a) Calcule as coordenadas do seu vértice $V(x_v, y_v)$.
b) Este vértice representa um ponto de máximo ou um ponto de mínimo absoluto? Justifique visualmente.
c) Com base no vértice, determine o conjunto Imagem desta função.

</div>

</div>
<div class="resolution">

</div>
</div>

---

# 6. Problemas de Modelagem (Otimização)

<div class="content-wrapper">
<div class="theory" style="font-size: 21px;">

A função quadrática é a protagonista em questões contextualizadas que pedem otimização (maximizar ou minimizar algo). O segredo para não errar é a interpretação do texto:

* **O texto pede o $x_v$ (A Causa):** Quando a pergunta é sobre "Quando", "Em que instante", "Qual a quantidade produzida", "Qual o preço cobrado" para que o máximo ocorra.

* **O texto pede o $y_v$ (A Consequência):** Quando a pergunta foca no limite do fenômeno: "Qual o lucro máximo", "Qual a altura máxima atingida", "Qual o custo mínimo".

</div>
<div class="resolution">

</div>
</div>

---

# 6.1 Exemplo: Modelando Negócios

<div class="content-wrapper">
<div class="theory">

<div class="example-box">

**Exemplo 06:** O lucro $L$, em milhares de reais, de uma pequena indústria na venda de $x$ centenas de unidades de um equipamento é modelado matematicamente por $L(x) = -2x^2 + 16x - 14$.
a) Quantas centenas de unidades a indústria precisa vender para obter o lucro máximo possível?
b) Qual é, em milhares de reais, o valor absoluto desse lucro máximo?

</div>

</div>
<div class="resolution">

</div>
</div>

---

# 7. UFRGS 2010

<div class="content-wrapper">
<div class="theory" style="font-size: 19px;">

O gráfico do polinômio de coeficientes reais $p(x) = ax^2 + bx + c$ está representado abaixo.

<div class="center">
  <div class="svg-box">
  <svg viewBox="0 0 200 200" width="160" height="160">
    <defs>
      <marker id="arrow1" markerWidth="10" markerHeight="10" refX="9" refY="3" orient="auto" markerUnits="strokeWidth">
        <path d="M0,0 L0,6 L9,3 z" fill="#E0E0E0" />
      </marker>
    </defs>
    <line x1="10" y1="140" x2="190" y2="140" stroke="#E0E0E0" stroke-width="2" marker-end="url(#arrow1)"/>
    <line x1="80" y1="195" x2="80" y2="10" stroke="#E0E0E0" stroke-width="2" marker-end="url(#arrow1)"/>
    <path d="M 20 105 Q 100 265 180 105" fill="none" stroke="#8BE9FD" stroke-width="2"/>
    <text x="185" y="130" fill="#E0E0E0" font-size="14">x</text>
    <text x="65" y="20" fill="#E0E0E0" font-size="14">y</text>
  </svg>
  </div>
</div>

Com base nos dados desse gráfico, é correto afirmar que os coeficientes $a$, $b$ e $c$ satisfazem as desigualdades:

(A) $a > 0$; $b < 0$; $c < 0$.<br>
(B) $a > 0$; $b < 0$; $c > 0$.<br>
(C) $a > 0$; $b > 0$; $c > 0$.<br>
(D) $a > 0$; $b > 0$; $c < 0$.<br>
(E) $a < 0$; $b < 0$; $c < 0$.

</div>
<div class="resolution">

</div>
</div>

---

# 8. UFRGS 2017

<div class="content-wrapper">
<div class="theory" style="font-size: 21px;">

As raízes da equação $2x^2 + bx + c = 0$ são $3$ e $-4$.

Nesse caso, o valor numérico de $b - c$ é:

<br><br>

(A) -26. <br>
(B) -22. <br>
(C) -1. <br>
(D) 22. <br>
(E) 26.

</div>
<div class="resolution">

</div>
</div>

---

# 9. UFRGS 2014

<div class="content-wrapper">
<div class="theory" style="font-size: 21px;">

Dadas as funções $f$ e $g$, definidas respectivamente por $f(x) = x^2 - 4x + 3$ e $g(x) = -x^2 - 4x - 3$ e representadas no mesmo sistema de coordenadas cartesianas.

A distância geométrica entre os vértices de suas parábolas é:

<br><br>

(A) 4. <br>
(B) 5. <br>
(C) $\sqrt{5}$. <br>
(D) $\sqrt{10}$. <br>
(E) $2\sqrt{5}$.

</div>
<div class="resolution">

</div>
</div>

---

# 10. UFRGS 2025

<div class="content-wrapper">
<div class="theory" style="font-size: 17px;">

O gráfico da função $f(x) = x^2 - 2x + 3$ está representado no sistema de coordenadas cartesianas da figura abaixo. O vértice A do triângulo isósceles ABC está posicionado no vértice da parábola, e o vértice B está posicionado na origem do sistema.

<div class="center" style="margin: 5px 0;">
  <div class="svg-box">
  <svg viewBox="0 0 300 200" width="220" height="150">
    <defs>
      <marker id="arrow2" markerWidth="10" markerHeight="10" refX="9" refY="3" orient="auto" markerUnits="strokeWidth">
        <path d="M0,0 L0,6 L9,3 z" fill="#E0E0E0" />
      </marker>
    </defs>
    <line x1="20" y1="160" x2="280" y2="160" stroke="#E0E0E0" stroke-width="2" marker-end="url(#arrow2)"/>
    <line x1="50" y1="180" x2="50" y2="20" stroke="#E0E0E0" stroke-width="2" marker-end="url(#arrow2)"/>
    <path d="M 10 32.5 Q 130 167.5 250 32.5" fill="none" stroke="#E0E0E0" stroke-width="2"/>
    <polygon points="50,160 210,160 130,100" fill="rgba(139, 233, 253, 0.4)" stroke="#8BE9FD" stroke-width="2"/>
    <circle cx="130" cy="100" r="4" fill="#FF79C6"/>
    <text x="130" y="90" fill="#FF79C6" font-size="16" text-anchor="middle">A</text>
    <circle cx="50" cy="160" r="4" fill="#FF79C6"/>
    <text x="40" y="175" fill="#FF79C6" font-size="16">B</text>
    <circle cx="210" cy="160" r="4" fill="#FF79C6"/>
    <text x="210" y="175" fill="#FF79C6" font-size="16">C</text>
  </svg>
  </div>
</div>

A área do triângulo ABC é:

(A) 1. <br>
(B) 2. <br>
(C) 4. <br>
(D) 6. <br>
(E) 8.

</div>
<div class="resolution">

</div>
</div>