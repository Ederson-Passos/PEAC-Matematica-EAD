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
## AULA 13 - Noções de Função, Função Linear e Função Afim

*(Aguardando o início da transmissão)*
</div>

---

# 1. Noções de Função: Domínio, Contradomínio e Imagem

<div class="content-wrapper">
<div class="theory">

No rigor algébrico, uma **função** $f: A \to B$ é uma regra determinística de mapeamento. Ela associa a **cada** elemento $x$ do conjunto $A$ um **único** elemento $y$ do conjunto $B$.

* **Domínio ($D$):** O conjunto $A$. É o espaço das variáveis independentes (as "entradas" permitidas).
* **Contradomínio ($CD$):** O conjunto $B$. É o espaço topológico que abriga as possíveis saídas.
* **Imagem ($Im$):** Um subconjunto do Contradomínio ($Im \subseteq CD$). Representa exclusivamente os valores que são efetivamente atingidos pela função.

</div>
<div class="resolution">

</div>
</div>

---

# 1.1 Exemplo: Noções de Função

<div class="content-wrapper">
<div class="theory">

Para consolidar a visão de conjuntos antes de irmos para o plano cartesiano continuo ($\mathbb{R}^2$):

<div class="example-box">

**Exemplo 01:** Seja a função $f: A \to B$, com $A = \{-1, 0, 1, 2\}$, $B = \{0, 1, 2, 3, 4, 5\}$ e a lei de formação $f(x) = x^2$. 
Determine rigorosamente o Domínio, o Contradomínio e o conjunto Imagem desta função.

</div>


</div>
<div class="resolution">

</div>
</div>

---

# 2. A Função Linear e a Função Afim

<div class="content-wrapper">
<div class="theory" style="font-size: 21px;">

**Função Linear:** Tem a forma $f(x) = ax$, com $a \neq 0$. Ela expressa uma **proporcionalidade direta** rigorosa. O seu gráfico é uma reta que passa *obrigatoriamente* pela origem $(0,0)$. 

**Função Afim:** Tem a forma $f(x) = ax + b$, com $a \neq 0$ e $b \neq 0$. Ela é uma transformação (translação) geométrica da função linear. A reta é deslocada verticalmente no plano.
* **$a$ (Coeficiente Angular):** Representa a Taxa de Variação (a derivada da reta). Define a inclinação.
* **$b$ (Coeficiente Linear):** É o ponto de intersecção com o eixo das ordenadas ($y$). Onde a "história começa" para $x = 0$.

</div>
<div class="resolution">

</div>
</div>

---

# 2.1 Exemplo: Construção Algébrica

<div class="content-wrapper">
<div class="theory">

Na prática analítica, uma reta fica perfeitamente determinada se conhecermos dois de seus pontos distintos no plano cartesiano.

<div class="example-box">

**Exemplo 02:** Sabemos que o gráfico de uma função afim $f(x) = ax + b$ passa pelos pontos $A(1, 5)$ e $B(3, 11)$. Calcule os coeficientes $a$ e $b$ e defina a lei da função.

</div>

</div>
<div class="resolution">

</div>
</div>

---

# 3. Gráfico da Função Afim: Crescimento e Zero

<div class="content-wrapper">
<div class="theory" style="font-size: 21px;">

A geometria de $f(x) = ax + b$ é governada exclusivamente pelos seus coeficientes:

* **Função Crescente ($a > 0$):** À medida que o valor de $x$ aumenta, o valor de $f(x)$ também aumenta. O ângulo de inclinação em relação ao eixo $x$ é agudo.
* **Função Decrescente ($a < 0$):** À medida que $x$ aumenta, $f(x)$ diminui. O ângulo de inclinação é obtuso.

**O Zero da Função (Raiz):**
É o ponto topológico onde a reta corta o eixo das abscissas (eixo $x$). Ocorre estritamente quando o sistema atinge o equilíbrio neutro, ou seja, $f(x) = 0$.
$$ax + b = 0 \implies x = -\frac{b}{a}$$

</div>
<div class="resolution">

</div>
</div>

---

# 4. O Estudo de Sinal da Função Afim

<div class="content-wrapper">
<div class="theory" style="font-size: 20px;">

Estudar o sinal significa determinar para quais intervalos do domínio $x$ o gráfico da função está **acima** do eixo $x$ ($y > 0$), **abaixo** do eixo $x$ ($y < 0$) ou **sobre** o eixo ($y = 0$).

A raiz $x = -\frac{b}{a}$ atua como o ponto de transição geométrica ("fronteira" de fase).

<div class="center" style="margin-top: 10px;">
  <div class="svg-box">
  <svg viewBox="0 0 400 150" width="350" height="130">
    <!-- Eixo X crescente -->
    <line x1="20" y1="75" x2="180" y2="75" stroke="#E0E0E0" stroke-width="2" marker-end="url(#arrow)"/>
    <line x1="40" y1="130" x2="160" y2="20" stroke="#8BE9FD" stroke-width="3"/>
    <circle cx="100" cy="75" r="4" fill="#FF79C6"/>
    <text x="100" y="95" fill="#E0E0E0" font-size="14" text-anchor="middle" font-family="sans-serif">Raiz (-b/a)</text>
    <text x="130" y="55" fill="#50FA7B" font-size="20" font-weight="bold">+</text>
    <text x="60" y="95" fill="#FF5555" font-size="20" font-weight="bold">-</text>
    <text x="100" y="15" fill="#E0E0E0" font-size="14" text-anchor="middle" font-family="sans-serif">a &gt; 0 (Crescente)</text>
    <!-- Eixo X decrescente -->
    <line x1="220" y1="75" x2="380" y2="75" stroke="#E0E0E0" stroke-width="2" marker-end="url(#arrow)"/>
    <line x1="240" y1="20" x2="360" y2="130" stroke="#8BE9FD" stroke-width="3"/>
    <circle cx="300" cy="75" r="4" fill="#FF79C6"/>
    <text x="300" y="95" fill="#E0E0E0" font-size="14" text-anchor="middle" font-family="sans-serif">Raiz (-b/a)</text>
    <text x="270" y="55" fill="#50FA7B" font-size="20" font-weight="bold">+</text>
    <text x="340" y="95" fill="#FF5555" font-size="20" font-weight="bold">-</text>
    <text x="300" y="15" fill="#E0E0E0" font-size="14" text-anchor="middle" font-family="sans-serif">a &lt; 0 (Decrescente)</text>
  </svg>
  </div>
