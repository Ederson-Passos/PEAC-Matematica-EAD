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
## AULA 17 - Função e Equação Logarítmica

*(Aguardando o início da transmissão)*
</div>

---

# 1. O que é um Logaritmo?

<style scoped>
section { font-size: 19px; }
.example-box { font-size: 18px; margin-top: 5px; }
</style>

<div class="content-wrapper">
<div class="theory">

O logaritmo é, em sua essência, a operação inversa da exponencial. Ele responde a uma pergunta direta: *a qual expoente devemos elevar a base para obter um determinado número?*

Definimos matematicamente como:
$$ \log_a b = x \iff a^x = b $$

**Condições de Existência (C.E.):**
Para a operação ser bem definida no conjunto dos números reais, exigimos que:
- A base $a$ seja positiva e diferente de 1 ($a > 0$ e $a \neq 1$).
- O logaritmando $b$ seja estritamente positivo ($b > 0$).

<div class="example-box">

**Exemplo 01:** Compreendendo a definição geométrica e algébrica, calcule o valor numérico da expressão $\log_2 32 + \log_3 81$.

</div>

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 2. Propriedades Operatórias

<div class="content-wrapper">
<div class="theory" style="font-size: 19px;">

As propriedades logarítmicas são ferramentas poderosas para simplificar equações complexas, transformando multiplicações em adições e divisões em subtrações. 

1. **Logaritmo do Produto:** $\log_a (b \cdot c) = \log_a b + \log_a c$
2. **Logaritmo do Quociente:** $\log_a \left(\dfrac{b}{c}\right) = \log_a b - \log_a c$
3. **Logaritmo da Potência:** $\log_a (b^n) = n \cdot \log_a b$
4. **Mudança de Base:** $\log_a b = \dfrac{\log_c b}{\log_c a}$

<div class="example-box">

**Exemplo 02:** Sabendo que $\log 2 = 0{,}3$ e $\log 3 = 0{,}48$, utilize as propriedades para decompor e determinar o valor de $\log 12$.

</div>

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 3. Equações Logarítmicas

<div class="content-wrapper">
<div class="theory" style="font-size: 19px;">

Para resolver equações logarítmicas, o objetivo central é aplicar as propriedades para obter uma **Igualdade de Bases**. Se tivermos o mesmo logaritmo em ambos os lados, igualamos os logaritmandos:

$$ \log_a x = \log_a y \implies x = y $$

**Atenção Absoluta:** O conjunto solução de uma equação logarítmica está sempre submetido à sua Condição de Existência (C.E.). Após encontrar as raízes algébricas, é imprescindível testá-las para garantir que nenhum logaritmando resulte em zero ou em valor negativo.

<div class="example-box">

**Exemplo 03:** Resolva a equação no conjunto dos números reais, indicando sua C.E.:
$$\log_2(x - 3) + \log_2(x + 3) = 4$$

</div>

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 4. A Função Logarítmica e seu Gráfico

<div class="content-wrapper">
<div class="theory" style="font-size: 18px;">

A função $f(x) = \log_a x$ é a inversa geométrica da função exponencial $y = a^x$ (refletida em relação à reta $y = x$). Sua curva sempre intercepta o eixo horizontal no ponto $(1, 0)$ e aproxima-se assintoticamente do eixo $y$ sem jamais tocá-lo.

<div class="flex-around">

<div class="center crescente-text">

Crescente ($a > 1$)

