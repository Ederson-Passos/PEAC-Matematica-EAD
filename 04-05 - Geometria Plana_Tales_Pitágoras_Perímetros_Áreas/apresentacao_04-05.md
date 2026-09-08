---
marp: true
theme: default
math: mathjax
size: 16:9
style: |
  @import url('https://fonts.googleapis.com/css2?family=Libre+Baskerville&display=swap');
  
  /* 1. O CANVAS: Fundo Noturno e Fonte principal */
  section {
    background-color: #000000;
    color: #E0E0E0;
    font-family: 'Libre Baskerville', serif;
    font-size: 28px;
    padding: 40px 60px;
    
    /* 2. A MALHA PONTILHADA MATEMÁTICA */
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
    width: 120px;
    height: 60px;
    background-image: url('logo-peac.png');
    background-size: contain;
    background-repeat: no-repeat;
    background-position: right bottom;
    opacity: 0.7;
  }

  /* 3. TIPOGRAFIA MINIMALISTA */
  h1 {
    color: #8BE9FD; /* Ciano suave */
    font-size: 32px;
    margin-bottom: 10px;
    border-bottom: 1px solid #444444;
    padding-bottom: 5px;
  }
  
  h2 {
    color: #F8F8F2;
    font-size: 24px;
    font-weight: normal;
  }

  /* 4. LISTAS */
  ul {
    list-style-type: disc;
    padding-left: 40px;
  }
  li {
    margin-bottom: 15px;
  }

  .sem-bolinha ul {
    list-style-type: none;
    padding-left: 0;
  }
  .sem-bolinha li {
    margin-bottom: 25px; 
  }

  .center { text-align: center; }

---
<div class="center">

# Matemática Pré-Vestibular
## Encontro 04: Geometria Plana (Tales, Pitágoras e Áreas)

<br><br>
*(Aguardando o início da transmissão)*
</div>

---

# 1. Teorema de Tales

O teorema afirma que um feixe de retas paralelas determina, em duas transversais, segmentos proporcionais.

$$\frac{A}{B} = \frac{C}{D}$$

<div class="center">
<svg viewBox="0 0 200 130" width="300">
  <line x1="10" y1="20" x2="190" y2="20" stroke="#8BE9FD" stroke-width="2"/>
  <line x1="10" y1="65" x2="190" y2="65" stroke="#8BE9FD" stroke-width="2"/>
  <line x1="10" y1="110" x2="190" y2="110" stroke="#8BE9FD" stroke-width="2"/>
  <line x1="50" y1="10" x2="80" y2="120" stroke="#F8F8F2" stroke-width="2"/>
  <line x1="150" y1="10" x2="120" y2="120" stroke="#F8F8F2" stroke-width="2"/>
  <text x="35" y="45" fill="#E0E0E0" font-size="14" font-family="sans-serif">A</text>
  <text x="50" y="90" fill="#E0E0E0" font-size="14" font-family="sans-serif">B</text>
  <text x="145" y="45" fill="#E0E0E0" font-size="14" font-family="sans-serif">C</text>
  <text x="130" y="90" fill="#E0E0E0" font-size="14" font-family="sans-serif">D</text>
</svg>
</div>

**Dica:** Muito útil em triângulos ao traçar uma paralela a um dos lados (Semelhança).

---

# 2. Teorema de Pitágoras

Em qualquer triângulo retângulo, o quadrado da hipotenusa é igual à soma dos quadrados dos catetos. Esta é a principal ferramenta métrica da prova.

$$a^2 = b^2 + c^2$$

<div class="center">

<svg viewBox="0 0 200 120" width="280">
  <polygon points="50,100 150,100 50,20" fill="none" stroke="#8BE9FD" stroke-width="2"/>
  <rect x="50" y="90" width="10" height="10" fill="none" stroke="#8BE9FD" stroke-width="1"/>
  <text x="90" y="115" fill="#E0E0E0" font-size="14" font-family="sans-serif">b</text>
  <text x="35" y="65" fill="#E0E0E0" font-size="14" font-family="sans-serif">c</text>
  <text x="110" y="55" fill="#8BE9FD" font-size="16" font-weight="bold" font-family="sans-serif">a</text>
</svg>

</div>

---

# 2.1 Classificação dos Triângulos (Lados)

Embora o Teorema de Pitágoras foque nos ângulos, é vital reconhecer os triângulos por suas medidas laterais, pois isso dita suas propriedades de simetria.

