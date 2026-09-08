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
## Encontro 05: Geometria Espacial (Sólidos, Áreas e Volumes)

<br><br>
*(Aguardando o início da transmissão)*
</div>

---

# 1. Fundamentos Planos Auxiliares

Antes de dominarmos o espaço tridimensional, precisamos dominar os polígonos regulares que servem de base para os principais sólidos. Eles são as "fundações" da Geometria Espacial.

<div style="display: flex; justify-content: space-around; align-items: center; margin-top: 30px; font-size: 24px;">

<div style="text-align: center;">

<svg viewBox="0 0 200 180" width="220">
  <polygon points="100,20 20,160 180,160" fill="none" stroke="#F8F8F2" stroke-width="2"/>
  <line x1="100" y1="20" x2="100" y2="160" stroke="#8BE9FD" stroke-width="2" stroke-dasharray="4"/>
  <rect x="100" y="150" width="10" height="10" fill="none" stroke="#8BE9FD" stroke-width="1"/>
  <text x="108" y="100" fill="#8BE9FD" font-size="18">h</text>
  <text x="45" y="90" fill="#E0E0E0" font-size="18">a</text>
  <text x="100" y="180" fill="#E0E0E0" font-size="18">a</text>
</svg>

<br>

**Triângulo Equilátero**<br>
$h = \frac{a\sqrt{3}}{2}$ <br> $A = \frac{a^2\sqrt{3}}{4}$

</div>

<div style="text-align: center;">

<svg viewBox="0 0 200 180" width="220">
  <polygon points="50,20 150,20 200,100 150,180 50,180 0,100" fill="none" stroke="#F8F8F2" stroke-width="2"/>
  <line x1="0" y1="100" x2="200" y2="100" stroke="#444444" stroke-width="1" stroke-dasharray="3"/>
  <line x1="50" y1="20" x2="150" y2="180" stroke="#444444" stroke-width="1" stroke-dasharray="3"/>
  <line x1="150" y1="20" x2="50" y2="180" stroke="#444444" stroke-width="1" stroke-dasharray="3"/>
  <text x="75" y="15" fill="#E0E0E0" font-size="18">a</text>
</svg>

<br>

**Hexágono Regular**<br>
6 Triângulos Equiláteros<br> $A = 6 \cdot \frac{a^2\sqrt{3}}{4}$
</div>

</div>

---

# 2. O Cubo (Hexaedro Regular)

O sólido mais perfeito e frequente. Todas as 6 faces são quadrados congruentes. É crucial dominar a diferença geométrica entre a diagonal da face e a diagonal espacial.

<div style="display: flex; justify-content: space-between; align-items: center; margin-top: 10px;">

<div style="flex: 1.2; font-size: 24px;">

* **Área Total ($A_t$):** 6 faces quadradas.
  $$A_t = 6a^2$$
* **Volume ($V$):** Base $\times$ Altura.
  $$V = a^3$$
* **Diagonal da Face ($d$):** Percorre a superfície.
  $$d = a\sqrt{2}$$
* **Diagonal do Cubo ($D$):** Atravessa o vazio interno, conectando vértices opostos.
  $$D = a\sqrt{3}$$

</div>

<div style="flex: 1; text-align: center;">

<svg viewBox="0 0 220 220" width="300">
  <polyline points="50,170 50,70 120,40" fill="none" stroke="#444444" stroke-width="2" stroke-dasharray="4"/>
  <line x1="50" y1="170" x2="120" y2="140" stroke="#444444" stroke-width="2" stroke-dasharray="4"/>
  <line x1="100" y1="200" x2="190" y2="70" stroke="#E0E0E0" stroke-width="2"/>
  <text x="145" y="150" fill="#E0E0E0" font-size="16">d = a√2</text>
  <line x1="100" y1="200" x2="120" y2="40" stroke="#8BE9FD" stroke-width="3" stroke-dasharray="6"/>
  <text x="80" y="115" fill="#8BE9FD" font-size="18" font-weight="bold">D = a√3</text>
  <polygon points="100,200 190,170 190,70 100,100" fill="none" stroke="#F8F8F2" stroke-width="2"/>
  <polygon points="100,100 190,70 120,40 30,70" fill="none" stroke="#F8F8F2" stroke-width="2"/>
  <polyline points="30,70 30,170 100,200" fill="none" stroke="#F8F8F2" stroke-width="2"/>
  <text x="60" y="200" fill="#E0E0E0" font-size="16">a</text>
