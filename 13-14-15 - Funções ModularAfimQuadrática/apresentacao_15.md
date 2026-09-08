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
---
<div class="center">

# Matemática Pré-Vestibular
## AULA 15 - Módulo, Função Modular e Transformações Geométricas

*(Aguardando o início da transmissão)*
</div>

---

# 1. O Conceito de Módulo (Valor Absoluto)

<div class="content-wrapper">
<div class="theory" style="font-size: 20px;">

O **Módulo** ou Valor Absoluto de um número real é, fundamentalmente, a sua **distância até a origem** (o zero) na reta numérica. Sendo uma distância, o resultado de um módulo é *sempre* não-negativo.

A definição algébrica estrita é dividida em duas sentenças (uma função definida por partes):

$$
|x| = \begin{cases} 
x, & \text{se } x \ge 0 \\ 
-x, & \text{se } x < 0 
\end{cases}
$$

Isso significa que o módulo mantém o sinal de valores positivos e inverte o sinal (multiplicando por $-1$) de valores negativos, "forçando-os" a ficarem positivos.

</div>
<div class="resolution">
<h3> </h3>
</div>
</div>

---

# 1.1 Exemplo: Equação Modular Clássica

<div class="content-wrapper">
<div class="theory">

Ao resolver uma equação com módulo, devemos sempre considerar os **dois caminhos** possíveis que geram aquela mesma distância.

<div class="example-box">

**Exemplo 01:** O módulo garante que a distância do interior até o zero é fixa. Resolva matematicamente a seguinte equação modular:
$$|2x - 6| = 10$$
Quais são os possíveis valores da variável $x$?

</div>

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 2. A Função Modular e a Geometria em "V"

<div class="content-wrapper">
<div class="theory" style="font-size: 21px;">

A função mãe desse estudo é a $f(x) = |x|$. 
Lembra da **Função Afim**? Geometricamente, o módulo atua pegando a reta $y=x$ e **espelhando a parte negativa** para o quadrante positivo. O resultado é o clássico gráfico em formato de "V".

<div class="center" style="margin-top: 15px;">
<div class="svg-box">
<svg viewBox="0 0 200 150" width="200" height="150">
<defs>
<marker id="arrow1" markerWidth="10" markerHeight="10" refX="9" refY="3" orient="auto" markerUnits="strokeWidth">
<path d="M0,0 L0,6 L9,3 z" fill="#E0E0E0"/>
</marker>
</defs>
<line x1="20" y1="120" x2="180" y2="120" stroke="#E0E0E0" stroke-width="2" marker-end="url(#arrow1)"/>
<line x1="100" y1="140" x2="100" y2="20" stroke="#E0E0E0" stroke-width="2" marker-end="url(#arrow1)"/>
<!-- V-shape -->
<path d="M 20 40 L 100 120 L 180 40" fill="none" stroke="#8BE9FD" stroke-width="3"/>
<line x1="100" y1="120" x2="70" y2="150" stroke="#8BE9FD" stroke-width="2" stroke-dasharray="4,4" opacity="0.4"/>
</svg>
</div>
</div>

O bico do "V" ocorre exatamente na **raiz** do interior do módulo, pois é onde o valor do $y$ bate no zero e rebate para cima.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 3. Transformações Geométricas: A Arte de Deslocar

<div class="content-wrapper">
<div class="theory" style="font-size: 20px;">

A UFRGS raramente pede contas complexas, ela exige que você saiba **deslocar** gráficos! A forma estrutural $f(x) = |x - h| + k$ nos dita todo o movimento do "V" a partir da origem:

* **O parâmetro $h$ (dentro do módulo):** Desloca o gráfico na **horizontal**. Dica: iguale o interior a zero para encontrar o novo "x" do bico.
* **O parâmetro $k$ (fora do módulo):** Desloca o gráfico na **vertical**. Eleva ou afunda a função no plano.

<div class="example-box">

**Exemplo 02:** Sem construir longas tabelas de valores, identifique mentalmente as coordenadas $(x,y)$ do vértice e esboce o gráfico da função $f(x) = |x - 3| - 2$.

</div>

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 4. O Efeito Espelho: Parábolas Modulares

<div class="content-wrapper">
<div class="theory" style="font-size: 20px;">

Podemos misturar o módulo com a nossa aula anterior sobre **Funções Quadráticas**. 
Quando aplicamos o módulo sobre uma função inteira, $y = |ax^2 + bx + c|$, criamos um espelho rigoroso apoiado no eixo $x$. 

As partes da parábola que já são positivas não se alteram. Porém, o "fundo" da parábola (a porção negativa) sofre um espelhamento rebatido para cima, criando a clássica curva em formato de **"W"** (ou "M").

<div class="example-box">

**Exemplo 03:** Dada a função quadrática basal $f(x) = x^2 - 4x + 3$. Suas raízes são 1 e 3. Esboce como ficaria o gráfico da função espelhada $g(x) = |x^2 - 4x + 3|$.

</div>

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 5. UFRGS 2021: Polígonos de Intersecção

<div class="content-wrapper">
<div class="theory" style="font-size: 20px;">

O auge da prova da UFRGS é cruzar duas funções modulares (uma "em pé" e outra de "cabeça para baixo") formando um polígono no meio para você calcular a área.