<div style="display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 15px; text-align: center; margin-top: 30px; font-size: 24px;">

<div>
<svg viewBox="0 0 200 150" width="180">
<polygon points="50,130 150,130 100,43.4" fill="none" stroke="#F8F8F2" stroke-width="2"/>
<line x1="96" y1="83" x2="104" y2="90" stroke="#8BE9FD" stroke-width="2"/>
<line x1="100" y1="135" x2="100" y2="125" stroke="#8BE9FD" stroke-width="2"/>
<line x1="96" y1="90" x2="104" y2="83" stroke="#8BE9FD" stroke-width="2"/>
</svg>
<br>

**Equilátero**
* **3 lados congruentes** (iguais).
* 3 ângulos internos de 60°.
</div>

<div>
<svg viewBox="0 0 200 150" width="180">
<polygon points="50,130 150,130 100,30" fill="none" stroke="#F8F8F2" stroke-width="2"/>
<line x1="71" y1="76" x2="79" y2="84" stroke="#8BE9FD" stroke-width="2"/>
<line x1="121" y1="76" x2="129" y2="84" stroke="#8BE9FD" stroke-width="2"/>
<path d="M 65 130 A 15 15 0 0 1 55 120" fill="none" stroke="#8BE9FD" stroke-width="2"/>
<path d="M 135 130 A 15 15 0 0 0 145 120" fill="none" stroke="#8BE9FD" stroke-width="2"/>
</svg>
<br>

**Isósceles**
* **2 lados congruentes**.
* Ângulos da base são iguais.
* A altura é mediana e bissetriz.
</div>

<div>
<svg viewBox="0 0 200 150" width="180">
<polygon points="30,130 170,130 80,50" fill="none" stroke="#F8F8F2" stroke-width="2"/>
<line x1="53" y1="86" x2="57" y2="94" stroke="#E0E0E0" stroke-width="1"/>
<line x1="122" y1="85" x2="128" y2="95" stroke="#E0E0E0" stroke-width="1"/>
<line x1="128" y1="85" x2="134" y2="95" stroke="#E0E0E0" stroke-width="1"/>
<line x1="97" y1="135" x2="97" y2="125" stroke="#E0E0E0" stroke-width="1"/>
<line x1="103" y1="135" x2="103" y2="125" stroke="#E0E0E0" stroke-width="1"/>
<line x1="109" y1="135" x2="109" y2="125" stroke="#E0E0E0" stroke-width="1"/>
</svg>
<br>

**Escaleno**
* Todos os **lados de medidas diferentes**.
* Todos os ângulos internos diferentes.
</div>

</div>

---

# 2.2 Soma dos Ângulos Internos

A soma dos ângulos internos de qualquer triângulo é sempre **$180^{\circ}$**.
*Curiosidade: Isso ocorre porque, ao traçarmos uma paralela à base pelo topo, criamos ângulos alternos internos.*

<div style="display: flex; justify-content: space-around; align-items: center; margin-top: 20px;">

<div style="flex: 1; font-size: 24px;">

* **Teorema do Ângulo Externo:**
  O ângulo externo ($e_1$) é igual à soma dos dois internos não adjacentes a ele.
  $$e_1 = \beta + \gamma$$

* **Lei Fundamental:**
  $$\alpha + \beta + \gamma = 180^{\circ}$$

</div>

<div style="flex: 1; text-align: center;">
<svg viewBox="0 0 250 180" width="350">
<line x1="20" y1="30" x2="230" y2="30" stroke="#444444" stroke-dasharray="4" stroke-width="1"/>
<polygon points="50,150 200,150 120,30" fill="none" stroke="#F8F8F2" stroke-width="2"/>
<path d="M 65 150 A 15 15 0 0 0 58 135" fill="none" stroke="#8BE9FD" stroke-width="2"/>
<path d="M 185 150 A 15 15 0 0 1 192 135" fill="none" stroke="#8BE9FD" stroke-width="2"/>
<path d="M 112 45 A 15 15 0 0 0 128 45" fill="none" stroke="#8BE9FD" stroke-width="2"/>
<text x="65" y="140" fill="#8BE9FD" font-size="16">β</text>
<text x="175" y="140" fill="#8BE9FD" font-size="16">γ</text>
<text x="115" y="60" fill="#8BE9FD" font-size="16">α</text>
</svg>
</div>

</div>

---