</svg>

</div>

</div>

---

# 3. Paralelepípedo Retângulo

Uma generalização do cubo, onde as dimensões (comprimento, largura e altura) são distintas. Pense nele como uma caixa de sapatos.

<div style="display: flex; justify-content: space-between; align-items: center; margin-top: 10px;">

<div style="flex: 1.2; font-size: 24px;">

* **Área Total ($A_t$):** Soma das áreas dos 3 pares de faces retangulares opostas.
  $$A_t = 2(ab + ac + bc)$$
* **Volume ($V$):** Área da base $\times$ altura.
  $$V = a \cdot b \cdot c$$
* **Diagonal Espacial ($D$):** Aplicação estendida do Teorema de Pitágoras no $\mathbb{R}^3$.
  $$D = \sqrt{a^2 + b^2 + c^2}$$

</div>

<div style="flex: 1; text-align: center;">

<svg viewBox="0 0 280 200" width="350">
  <line x1="100" y1="140" x2="60" y2="180" stroke="#444444" stroke-width="2" stroke-dasharray="4"/>
  <line x1="100" y1="140" x2="260" y2="140" stroke="#444444" stroke-width="2" stroke-dasharray="4"/>
  <line x1="100" y1="140" x2="100" y2="60" stroke="#444444" stroke-width="2" stroke-dasharray="4"/>
  <line x1="60" y1="180" x2="260" y2="60" stroke="#8BE9FD" stroke-width="3" stroke-dasharray="6"/>
  <text x="150" y="115" fill="#8BE9FD" font-size="18" font-weight="bold">D</text>
  <polygon points="60,180 220,180 220,100 60,100" fill="none" stroke="#F8F8F2" stroke-width="2"/>
  <polygon points="220,180 260,140 260,60 220,100" fill="none" stroke="#F8F8F2" stroke-width="2"/>
  <polygon points="60,100 220,100 260,60 100,60" fill="none" stroke="#F8F8F2" stroke-width="2"/>
  <text x="130" y="195" fill="#E0E0E0" font-size="18">a</text>
  <text x="245" y="170" fill="#E0E0E0" font-size="18">b</text>
  <text x="35" y="145" fill="#E0E0E0" font-size="18">c</text>
</svg>

</div>

</div>

---

# 4. Pirâmides e Cones (Os Sólidos "de Bico")

Qualquer sólido que se afunila até um único vértice obedece à mesma regra mestre de volume, que equivale a exatamente **um terço** do volume do prisma ou cilindro que o contém.

<div style="display: flex; justify-content: space-around; align-items: center; margin-top: 20px; font-size: 24px;">

<div style="text-align: center;">

<svg viewBox="0 0 200 220" width="220">
  <polyline points="40,170 100,140 160,170" fill="none" stroke="#444444" stroke-width="2" stroke-dasharray="4"/>
  <line x1="100" y1="20" x2="100" y2="155" stroke="#8BE9FD" stroke-width="3" stroke-dasharray="5"/>
  <text x="110" y="100" fill="#8BE9FD" font-size="18">h</text>
  <polyline points="40,170 100,200 160,170" fill="none" stroke="#F8F8F2" stroke-width="2"/>
  <polyline points="40,170 100,20 160,170" fill="none" stroke="#F8F8F2" stroke-width="2"/>
  <line x1="100" y1="20" x2="100" y2="200" stroke="#F8F8F2" stroke-width="2"/>
</svg>

<br>

**Pirâmide (Base Poligonal)**<br>
$$V = \frac{A_b \cdot h}{3}$$

</div>

<div style="text-align: center;">

<svg viewBox="0 0 200 220" width="220">
  <ellipse cx="100" cy="180" rx="70" ry="25" fill="none" stroke="#444444" stroke-width="2" stroke-dasharray="4"/>
  <path d="M 30 180 A 70 25 0 0 0 170 180" fill="none" stroke="#F8F8F2" stroke-width="2"/>
  <line x1="100" y1="30" x2="100" y2="180" stroke="#8BE9FD" stroke-width="3" stroke-dasharray="5"/>
  <line x1="100" y1="180" x2="170" y2="180" stroke="#F8F8F2" stroke-width="2"/>
  <polyline points="30,180 100,30 170,180" fill="none" stroke="#F8F8F2" stroke-width="2"/>
  <text x="110" y="100" fill="#8BE9FD" font-size="18">h</text>
  <text x="135" y="195" fill="#E0E0E0" font-size="16">R</text>