<div class="svg-box">
<img src="data:image/svg+xml;utf8,%3Csvg%20viewBox%3D%220%200%20200%20150%22%20width%3D%22180%22%20height%3D%22135%22%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%3E%0A%20%20%3Cdefs%3E%0A%20%20%20%20%3Cmarker%20id%3D%22arrow1%22%20markerWidth%3D%2210%22%20markerHeight%3D%2210%22%20refX%3D%229%22%20refY%3D%223%22%20orient%3D%22auto%22%20markerUnits%3D%22strokeWidth%22%3E%0A%20%20%20%20%20%20%3Cpath%20d%3D%22M0%2C0%20L0%2C6%20L9%2C3%20z%22%20fill%3D%22%23E0E0E0%22/%3E%0A%20%20%20%20%3C/marker%3E%0A%20%20%3C/defs%3E%0A%20%20%3Cline%20x1%3D%2220%22%20y1%3D%22110%22%20x2%3D%22190%22%20y2%3D%22110%22%20stroke%3D%22%23E0E0E0%22%20stroke-width%3D%222%22%20marker-end%3D%22url%28%23arrow1%29%22/%3E%0A%20%20%3Cline%20x1%3D%2280%22%20y1%3D%22140%22%20x2%3D%2280%22%20y2%3D%2210%22%20stroke%3D%22%23E0E0E0%22%20stroke-width%3D%222%22%20marker-end%3D%22url%28%23arrow1%29%22/%3E%0A%20%20%3Cpolyline%20points%3D%2285%20160%2C%2092.5%20135%2C%20105%20110%2C%20117.5%2095.5%2C%20130%2085%2C%20155%2070.5%2C%20180%2060%22%20fill%3D%22none%22%20stroke%3D%22%2350fa7b%22%20stroke-width%3D%223%22%20stroke-linejoin%3D%22round%22/%3E%0A%20%20%3Ctext%20x%3D%22100%22%20y%3D%22125%22%20fill%3D%22%23E0E0E0%22%20font-size%3D%2212%22%3E1%3C/text%3E%0A%20%20%3Ccircle%20cx%3D%22105%22%20cy%3D%22110%22%20r%3D%223%22%20fill%3D%22%23E0E0E0%22/%3E%0A%3C/svg%3E">
</div>
</div>

<div class="center decrescente-text">

Decrescente ($0 < a < 1$)

<div class="svg-box">
<img src="data:image/svg+xml;utf8,%3Csvg%20viewBox%3D%220%200%20200%20150%22%20width%3D%22180%22%20height%3D%22135%22%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%3E%0A%20%20%3Cdefs%3E%0A%20%20%20%20%3Cmarker%20id%3D%22arrow2%22%20markerWidth%3D%2210%22%20markerHeight%3D%2210%22%20refX%3D%229%22%20refY%3D%223%22%20orient%3D%22auto%22%20markerUnits%3D%22strokeWidth%22%3E%0A%20%20%20%20%20%20%3Cpath%20d%3D%22M0%2C0%20L0%2C6%20L9%2C3%20z%22%20fill%3D%22%23E0E0E0%22/%3E%0A%20%20%20%20%3C/marker%3E%0A%20%20%3C/defs%3E%0A%20%20%3Cline%20x1%3D%2220%22%20y1%3D%22110%22%20x2%3D%22190%22%20y2%3D%22110%22%20stroke%3D%22%23E0E0E0%22%20stroke-width%3D%222%22%20marker-end%3D%22url%28%23arrow2%29%22/%3E%0A%20%20%3Cline%20x1%3D%2280%22%20y1%3D%22140%22%20x2%3D%2280%22%20y2%3D%2210%22%20stroke%3D%22%23E0E0E0%22%20stroke-width%3D%222%22%20marker-end%3D%22url%28%23arrow2%29%22/%3E%0A%20%20%3Cpolyline%20points%3D%2285%2060%2C%2092.5%2085%2C%20105%20110%2C%20117.5%20124.5%2C%20130%20135%2C%20155%20149.5%2C%20180%20160%22%20fill%3D%22none%22%20stroke%3D%22%23ff79c6%22%20stroke-width%3D%223%22%20stroke-linejoin%3D%22round%22/%3E%0A%20%20%3Ctext%20x%3D%22100%22%20y%3D%22125%22%20fill%3D%22%23E0E0E0%22%20font-size%3D%2212%22%3E1%3C/text%3E%0A%20%20%3Ccircle%20cx%3D%22105%22%20cy%3D%22110%22%20r%3D%223%22%20fill%3D%22%23E0E0E0%22/%3E%0A%3C/svg%3E">
</div>
</div>

</div>

<div class="example-box" style="font-size: 18px;">

**Exemplo 04:** Utilizando os conceitos de análise de domínio, determine o intervalo real para o qual a função $f(x) = \log_5(2x - 10)$ está definida.

</div>

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 5. UFRGS 2025:

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

# 6. UFRGS 2025:

<div class="content-wrapper">
<div class="theory" style="font-size: 19px;">

A equação $\log(x) + \log(x - 1) = \log 6$ tem conjunto solução nos números reais. 

O conjunto solução da equação é

(A) $\{-2\}$.
(B) $\{3\}$.
(C) $\{3, 2\}$.
(D) $\{3, -2\}$.
(E) $\{-3, -2\}$.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 7. UFRGS 2024:

<div class="content-wrapper">
<div class="theory" style="font-size: 19px;">

O valor da expressão 
$\log(2024) - \log(202{,}4) + \log(20{,}24) - \log(2{,}024)$ é