<br>

**(UFRGS 2021) Questão 09** - A área da região compreendida entre os gráficos das funções $f(x)$ e $g(x)$, definidas por $f(x) = |x - 2| + 1$ e $g(x) = -|x| + 5$, é:

<br>

(A) 4.<br>
(B) 6.<br>
(C) 10.<br>
(D) 15.<br>
(E) 20.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 6. UFRGS 2012: O Losango Modular

<div class="content-wrapper">
<div class="theory" style="font-size: 21px;">

**(UFRGS 2012) Questão 23** - A interseção dos gráficos das funções $f$ e $g$, definidas por $f(x) = |x|$ e $g(x) = 1 - |x|$, os quais são desenhados no mesmo sistema de coordenadas cartesianas, determina um polígono.

A área desse polígono é:

<br>

(A) 0,125.<br>
(B) 0,25.<br>
(C) 0,5.<br>
(D) 1.<br>
(E) 2.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 7. UFRGS 2019: Inequações Modulares

<div class="content-wrapper">
<div class="theory" style="font-size: 21px;">

**(UFRGS 2019) Questão 11** - Considere as funções $f(x) = |x + 1|$ e $g(x) = -|x| - 1$.

O intervalo tal que $f(x) > g(x)$ é:

<br><br>

(A) $(-\infty, -1) \cup (1, +\infty)$<br>
(B) $\left(-\frac{1}{2}, \frac{1}{2}\right)$<br>
(C) $(-\infty, 0) \cup (1, +\infty)$<br>
(D) $(-1, +\infty)$<br>
(E) $(-\infty, +\infty)$

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 8. UFRGS 2018: Translação com Módulo

<div class="content-wrapper">
<div class="theory" style="font-size: 19px;">

**(UFRGS 2018) Questão 14** - O gráfico de $f(x)$ está esboçado na imagem a seguir (vértice em $(0,5)$ e raízes $-3$ e $3$).

<div class="center" style="margin-top: 5px;">
<div class="svg-box">
<svg viewBox="0 0 300 200" width="220" height="150">
<defs>
<marker id="arrow3" markerWidth="10" markerHeight="10" refX="9" refY="3" orient="auto" markerUnits="strokeWidth">
<path d="M0,0 L0,6 L9,3 z" fill="#E0E0E0"/>
</marker>
</defs>
<line x1="20" y1="150" x2="280" y2="150" stroke="#E0E0E0" stroke-width="2" marker-end="url(#arrow3)"/>
<line x1="150" y1="180" x2="150" y2="20" stroke="#E0E0E0" stroke-width="2" marker-end="url(#arrow3)"/>
<!-- Parabola downwards: roots at x=90 (-3*20), x=210 (3*20). Vertex at (150, 50). Control point Y = -50 -->
<path d="M 60 200 Q 150 -100 240 200" fill="none" stroke="#E0E0E0" stroke-width="2"/>
<text x="80" y="140" fill="#E0E0E0" font-family="sans-serif" font-size="14" font-weight="bold">-3</text>
<text x="210" y="140" fill="#E0E0E0" font-family="sans-serif" font-size="14" font-weight="bold">3</text>
<text x="160" y="55" fill="#E0E0E0" font-family="sans-serif" font-size="14" font-weight="bold">5</text>
</svg>
</div>
</div>

A prova questiona qual das alternativas (que origalmente exibiam gráficos) representa o esboço correto da transformação $|f(x-3)| + 2$. 
*(Esboce a resolução gráfica preenchendo o raciocínio das translações na tela ao lado!)*

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 9. UFRGS 2012: O Gráfico de $z = |f(x)|$

<div class="content-wrapper">
<div class="theory" style="font-size: 19px;">

**(UFRGS 2012) Questão 25** - O gráfico a seguir é o gráfico da função $f$ definida por $y = f(x)$.

<div class="center" style="margin-top: 5px;">
<div class="svg-box">
<svg viewBox="0 0 300 200" width="220" height="150">
<defs>
<marker id="arrow4" markerWidth="10" markerHeight="10" refX="9" refY="3" orient="auto" markerUnits="strokeWidth">
<path d="M0,0 L0,6 L9,3 z" fill="#E0E0E0"/>
</marker>
</defs>
<line x1="20" y1="120" x2="280" y2="120" stroke="#E0E0E0" stroke-width="2" marker-end="url(#arrow4)"/>
<line x1="120" y1="180" x2="120" y2="20" stroke="#E0E0E0" stroke-width="2" marker-end="url(#arrow4)"/>
<!-- Parabola upwards. Roots at x=60 and x=240. Vertex at 150, 170. Control point Y = 220 -->
<path d="M 40 40 Q 150 250 260 40" fill="none" stroke="#E0E0E0" stroke-width="2"/>
<text x="285" y="115" fill="#E0E0E0" font-family="sans-serif" font-size="14">x</text>
<text x="100" y="25" fill="#E0E0E0" font-family="sans-serif" font-size="14">y</text>
</svg>
</div>
</div>

Então, das alternativas (que originalmente exibiam gráficos), a que pode representar o gráfico da função $z$, definida por $z = |f(x)|$, é:
*(Construa a resposta geométrica correta ao lado, demonstrando o efeito espelho do Módulo.)*

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>