</svg>

<br>

**Cone Circular Reto**<br>
$$V = \frac{\pi R^2 h}{3}$$

</div>

</div>

---

# 5. O Tetraedro Regular

A pirâmide triangular perfeita. Composta estritamente por 4 triângulos equiláteros. Suas propriedades derivam elegantemente do teorema de Pitágoras aplicado ao baricentro de sua base.

<div style="display: flex; justify-content: space-between; align-items: center; margin-top: 10px;">

<div style="flex: 1; font-size: 24px;">

* **Área Total ($A_t$):** 4 triângulos equiláteros.
  $$A_t = a^2\sqrt{3}$$
* **Altura ($H$):** Cai exatamente no baricentro do triângulo da base.
  $$H = \frac{a\sqrt{6}}{3}$$
* **Volume ($V$):** $\frac{1}{3} \cdot A_b \cdot H$
  $$V = \frac{a^3\sqrt{2}}{12}$$

</div>

<div style="flex: 1; text-align: center;">
<svg viewBox="0 0 240 220" width="300">
  <line x1="40" y1="180" x2="200" y2="160" stroke="#444444" stroke-width="2" stroke-dasharray="4"/>
  <line x1="120" y1="20" x2="125" y2="155" stroke="#8BE9FD" stroke-width="3" stroke-dasharray="5"/>
  <line x1="120" y1="200" x2="125" y2="155" stroke="#444444" stroke-width="1" stroke-dasharray="2"/>
  <text x="105" y="95" fill="#8BE9FD" font-size="18" font-weight="bold">H</text>
  <polygon points="120,20 40,180 120,200" fill="none" stroke="#F8F8F2" stroke-width="2"/>
  <polygon points="120,20 200,160 120,200" fill="none" stroke="#F8F8F2" stroke-width="2"/>
  <text x="65" y="205" fill="#E0E0E0" font-size="18">a</text>
</svg>
</div>

</div>

---

# 6. A Esfera

O sólido de máxima otimização: possui a maior proporção de volume contido para a menor área de superfície possível. É gerado pela rotação de $360^{\circ}$ de um semicírculo em torno de seu diâmetro.

<div style="display: flex; justify-content: space-between; align-items: center; margin-top: 10px;">

<div style="flex: 1.2; font-size: 24px;">

* **Área da Superfície Esférica ($A$):** Equivale exatamente a quatro vezes a área de seu círculo equatorial máximo.
  $$A = 4\pi R^2$$

* **Volume ($V$):**
  $$V = \frac{4}{3}\pi R^3$$

*(Nota: Secções em uma esfera sempre geram círculos menores, cuja distância ao centro pode ser calculada via Pitágoras).*

</div>

<div style="flex: 1; text-align: center;">

<svg viewBox="0 0 240 240" width="300">
  <circle cx="120" cy="120" r="100" fill="none" stroke="#F8F8F2" stroke-width="2"/>
  <path d="M 20 120 A 100 35 0 0 1 220 120" fill="none" stroke="#444444" stroke-width="2" stroke-dasharray="4"/>
  <path d="M 20 120 A 100 35 0 0 0 220 120" fill="none" stroke="#8BE9FD" stroke-width="2"/>
  <circle cx="120" cy="120" r="3" fill="#F8F8F2"/>
  <line x1="120" y1="120" x2="215" y2="135" stroke="#F8F8F2" stroke-width="2"/>
  <text x="160" y="125" fill="#E0E0E0" font-size="18">R</text>
</svg>

</div>

</div>

---

# 7. UFRGS 2025 - Questão 69

<div style="display: flex; justify-content: space-between; align-items: flex-start; gap: 20px;">

<div style="flex: 1.2;">

<div style="font-size: 22px; line-height: 1.4;">

**69.** Um sólido S é formado por cubos de aresta 1, justapostos. A figura abaixo mostra as vistas frontal, lateral e superior do sólido S.
</div>