# 2.3 Triângulos e a Circunferência

Relações que você **precisa** saber para ganhar tempo:

<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 20px; margin-top: 20px; font-size: 22px;">

<div>
<div style="text-align: center; margin-bottom: 10px;">
<svg viewBox="0 0 200 150" width="180">
<circle cx="100" cy="75" r="70" fill="none" stroke="#444444" stroke-width="2" stroke-dasharray="4"/>
<polygon points="30,75 170,75 70,18" fill="none" stroke="#F8F8F2" stroke-width="2"/>
<rect x="65" y="25" width="10" height="10" fill="none" stroke="#8BE9FD" stroke-width="1" transform="rotate(-30 70 18)"/>
</svg>
</div>

**Triângulo Inscrito (no Semicírculo):**
Todo triângulo inscrito em uma semicirfurença é **Retângulo**.
* A hipotenusa é o próprio diâmetro ($2R$).
</div>

<div>
<div style="text-align: center; margin-bottom: 10px;">
<svg viewBox="0 0 200 150" width="180">
<polygon points="40,130 160,130 100,20" fill="none" stroke="#F8F8F2" stroke-width="2"/>
<circle cx="100" cy="95" r="35" fill="none" stroke="#8BE9FD" stroke-width="2"/>
</svg>
</div>

**Círculo Inscrito (no Triângulo):**
O raio ($r$) se relaciona com a área ($A$) e o semiperímetro ($p$):
$$A = p \cdot r$$
*(Área e semiperímetro do triângulo.)*
</div>

</div>

---

# 2.4 O Caso Especial: Triângulo Equilátero

No triângulo equilátero de lado $L$, os centros (incentro, baricentro, etc) coincidem. É o favorito da UFRGS.

<div style="display: flex; justify-content: space-between; align-items: center; margin-top: 10px;">

<div style="flex: 1.2; font-size: 22px;">

* **Altura ($h$):** $h = \frac{L\sqrt{3}}{2}$
* **Área ($A$):** $A = \frac{L^2\sqrt{3}}{4}$
* **Raio do Círculo Inscrito ($r$):**
  É $1/3$ da altura: $r = \frac{1}{3}h$
* **Raio do Círculo Circunscrito ($R$):**
  É $2/3$ da altura: $R = \frac{2}{3}h$

</div>

<div style="flex: 1; text-align: center;">
<svg viewBox="0 0 200 200" width="280">
<circle cx="100" cy="110" r="80" fill="none" stroke="#444444" stroke-width="1" stroke-dasharray="3"/>
<polygon points="31,150 169,150 100,30" fill="none" stroke="#F8F8F2" stroke-width="2"/>
<circle cx="100" cy="110" r="40" fill="none" stroke="#8BE9FD" stroke-width="2"/>
<line x1="100" y1="110" x2="100" y2="30" stroke="#F8F8F2" stroke-width="2"/>
<line x1="100" y1="110" x2="100" y2="150" stroke="#8BE9FD" stroke-width="2"/>
<text x="105" y="70" fill="#F8F8F2" font-size="16">R</text>
<text x="105" y="135" fill="#8BE9FD" font-size="16">r</text>
</svg>
</div>

</div>

---

# 2.5 Semelhança de Triângulos

A semelhança é a ferramenta mais elegante para evitar cálculos complexos. Dois triângulos são semelhantes quando possuem os mesmos ângulos internos. Como consequência, seus lados homólogos (opostos aos mesmos ângulos) sofrem a mesma dilatação.

<div style="display: flex; justify-content: space-between; align-items: center; margin-top: 30px;">

<div style="flex: 1.2; font-size: 24px;">