(A) $4$.
(B) $2$.
(C) $0$.
(D) $-2$.
(E) $-4$.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 8. UFRGS 2023:

<div class="content-wrapper">
<div class="theory" style="font-size: 15px;">

A figura abaixo mostra o início de uma sequência infinita de quadrados. A medida dos lados dos quadrados $Q_1$, $Q_2$ e $Q_3$ são, respectivamente, $\log(2)$, $\log(\sqrt{2})$ e $\log(\sqrt[4]{2})$.

<div class="center svg-box" style="margin: 10px 0;">
<img src="data:image/svg+xml;utf8,%3Csvg%20viewBox%3D%220%200%20220%20100%22%20width%3D%22220%22%20height%3D%22100%22%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%3E%0A%20%20%3Crect%20x%3D%2210%22%20y%3D%2210%22%20width%3D%2260%22%20height%3D%2260%22%20fill%3D%22none%22%20stroke%3D%22%23E0E0E0%22%20stroke-width%3D%222%22/%3E%0A%20%20%3Ctext%20x%3D%2240%22%20y%3D%2290%22%20fill%3D%22%23E0E0E0%22%20font-size%3D%2214%22%20text-anchor%3D%22middle%22%3EQ1%3C/text%3E%0A%20%20%3Crect%20x%3D%2280%22%20y%3D%2240%22%20width%3D%2230%22%20height%3D%2230%22%20fill%3D%22none%22%20stroke%3D%22%23E0E0E0%22%20stroke-width%3D%222%22/%3E%0A%20%20%3Ctext%20x%3D%2295%22%20y%3D%2290%22%20fill%3D%22%23E0E0E0%22%20font-size%3D%2214%22%20text-anchor%3D%22middle%22%3EQ2%3C/text%3E%0A%20%20%3Crect%20x%3D%22120%22%20y%3D%2255%22%20width%3D%2215%22%20height%3D%2215%22%20fill%3D%22none%22%20stroke%3D%22%23E0E0E0%22%20stroke-width%3D%222%22/%3E%0A%20%20%3Ctext%20x%3D%22127.5%22%20y%3D%2290%22%20fill%3D%22%23E0E0E0%22%20font-size%3D%2214%22%20text-anchor%3D%22middle%22%3EQ3%3C/text%3E%0A%20%20%3Ctext%20x%3D%22155%22%20y%3D%2265%22%20fill%3D%22%23E0E0E0%22%20font-size%3D%2216%22%3E...%3C/text%3E%0A%3C/svg%3E">
</div>

A soma das áreas dessa sequência infinita de quadrados é

(A) $\dfrac{1}{3} \cdot [\log(2)]^2$.
(B) $\dfrac{4}{3} \cdot [\log(2)]^2$.
(C) $\dfrac{2}{3} \cdot [\log(2)]^2$.
(D) $\log(2 + \sqrt{2} + \sqrt[4]{2})$.
(E) $\log(2 \cdot \sqrt{2} \cdot \sqrt[4]{2})$.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 9. UFRGS 2022:

<div class="content-wrapper">
<div class="theory" style="font-size: 19px;">

O valor de $\log(2^2) + \log(2^3) + \log(2^4) + \dots + \log(2^{50})$ é

(A) $\log(2^{1247})$.
(B) $\log(2^{1274})$.
(C) $\log(2^{1472})$.
(D) $\log(2^{59})$.
(E) $\log(8^{59})$.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 10. UFRGS 2017:

<style scoped>
section { font-size: 20px; }
</style>

<div class="content-wrapper">
<div class="theory">

Leia o texto abaixo, sobre terremotos.

Magnitude é uma medida quantitativa do tamanho do terremoto. Ela está relacionada com a energia sísmica liberada no foco e também com a amplitude das ondas registradas pelos sismógrafos. Para cobrir todos os tamanhos de terremotos, desde os microtremores de magnitudes negativas até os grandes terremotos com magnitudes superiores a 8.0, foi idealizada uma escala logarítmica, sem limites. (...) Magnitude e energia podem ser relacionadas pela fórmula descrita por Gutenberg e Richter em 1935: $\log(E) = 11{,}8 + 1{,}5M$ onde: $E =$ energia liberada em *Erg* ; $M =$ magnitude do terremoto.

Sabendo que o terremoto que atingiu o México em setembro de 2017 teve magnitude 8,2, assinale a alternativa que representa a melhor aproximação para a energia liberada por esse terremoto, em *Erg*.

(A) $13{,}3$
(B) $20$
(C) $24$
(D) $10^{24}$
(E) $10^{28}$

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>