<div style="margin-top: 15px; text-align: center;">
<svg viewBox="0 0 450 150" width="450">
  <g transform="translate(10, 10)">
    <rect x="0" y="80" width="40" height="40" fill="#D0D0D0" stroke="#000" stroke-width="1"/>
    <rect x="40" y="80" width="40" height="40" fill="#D0D0D0" stroke="#000" stroke-width="1"/>
    <rect x="40" y="40" width="40" height="40" fill="#D0D0D0" stroke="#000" stroke-width="1"/>
    <rect x="80" y="80" width="40" height="40" fill="#D0D0D0" stroke="#000" stroke-width="1"/>
    <rect x="80" y="40" width="40" height="40" fill="#D0D0D0" stroke="#000" stroke-width="1"/>
    <rect x="80" y="0" width="40" height="40" fill="#D0D0D0" stroke="#000" stroke-width="1"/>
    <text x="80" y="140" fill="#E0E0E0" font-size="14" text-anchor="middle">FRONTAL</text>
  </g>
  <g transform="translate(190, 10)">
    <rect x="0" y="80" width="40" height="40" fill="#D0D0D0" stroke="#000" stroke-width="1"/>
    <rect x="0" y="40" width="40" height="40" fill="#D0D0D0" stroke="#000" stroke-width="1"/>
    <rect x="0" y="0" width="40" height="40" fill="#D0D0D0" stroke="#000" stroke-width="1"/>
    <rect x="40" y="80" width="40" height="40" fill="#D0D0D0" stroke="#000" stroke-width="1"/>
    <rect x="40" y="40" width="40" height="40" fill="#D0D0D0" stroke="#000" stroke-width="1"/>
    <rect x="80" y="80" width="40" height="40" fill="#D0D0D0" stroke="#000" stroke-width="1"/>
    <text x="60" y="140" fill="#E0E0E0" font-size="14" text-anchor="middle">LATERAL</text>
  </g>
  <g transform="translate(320, 10)">
    <rect x="0" y="0" width="40" height="40" fill="#D0D0D0" stroke="#000" stroke-width="1"/>
    <rect x="40" y="0" width="40" height="40" fill="#D0D0D0" stroke="#000" stroke-width="1"/>
    <rect x="80" y="0" width="40" height="40" fill="#D0D0D0" stroke="#000" stroke-width="1"/>
    <rect x="80" y="40" width="40" height="40" fill="#D0D0D0" stroke="#000" stroke-width="1"/>
    <rect x="80" y="80" width="40" height="40" fill="#D0D0D0" stroke="#000" stroke-width="1"/>
    <text x="60" y="140" fill="#E0E0E0" font-size="14" text-anchor="middle">SUPERIOR</text>
  </g>
</svg>
</div>

<div style="font-size: 22px; margin-top: 10px;">
O volume do sólido S é:
</div>

<div style="margin-top: 10px; font-size: 20px;">
(A) 9. &nbsp;&nbsp;&nbsp; (B) 10. &nbsp;&nbsp;&nbsp; (C) 12. &nbsp;&nbsp;&nbsp; (D) 15. &nbsp;&nbsp;&nbsp; (E) 17.
</div>

</div>

<div style="flex: 1; border-left: 1px solid #444444; height: 500px; padding-left: 30px;">
<span style="color: #444444; font-size: 20px;">Resolução:</span>

</div>

</div>

---

# 7.1 UFRGS 2025 - Questão 70

<div style="display: flex; justify-content: space-between; align-items: flex-start; gap: 20px;">

<div style="flex: 1.2;">

<div style="font-size: 19px; line-height: 1.4;">

**70.** Na figura abaixo, $ABCD$ é um tetraedro regular de aresta 1. Os pontos $E, F, G, I$ e $H$ são pontos médios das arestas $AD, CD, BD, AB$ e $AC$, respectivamente.
</div>