* **Razão de Semelhança ($k$):**
  A proporção se mantém constante para todos os lados correspondentes:
  $$k = \frac{a'}{a} = \frac{b'}{b} = \frac{c'}{c}$$

* **Relação de Áreas (Atenção UFRGS!):**
  Se a razão unidimensional (lados, alturas) é $k$, a razão bidimensional (área) será sempre elevada ao quadrado:
  $$\text{Razão das Áreas} = k^2$$

</div>

<div style="flex: 1; text-align: center;">

<svg viewBox="0 0 320 180" width="380">
<polygon points="20,150 100,150 70,70" fill="none" stroke="#F8F8F2" stroke-width="2"/>
<text x="40" y="142" fill="#8BE9FD" font-size="16">α</text>
<text x="75" y="142" fill="#8BE9FD" font-size="16">β</text>
<text x="63" y="100" fill="#8BE9FD" font-size="16">θ</text>
<text x="55" y="168" fill="#E0E0E0" font-size="18">c</text>
<text x="30" y="105" fill="#E0E0E0" font-size="18">b</text>
<text x="90" y="105" fill="#E0E0E0" font-size="18">a</text>

<polygon points="140,150 260,150 215,30" fill="none" stroke="#F8F8F2" stroke-width="2"/>
<text x="165" y="140" fill="#8BE9FD" font-size="16">α</text>
<text x="222" y="140" fill="#8BE9FD" font-size="16">β</text>
<text x="205" y="70" fill="#8BE9FD" font-size="16">θ</text>
<text x="185" y="168" fill="#E0E0E0" font-size="18">k·c</text>
<text x="155" y="85" fill="#E0E0E0" font-size="18">k·b</text>
<text x="245" y="85" fill="#E0E0E0" font-size="18">k·a</text>

<path d="M 35 150 A 15 15 0 0 0 28 135" fill="none" stroke="#8BE9FD" stroke-width="1"/>
<path d="M 160 150 A 20 20 0 0 0 148 130" fill="none" stroke="#8BE9FD" stroke-width="1"/>
</svg>

</div>

</div>

---

# 3. Perímetros e Comprimentos

As medidas de perímetro e comprimento tratam de grandezas unidimensionais (1D), ou seja, a "borda" das figuras.

<div style="display: flex; justify-content: space-between; align-items: center; margin-top: 30px;">

<div style="flex: 1;">

* **Perímetro (2p):** Soma de todos os lados.
* **Circunferência Inteira:** $C = 2\pi R$
* **Arco de Ângulo $\alpha$:**
  É uma fração da circunferência.

$$L = \frac{\alpha}{360^{\circ}} \cdot 2\pi R$$

</div>

<div style="flex: 1; text-align: center;">

<svg viewBox="0 0 200 200" width="280">
<circle cx="100" cy="100" r="80" fill="none" stroke="#444444" stroke-width="2" stroke-dasharray="4"/>
<path d="M 180 100 A 80 80 0 0 0 140 30" fill="none" stroke="#8BE9FD" stroke-width="4"/>
<line x1="100" y1="100" x2="180" y2="100" stroke="#F8F8F2" stroke-width="2"/>
<line x1="100" y1="100" x2="140" y2="30" stroke="#F8F8F2" stroke-width="2"/>
<text x="125" y="90" fill="#E0E0E0" font-size="14">α</text>
<text x="135" y="115" fill="#E0E0E0" font-size="14">R</text>
<text x="165" y="55" fill="#8BE9FD" font-size="18" font-weight="bold">L</text>
<circle cx="100" cy="100" r="3" fill="#F8F8F2"/>
</svg>

</div>

</div>

---

# 3.1 Áreas Fundamentais

A área mede a superfície bidimensional (2D). A altura ($h$) é sempre perpendicular à base.

<div style="display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 10px; text-align: center; margin-top: 10px;">

<div>
<svg viewBox="0 0 200 120" width="180">
<polygon points="40,100 160,100 100,20" fill="none" stroke="#F8F8F2" stroke-width="2"/>
<line x1="100" y1="20" x2="100" y2="100" stroke="#8BE9FD" stroke-dasharray="4" stroke-width="2"/>
<rect x="100" y="90" width="10" height="10" fill="none" stroke="#8BE9FD" stroke-width="1"/>
<text x="108" y="65" fill="#8BE9FD" font-size="16">h</text>
<text x="95" y="118" fill="#E0E0E0" font-size="16">b</text>
</svg>

**Triângulo**
$$A = \frac{b \cdot h}{2}$$
</div>

<div>
<svg viewBox="0 0 200 120" width="180">
<rect x="70" y="30" width="60" height="60" fill="none" stroke="#F8F8F2" stroke-width="2"/>
<text x="95" y="22" fill="#E0E0E0" font-size="16">l</text>
<text x="135" y="65" fill="#E0E0E0" font-size="16">l</text>
</svg>

**Quadrado**
$$A = l^2$$
</div>

<div>
<svg viewBox="0 0 200 120" width="180">
<rect x="40" y="40" width="120" height="60" fill="none" stroke="#F8F8F2" stroke-width="2"/>
<text x="95" y="115" fill="#E0E0E0" font-size="16">b</text>
<text x="165" y="75" fill="#E0E0E0" font-size="16">h</text>
</svg>

**Retângulo**
$$A = b \cdot h$$
</div>

<div>
<svg viewBox="0 0 200 120" width="180">
<polygon points="20,100 160,100 130,30 60,30" fill="none" stroke="#F8F8F2" stroke-width="2"/>
<line x1="60" y1="30" x2="60" y2="100" stroke="#8BE9FD" stroke-dasharray="4" stroke-width="2"/>
<rect x="60" y="90" width="10" height="10" fill="none" stroke="#8BE9FD" stroke-width="1"/>
<text x="68" y="70" fill="#8BE9FD" font-size="16">h</text>
<text x="90" y="118" fill="#E0E0E0" font-size="16">B</text>
<text x="90" y="22" fill="#E0E0E0" font-size="16">b</text>
</svg>

**Trapézio**
$$A = \frac{(B+b)h}{2}$$
</div>

<div>
<svg viewBox="0 0 200 120" width="180">
<polygon points="40,30 180,30 160,90 20,90" fill="none" stroke="#F8F8F2" stroke-width="2"/>
<line x1="40" y1="30" x2="40" y2="90" stroke="#8BE9FD" stroke-dasharray="4" stroke-width="2"/>
<rect x="40" y="80" width="10" height="10" fill="none" stroke="#8BE9FD" stroke-width="1"/>
<text x="48" y="65" fill="#8BE9FD" font-size="16">h</text>
<text x="90" y="110" fill="#E0E0E0" font-size="16">b</text>
</svg>

**Paralelogramo**
$$A = b \cdot h$$
</div>

<div>
<svg viewBox="0 0 200 120" width="180">
<circle cx="100" cy="60" r="50" fill="none" stroke="#F8F8F2" stroke-width="2"/>
<line x1="100" y1="60" x2="150" y2="60" stroke="#8BE9FD" stroke-width="2"/>
<circle cx="100" cy="60" r="3" fill="#8BE9FD"/>
<text x="120" y="55" fill="#8BE9FD" font-size="16">R</text>
</svg>

**Círculo**
$$A = \pi \cdot R^2$$
</div>

</div>

---

# 4. Estratégia: Figuras Compostas

Muitas questões exigem calcular áreas de formatos não convencionais. A técnica é sempre a mesma:

* **Decomposição:** Divida a figura em formas simples (triângulos e retângulos).
* **Subtração:** A área final geralmente é uma "Figura Maior" menos uma "Figura Menor" (um buraco).

<div class="center">
<svg viewBox="0 0 250 120" width="350">
  <rect x="75" y="10" width="100" height="100" fill="#222222" stroke="#8BE9FD" stroke-width="2"/>
  <circle cx="125" cy="60" r="40" fill="#000000" stroke="#F8F8F2" stroke-dasharray="4"/>
  <text x="25" y="65" fill="#E0E0E0" font-size="14" font-family="sans-serif">Sombreado =</text>
  <text x="190" y="65" fill="#E0E0E0" font-size="14" font-family="sans-serif">Quadrado - Círculo</text>
</svg>
</div>

---

# 5. UFRGS 2025 (Nível Médio -> Difícil)

<div style="display: flex; justify-content: space-between; align-items: flex-start; gap: 20px;">

<div style="flex: 1.2;">

**66:** Na figura abaixo, ABC é um triângulo retângulo com catetos medindo 6 e 8. A medida do raio da circunferência inscrita no triângulo ABC é:

<div style="margin-top: 20px; text-align: center;">
<svg viewBox="0 0 250 200" width="350">
<polygon points="60,30 60,160 220,160" fill="none" stroke="#F8F8F2" stroke-width="3"/>
<rect x="60" y="150" width="10" height="10" fill="none" stroke="#8BE9FD" stroke-width="1"/>
<circle cx="102" cy="118" r="42" fill="none" stroke="#8BE9FD" stroke-width="2"/>
<text x="50" y="25" fill="#E0E0E0" font-size="18">C</text>
<text x="45" y="175" fill="#E0E0E0" font-size="18">A</text>
<text x="225" y="175" fill="#E0E0E0" font-size="18">B</text>
<text x="35" y="100" fill="#8BE9FD" font-size="20">6</text>
<text x="135" y="185" fill="#8BE9FD" font-size="20">8</text>
</svg>
</div>

(A) 1. &nbsp; (B) 1,5. &nbsp; (C) 2. &nbsp; (D) 2,5. &nbsp; (E) 3.

</div>

<div style="flex: 1; border-left: 1px solid #444444; height: 500px; padding-left: 30px;">
<span style="color: #444444; font-size: 20px;">Resolução: dividir em três triângulos cuja altura é a medida do raio.</span>

</div>

</div>

---

# 5.1 UFRGS 2025 (Nível Fácil)

<div style="display: flex; justify-content: space-between; align-items: flex-start; gap: 20px;">

<div style="flex: 1.2;">

<div style="font-size: 24px; line-height: 1.4;">

**68.** Na figura abaixo, ABC é um triângulo retângulo isósceles com hipotenusa $\overline{BC} = \sqrt{2}$. Um dos arcos tem centro em A, e o outro arco tem centro no ponto médio de BC.
</div>

<div style="margin-top: 10px; text-align: center;">
<svg viewBox="0 0 250 250" width="300">
<path d="M 60 60 A 98.995 98.995 0 0 1 200 200 A 140 140 0 0 0 60 60 Z" fill="#444444" stroke="#F8F8F2" stroke-width="2"/>
<polygon points="60,200 200,200 60,60" fill="none" stroke="#F8F8F2" stroke-width="2"/>
<line x1="126" y1="195" x2="126" y2="205" stroke="#E0E0E0" stroke-width="2"/>
<line x1="134" y1="195" x2="134" y2="205" stroke="#E0E0E0" stroke-width="2"/>
<line x1="55" y1="126" x2="65" y2="126" stroke="#E0E0E0" stroke-width="2"/>
<line x1="55" y1="134" x2="65" y2="134" stroke="#E0E0E0" stroke-width="2"/>
<circle cx="60" cy="200" r="4" fill="#8BE9FD"/>
<circle cx="200" cy="200" r="4" fill="#8BE9FD"/>
<circle cx="60" cy="60" r="4" fill="#8BE9FD"/>
<text x="45" y="215" fill="#E0E0E0" font-size="18">A</text>
<text x="210" y="215" fill="#E0E0E0" font-size="18">B</text>
<text x="40" y="55" fill="#E0E0E0" font-size="18">C</text>
</svg>
</div>

<div style="font-size: 24px;">

A área da região sombreada, entre os dois arcos de circunferência de extremidades B e C, é:
</div>

<div style="margin-top: 15px; font-size: 20px;">

(A) $\frac{\sqrt{2}}{2}$ &nbsp;&nbsp;&nbsp; (B) $\frac{1}{2}$ &nbsp;&nbsp;&nbsp; (C) $\frac{\pi}{2}$ &nbsp;&nbsp;&nbsp; (D) $\frac{3\pi}{2}$ &nbsp;&nbsp;&nbsp; (E) $\frac{3\sqrt{2}}{2}$

</div>

</div>

<div style="flex: 1; border-left: 1px solid #444444; height: 550px; padding-left: 30px;">
<span style="color: #444444; font-size: 20px;">Resolução:</span>

</div>

</div>

---

# 5.2 UFRGS 2024 (Nível Médio)

<div style="display: flex; justify-content: space-between; align-items: flex-start; gap: 20px;">

<div style="flex: 1.2;">

<div style="font-size: 23px; line-height: 1.4;">

**66.** Uma folha de papel retangular $ABCD$ com lados medindo $6$ e $4$ é dobrada, de modo que o vértice $A$ fique sobre o lado $\overline{BC}$, como mostra a figura a seguir.
</div>

<div style="margin-top: 10px; text-align: center;">
<svg viewBox="0 0 250 180" width="340">
<rect x="40" y="30" width="180" height="120" fill="none" stroke="#444444" stroke-width="1" stroke-dasharray="3"/>
<polygon points="40,98.7 85.9,150 220,30" fill="#444444" stroke="#F8F8F2" stroke-width="2"/>
<polyline points="40,98.7 40,150 85.9,150" fill="none" stroke="#F8F8F2" stroke-width="2"/>
<polyline points="85.9,150 220,150 220,30" fill="none" stroke="#F8F8F2" stroke-width="2"/>
<circle cx="220" cy="30" r="3" fill="#8BE9FD"/>
<circle cx="40" cy="98.7" r="3" fill="#8BE9FD"/>
<circle cx="85.9" cy="150" r="3" fill="#8BE9FD"/>
<text x="225" y="25" fill="#E0E0E0" font-size="16">D</text>
<text x="225" y="165" fill="#E0E0E0" font-size="16">C</text>
<text x="80" y="170" fill="#E0E0E0" font-size="16">A</text>
<text x="25" y="165" fill="#E0E0E0" font-size="16">B</text>
<text x="25" y="105" fill="#E0E0E0" font-size="16">E</text>
</svg>
</div>

<div style="font-size: 23px;">

A área do triângulo $EAD$ sombreado é:
</div>

<div style="margin-top: 10px; font-size: 19px; line-height: 1.6;">

(A) $18\sqrt{5} - 30$ &nbsp;&nbsp; (B) $16 - 2\sqrt{5}$ &nbsp;&nbsp; (C) $54 - 18\sqrt{5}$ <br>
(D) $27 - 9\sqrt{5}$ &nbsp;&nbsp; (E) $27 - 2\sqrt{5}$

</div>

</div>

<div style="flex: 1; border-left: 1px solid #444444; height: 550px; padding-left: 30px;">
<span style="color: #444444; font-size: 20px;">Resolução:</span>

</div>

</div>

---

# 5.3 UFRGS 2024 (Médio com Trigonometria, Baixaria sem Trigonometria)

<div style="display: flex; justify-content: space-between; align-items: flex-start; gap: 20px;">

<div style="flex: 1.2;">

<div style="font-size: 23px; line-height: 1.4;">

**67.** Na figura abaixo, $ABC$ é um triângulo equilátero de lado 6. O ponto $D$ é ponto médio do lado $\overline{AC}$, e a medida de $\overline{EB}$ é 2.
</div>

<div style="margin-top: 10px; text-align: center;">
<svg viewBox="0 0 260 220" width="300">
<polygon points="130,24 40,180 220,180" fill="none" stroke="#F8F8F2" stroke-width="2"/>
<line x1="70" y1="128" x2="175" y2="102" stroke="#8BE9FD" stroke-width="2"/>
<circle cx="130" cy="24" r="3" fill="#8BE9FD"/>
<circle cx="40" cy="180" r="3" fill="#8BE9FD"/>
<circle cx="220" cy="180" r="3" fill="#8BE9FD"/>
<circle cx="175" cy="102" r="3" fill="#8BE9FD"/>
<circle cx="70" cy="128" r="3" fill="#8BE9FD"/>
<text x="123" y="15" fill="#E0E0E0" font-size="16">A</text>
<text x="25" y="195" fill="#E0E0E0" font-size="16">B</text>
<text x="225" y="195" fill="#E0E0E0" font-size="16">C</text>
<text x="185" y="100" fill="#E0E0E0" font-size="16">D</text>
<text x="50" y="125" fill="#E0E0E0" font-size="16">E</text>
</svg>
</div>

<div style="font-size: 23px;">

O perímetro do triângulo $AED$ é:
</div>

<div style="margin-top: 15px; font-size: 20px; line-height: 1.6;">

(A) $5 + \sqrt{5}$ &nbsp;&nbsp;&nbsp;&nbsp; (B) $7 + \sqrt{5}$ &nbsp;&nbsp;&nbsp;&nbsp; (C) $10 + \sqrt{5}$ <br>
(D) $7 + \sqrt{13}$ &nbsp;&nbsp; (E) $10 + \sqrt{13}$

</div>

</div>

<div style="flex: 1; border-left: 1px solid #444444; height: 550px; padding-left: 30px;">
<span style="color: #444444; font-size: 20px;">Resolução (com baixaria): Descobrir a altura BD, usar uma paralela EF // BD e semelhança entre os triângulos AEF e ABD.</span>

</div>

</div>

---

# 5.4 UFRGS 2024 (Fácil)

<div style="display: flex; justify-content: space-between; align-items: flex-start; gap: 20px;">

<div style="flex: 1.2;">

<div style="font-size: 22px; line-height: 1.3;">

**68.** Na figura abaixo, $ABCD$ é um quadrado de área igual a 64. O círculo sombreado passa pelos vértices $A$ e $B$ do quadrado e é tangente ao lado $\overline{CD}$.
</div>

<div style="margin-top: 5px; text-align: center;">
<svg viewBox="0 0 260 250" width="220">
<circle cx="130" cy="130" r="100" fill="#444444" stroke="#8BE9FD" stroke-width="2" opacity="0.8"/>
<rect x="50" y="30" width="160" height="160" fill="none" stroke="#F8F8F2" stroke-width="2"/>
<circle cx="50" cy="190" r="3" fill="#F8F8F2"/>
<circle cx="210" cy="190" r="3" fill="#F8F8F2"/>
<circle cx="210" cy="30" r="3" fill="#F8F8F2"/>
<circle cx="50" cy="30" r="3" fill="#F8F8F2"/>
<circle cx="130" cy="130" r="2" fill="#8BE9FD"/>
<text x="35" y="205" fill="#E0E0E0" font-size="16">A</text>
<text x="215" y="205" fill="#E0E0E0" font-size="16">B</text>
<text x="215" y="25" fill="#E0E0E0" font-size="16">C</text>
<text x="35" y="25" fill="#E0E0E0" font-size="16">D</text>
</svg>
</div>

<div style="font-size: 22px; margin-top: 5px;">

A área do círculo é:
</div>

<div style="margin-top: 10px; font-size: 20px;">

(A) $32\pi$ &nbsp;&nbsp;&nbsp; (B) $25\pi$ &nbsp;&nbsp;&nbsp; (C) $24\pi$ &nbsp;&nbsp;&nbsp; (D) $20\pi$ &nbsp;&nbsp;&nbsp; (E) $16\pi$

</div>

</div>

<div style="flex: 1; border-left: 1px solid #444444; height: 500px; padding-left: 30px;">
<span style="color: #444444; font-size: 20px;">Resolução: Construindo dois triângulos AD'B e AOB.</span>

</div>

</div>

---

# 5.5 UFRGS 2024 (Média)

<div style="display: flex; justify-content: space-between; align-items: flex-start; gap: 20px;">

<div style="flex: 1.2;">

<div style="font-size: 22px; line-height: 1.3;">

**72.** Na figura abaixo, $ABC$ é um triângulo inscrito em um semicírculo de centro $O$ e raio igual a $10$. O segmento $\overline{AD}$ é a altura do triângulo $ABC$ relativa ao vértice $A$. Tomando $x$ como a medida do segmento $\overline{BD}$, considere $A(x)$ a função que expressa a área do triângulo $ABC$ em função de $x$.

</div>

<div style="margin-top: 10px; text-align: center;">

<svg viewBox="0 0 260 140" width="320">
<path d="M 30 110 A 100 100 0 0 1 230 110 Z" fill="#222222" stroke="#F8F8F2" stroke-width="2"/>
<line x1="30" y1="110" x2="230" y2="110" stroke="#F8F8F2" stroke-width="2"/>
<polygon points="70,30 30,110 230,110" fill="none" stroke="#8BE9FD" stroke-width="2"/>
<line x1="70" y1="30" x2="70" y2="110" stroke="#8BE9FD" stroke-dasharray="4" stroke-width="2"/>
<rect x="70" y="100" width="10" height="10" fill="none" stroke="#8BE9FD" stroke-width="1"/>
<circle cx="130" cy="110" r="3" fill="#F8F8F2"/> 
<text x="65" y="25" fill="#E0E0E0" font-size="16">A</text>
<text x="15" y="125" fill="#E0E0E0" font-size="16">B</text>
<text x="235" y="125" fill="#E0E0E0" font-size="16">C</text>
<text x="65" y="125" fill="#E0E0E0" font-size="16">D</text>
<text x="125" y="125" fill="#E0E0E0" font-size="16">O</text>
<text x="45" y="125" fill="#8BE9FD" font-size="16">x</text>
</svg>

</div>

<div style="font-size: 21px; margin-top: 5px;">

Com base na figura, para $x \in [0, 20]$, $A(x)$ é:

</div>

<div style="margin-top: 10px; font-size: 18px; line-height: 1.5;">

(A) $A(x) = 20\sqrt{20x - x^2}$ &nbsp;&nbsp; (B) $A(x) = 10\sqrt{10x - x^2}$ <br>
(C) $A(x) = 10\sqrt{20x - x^2}$ &nbsp;&nbsp; (D) $A(x) = 20\sqrt{10 - x^2}$ <br>
(E) $A(x) = 10\sqrt{20 - x^2}$

</div>

</div>

<div style="flex: 1; border-left: 1px solid #444444; height: 500px; padding-left: 30px;">

<span style="color: #444444; font-size: 20px;">Resolução:</span>

</div>

</div>

---