</div>

</div>
<div class="resolution">

</div>
</div>

---

# 4.1 Exemplo: Gráfico, Zero e Sinal

<div class="content-wrapper">
<div class="theory">

Vamos operacionalizar toda a teoria visualizada até aqui.

<div class="example-box">

**Exemplo 03:** Dada a função afim $f(x) = -2x + 8$.
a) Identifique se ela é crescente ou decrescente.
b) Calcule o zero da função (a raiz).
c) Onde a função intercepta o eixo $y$?
d) Faça o estudo do sinal desta função.

</div>

</div>
<div class="resolution">

</div>
</div>

---

# 5. Problemas Contextualizados Envolvendo Função Afim

<div class="content-wrapper">
<div class="theory">

A função afim é o modelo matemático perfeito para fenômenos que possuem **taxas de crescimento constantes** (velocidade constante, tarifa por metro, juros simples).

Ao ler um problema contextualizado (estilo ENEM e UFRGS), desmonte o texto para encontrar o padrão $y = ax + b$:

* **$b$ (Fixo):** Procure palavras como "taxa fixa", "custo inicial", "bandeirada", "despesa constante". É o valor de largada quando $x = 0$.
* **$ax$ (Variável):** Procure palavras associadas a taxas unitárias: "R$ por quilômetro", "gotas por segundo", "custo por unidade". É o multiplicador da sua variável.

</div>
<div class="resolution">

</div>
</div>

---

# 5.1 Exemplo: Modelagem Algébrica

<div class="content-wrapper">
<div class="theory">

<div class="example-box">

**Exemplo 04:** Um vendedor recebe um salário mensal composto de uma parte fixa de R$ 1.200,00 e mais uma comissão de 5% sobre o total em reais das vendas que ele efetuar durante o mês.
a) Determine a lei de formação da função $S(x)$ que representa o salário mensal em função das vendas $x$.
b) Se ele vender R$ 10.000,00 no mês, qual será seu salário?

</div>

</div>
<div class="resolution">

</div>
</div>

---

# 6. UFRGS 2017

<div class="content-wrapper">
<div class="theory" style="font-size: 21px;">

Para produzir determinado tipo de tecido, uma fábrica gasta R$ 2,20 por metro. Além disso, há uma despesa fixa de R$ 2.500,00, independente da quantidade de metros produzidos. Se cada metro do tecido é vendido por R$ 4,00, o número mínimo de metros no qual a fábrica passa a ter lucro com a venda é:

<br>

(A) 1388. <br>
(B) 1389. <br>
(C) 1390. <br>
(D) 1391. <br>
(E) 1392.

</div>
<div class="resolution">

</div>
</div>

---

# 7. UFRGS 2025

<div class="content-wrapper">
<div class="theory" style="font-size: 21px;">

Considere as funções $f, g$ e $h$ definidas por $f(x) = x - 2$, $g(x) = -x + 2$ e $h(x) = 2$, desenhadas em um único sistema de coordenadas cartesianas. A área da região compreendida entre os gráficos das funções $f(x)$, $g(x)$ e $h(x)$ é:

<br><br>

(A) 4. <br>
(B) 6. <br>
(C) 8. <br>
(D) 10. <br>
(E) 16.

</div>
<div class="resolution">

</div>
</div>

---

# 8. UFRGS 2018

<div class="content-wrapper">
<div class="theory" style="font-size: 21px;">

Considere as seguintes afirmações sobre quaisquer funções $f$ reais de variável real.

<br>

I - Se $x \in \mathbb{R}$ e $x > 0$, então $f(x) > 0$.<br>
II - Se $f(x) = 0$, então $x$ é zero da função $f(x)$.<br>
III - Se $x_1$ e $x_2$ são números reais, com $x_1 < x_2$, então $f(x_1) < f(x_2)$.

<br>

Quais estão corretas?

<br>

(A) Apenas I. <br>
(B) Apenas II. <br>
(C) Apenas III. <br>
(D) Apenas I e II. <br>
(E) I, II e III.

</div>
<div class="resolution">

</div>
</div>

---

# 9. UFRGS 2010

<div class="content-wrapper">
<div class="theory" style="font-size: 21px;">

Uma torneira com vazamento pinga, de maneira constante, 25 gotas de água por minuto. Se cada gota contém $0,2\text{ mL}$ de água, então, em 24 horas o vazamento será de:

<br><br>

(A) $0,072\text{ L}$. <br>
(B) $0,72\text{ L}$. <br>
(C) $1,44\text{ L}$. <br>
(D) $7,2\text{ L}$. <br>
(E) $14,4\text{ L}$.

</div>
<div class="resolution">

</div>
</div>

---