<div style="margin-top: 5px; text-align: center;">
<svg viewBox="0 0 300 250" width="280">
  <line x1="40" y1="180" x2="240" y2="150" stroke="#F8F8F2" stroke-width="2" stroke-dasharray="4"/>
  <line x1="240" y1="150" x2="140" y2="40" stroke="#F8F8F2" stroke-width="2"/>
  <polygon points="40,180 120,210 180,165 140,110 80,125 90,110" fill="#8BE9FD" opacity="0.3"/>
  <line x1="40" y1="180" x2="140" y2="165" stroke="#444444" stroke-width="2" stroke-dasharray="4"/>
  <line x1="140" y1="165" x2="190" y2="105" stroke="#444444" stroke-width="2" stroke-dasharray="4"/>
  <line x1="40" y1="180" x2="120" y2="210" stroke="#E0E0E0" stroke-width="2"/>
  <line x1="120" y1="210" x2="180" y2="165" stroke="#E0E0E0" stroke-width="2"/>
  <line x1="40" y1="180" x2="90" y2="110" stroke="#E0E0E0" stroke-width="2"/>
  <line x1="120" y1="210" x2="140" y2="110" stroke="#E0E0E0" stroke-width="2"/>
  <line x1="180" y1="165" x2="190" y2="105" stroke="#E0E0E0" stroke-width="2"/>
  <polygon points="90,110 140,110 190,105 140,95" fill="none" stroke="#E0E0E0" stroke-width="2"/>
  <line x1="140" y1="40" x2="40" y2="180" stroke="#F8F8F2" stroke-width="2"/>
  <line x1="140" y1="40" x2="160" y2="230" stroke="#F8F8F2" stroke-width="2"/>
  <line x1="40" y1="180" x2="160" y2="230" stroke="#F8F8F2" stroke-width="2"/>
  <line x1="160" y1="230" x2="240" y2="150" stroke="#F8F8F2" stroke-width="2"/>
  <circle cx="140" cy="40" r="3" fill="#8BE9FD"/> <text x="135" y="30" fill="#E0E0E0" font-size="14">D</text>
  <circle cx="40" cy="180" r="3" fill="#8BE9FD"/> <text x="20" y="190" fill="#E0E0E0" font-size="14">A</text>
  <circle cx="160" cy="230" r="3" fill="#8BE9FD"/> <text x="165" y="245" fill="#E0E0E0" font-size="14">B</text>
  <circle cx="240" cy="150" r="3" fill="#8BE9FD"/> <text x="250" y="155" fill="#E0E0E0" font-size="14">C</text>
  <text x="75" y="105" fill="#E0E0E0" font-size="14">E</text>
  <text x="200" y="105" fill="#E0E0E0" font-size="14">F</text>
  <text x="120" y="130" fill="#E0E0E0" font-size="14">G</text>
  <text x="105" y="215" fill="#E0E0E0" font-size="14">I</text>
  <text x="145" y="185" fill="#E0E0E0" font-size="14">H</text>
</svg>
</div>

<div style="font-size: 19px; margin-top: -5px;">
O volume do prisma AIHEGF é:
</div>

<div style="margin-top: 5px; font-size: 18px;">

(A) $\frac{\sqrt{2}}{32}$ &nbsp;&nbsp;&nbsp;&nbsp; (B) $\frac{\sqrt{2}}{24}$ &nbsp;&nbsp;&nbsp;&nbsp; (C) $\frac{\sqrt{2}}{16}$ &nbsp;&nbsp;&nbsp;&nbsp; (D) $\frac{\sqrt{2}}{8}$ &nbsp;&nbsp;&nbsp;&nbsp; (E) $\frac{\sqrt{2}}{4}$

</div>

</div>

<div style="flex: 1; border-left: 1px solid #444444; height: 500px; padding-left: 30px;">
<span style="color: #444444; font-size: 20px;">Resolução:</span>

</div>

</div>

---

# 7.2 UFRGS 2024 - Questão 69

<div style="display: flex; justify-content: space-between; align-items: flex-start; gap: 20px;">

<div style="flex: 1.2;">

<div style="font-size: 19px; line-height: 1.4;">

**69.** Na figura abaixo, $ABCDEFGH$ é um cubo de aresta 1. Os pontos $M, N, O, P, Q$ e $R$ são pontos médios das arestas $\overline{AB}, \overline{BC}, \overline{CG}, \overline{GH}, \overline{HE}$ e $\overline{EA}$, respectivamente.
</div>

<div style="margin-top: 5px; text-align: center;">
<svg viewBox="0 0 300 240" width="280">
  <polyline points="70,180 110,140 190,140" fill="none" stroke="#444444" stroke-width="2" stroke-dasharray="4"/>
  <line x1="110" y1="140" x2="110" y2="60" stroke="#444444" stroke-width="2" stroke-dasharray="4"/>
  <polygon points="110,180 170,180 210,140 170,60 90,60 70,120" fill="#8BE9FD" opacity="0.4" stroke="#8BE9FD" stroke-width="2"/>
  <line x1="190" y1="60" x2="110" y2="180" stroke="#E0E0E0" stroke-width="1"/>
  <line x1="190" y1="60" x2="170" y2="180" stroke="#E0E0E0" stroke-width="1"/>
  <line x1="190" y1="60" x2="210" y2="140" stroke="#E0E0E0" stroke-width="1"/>
  <line x1="190" y1="60" x2="170" y2="60" stroke="#E0E0E0" stroke-width="1"/>
  <line x1="190" y1="60" x2="90" y2="60" stroke="#E0E0E0" stroke-width="1"/>
  <line x1="190" y1="60" x2="70" y2="120" stroke="#E0E0E0" stroke-width="1"/>
  <polygon points="70,180 150,180 150,100 70,100" fill="none" stroke="#F8F8F2" stroke-width="2"/>
  <polygon points="70,100 110,60 190,60 150,100" fill="none" stroke="#F8F8F2" stroke-width="2"/>
  <polyline points="190,60 190,140 150,180" fill="none" stroke="#F8F8F2" stroke-width="2"/>
  <text x="55" y="195" fill="#E0E0E0" font-size="12">A</text>
  <text x="155" y="195" fill="#E0E0E0" font-size="12">B</text>
  <text x="200" y="145" fill="#E0E0E0" font-size="12">C</text>
  <text x="100" y="135" fill="#E0E0E0" font-size="12">D</text>
  <text x="55" y="95" fill="#E0E0E0" font-size="12">E</text>
  <text x="180" y="105" fill="#E0E0E0" font-size="12">F</text>
  <text x="200" y="55" fill="#E0E0E0" font-size="12">G</text>
  <text x="105" y="50" fill="#E0E0E0" font-size="12">H</text>
  <text x="105" y="195" fill="#8BE9FD" font-size="14">M</text>
  <text x="175" y="190" fill="#8BE9FD" font-size="14">N</text>
  <text x="220" y="110" fill="#8BE9FD" font-size="14">O</text>
</svg>
</div>

<div style="font-size: 19px; margin-top: -5px;">
O volume da pirâmide de base MNOPQR e vértice F é:
</div>

<div style="margin-top: 5px; font-size: 18px;">

(A) $\frac{1}{4}$ &nbsp;&nbsp;&nbsp;&nbsp; (B) $\frac{1}{2}$ &nbsp;&nbsp;&nbsp;&nbsp; (C) $\frac{3}{2}$ &nbsp;&nbsp;&nbsp;&nbsp; (D) $\frac{3}{4}$ &nbsp;&nbsp;&nbsp;&nbsp; (E) $\frac{3}{8}$

</div>

</div>

<div style="flex: 1; border-left: 1px solid #444444; height: 500px; padding-left: 30px;">
<span style="color: #444444; font-size: 20px;">Resolução:</span>

</div>

</div>

---

# 7.3 UFRGS 2024 - Questão 70

<div style="display: flex; justify-content: space-between; align-items: flex-start; gap: 20px;">

<div style="flex: 1.2;">

<div style="font-size: 23px; line-height: 1.5;">

**70.** O volume do sólido gerado pela rotação de um quadrado de lado $a$ em torno de uma de suas diagonais é:

</div>

<div style="margin-top: 30px; text-align: center;">

</div>

<div style="margin-top: 30px; font-size: 21px; line-height: 1.6;">

(A) $\frac{a^3\pi\sqrt{2}}{12}$ &nbsp;&nbsp;&nbsp;&nbsp; (B) $\frac{a^3\pi\sqrt{2}}{6}$ &nbsp;&nbsp;&nbsp;&nbsp; (C) $\frac{a^3\pi\sqrt{2}}{4}$ <br><br>
(D) $\frac{a^3\pi\sqrt{2}}{3}$ &nbsp;&nbsp;&nbsp;&nbsp; (E) $\frac{a^3\pi\sqrt{2}}{2}$
</div>

</div>

<div style="flex: 1; border-left: 1px solid #444444; height: 500px; padding-left: 30px;">
<span style="color: #444444; font-size: 20px;">Resolução:</span>

</div>

</div>

---