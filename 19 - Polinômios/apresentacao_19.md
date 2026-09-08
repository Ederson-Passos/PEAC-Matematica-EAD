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
---
<div class="center">

# Matemática Pré-Vestibular
## AULA 19 - Polinômios e Expressões Algébricas

*(Aguardando o início da transmissão)*
</div>

---

# 1. Fundamentos e a Estrutura de $\mathbb{R}[x]$

<style scoped>
section { font-size: 19px; }
.example-box { font-size: 18px; margin-top: 5px; }
</style>

<div class="content-wrapper">
<div class="theory">

Um polinômio na variável $x$ é uma expressão algébrica estruturada pela soma de potências inteiras não negativas. Sua forma canônica é:
$$ P(x) = a_n x^n + a_{n-1} x^{n-1} + \dots + a_1 x + a_0 $$

- **Grau do Polinômio:** Definido pelo maior expoente $n$ cujo coeficiente $a_n$ seja não nulo.
- **Valor Numérico:** É o resultado obtido ao substituir a variável $x$ por um número constante $\alpha$. Se $P(\alpha) = 0$, dizemos que $\alpha$ é **raiz** do polinômio.
- **Identidade Polinomial:** Dois polinômios são idênticos ($P(x) \equiv Q(x)$) se, e somente se, todos os seus coeficientes de termos de mesmo grau forem iguais.

<div class="example-box">

**Exemplo 01:** Calcule a soma dos coeficientes do polinômio $P(x) = (3x^2 - 2x + 1)^3$. 
*(Dica de mestre: qual valor de $x$ faz a variável "desaparecer", deixando apenas os coeficientes?)*

</div>

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 2. Operações e Produtos Notáveis

<style scoped>
.theory { font-size: 20px; }
.theory ol { font-size: 18px; margin-bottom: 16px; }
.example-box { font-size: 16px; padding: 16px 12px; margin-top: 5px; }
</style>

<div class="content-wrapper">
<div class="theory">

Para operar polinômios com maestria, precisamos ir além da distribuição mecânica e reconhecer padrões geométricos clássicos. Os Produtos Notáveis são atalhos algébricos essenciais:

1. **Quadrado da Soma/Diferença:** $(a \pm b)^2 = a^2 \pm 2ab + b^2$
2. **Diferença de Quadrados:** $a^2 - b^2 = (a + b)(a - b)$
3. **Cubo da Soma/Diferença:** $(a \pm b)^3 = a^3 \pm 3a^2b + 3ab^2 \pm b^3$
4. **Soma/Diferença de Cubos:** $a^3 \pm b^3 = (a \pm b)(a^2 \mp ab + b^2)$

Fatorar um polinômio significa decompô-lo em seus blocos multiplicativos fundamentais, uma habilidade vital para simplificar divisões.

<div class="example-box">

**Exemplo 02:** Sem calcular o cubo de $101$ nem de $99$, determine o valor numérico exato da expressão algébrica: $\dfrac{101^3 - 99^3}{101 - 99}$

</div>

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 3. A Dinâmica da Divisão e o Teorema do Resto

<style scoped>
.theory { font-size: 20px; }
.theory ul { font-size: 18px; margin-bottom: 16px; }
.example-box { font-size: 16px; padding: 16px 12px; margin-top: 5px; }
</style>

<div class="content-wrapper">
<div class="theory">

Pelo Algoritmo de Euclides, ao dividir um polinômio $P(x)$ por $D(x)$, obtemos um quociente $Q(x)$ e um resto $R(x)$ únicos, tal que:
$$ P(x) = Q(x)D(x) + R(x) $$
A divisão cessa quando o $\text{grau}(R) < \text{grau}(D)$.

**Teorema do Resto (d'Alembert):**
Se dividirmos $P(x)$ por um binômio linear da forma $(x - a)$, o divisor se anula em $x = a$. Consequentemente, o resto numérico da divisão é simplesmente $R = P(a)$.

**Corolário (Teorema do Fator):**
Um polinômio $P(x)$ é divisível por $(x - a)$ se, e somente se, $a$ for raiz de $P(x)$.

<div class="example-box">

**Exemplo 03:** Determine o resto da divisão do polinômio gigantesco $P(x) = x^{2026} + 5x - 8$ pelo binômio $D(x) = x - 1$.

</div>

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 4. Espectro de Raízes e Relações de Girard

<div class="content-wrapper">
<div class="theory" style="font-size: 19px;">

Pelo **Teorema Fundamental da Álgebra**, todo polinômio de grau $n \ge 1$ possui exatamente $n$ raízes (reais ou complexas) e pode ser absolutamente fatorado como:
$$ P(x) = a_n(x - r_1)(x - r_2) \dots (x - r_n) $$

Ao expandirmos essa forma fatorada e compararmos com a forma canônica, emergem as **Relações de Girard (Viète)**, que conectam os coeficientes com somas e produtos de raízes, permitindo a análise de um sistema sem a necessidade de calcular as raízes individualmente.

<div class="example-box">

**Exemplo 04:** Partindo da forma fatorada $a(x - r_1)(x - r_2) = 0$, expanda a expressão e deduza, por si só, as clássicas fórmulas da Soma ($S$) e do Produto ($P$) das raízes de uma equação do 2º grau ($ax^2 + bx + c = 0$).

</div>

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 5. UFRGS 2024

<div class="content-wrapper">
<div class="theory" style="font-size: 19px;">

Se $n > 1$ é um número par, então o resto da divisão do polinômio $x^n - x + 2$ por $x - 1$ é

(A) $0$.
(B) $1$.
(C) $2$.
(D) $3$.
(E) $4$.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 6. UFRGS 2022

<div class="content-wrapper">
<div class="theory" style="font-size: 19px;">

O valor de $\dfrac{a^3 - b^3}{a - b}$ para $a = 27$ e $b = 26$ é

(A) $2017$.
(B) $2071$.
(C) $2107$.
(D) $2170$.
(E) $2710$.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 7. UFRGS 2021

<div class="content-wrapper">
<div class="theory" style="font-size: 19px;">

Se $a$ e $b$ são as raízes da equação $x^2 - 6x + 3 = 0$, então o valor de $\left( \dfrac{1}{\dfrac{1}{a} + \dfrac{1}{b}} \right)^{-2}$ é

(A) $2$.
(B) $4$.
(C) $6$.
(D) $8$.
(E) $10$.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 8. UFRGS 2018

<div class="content-wrapper">
<div class="theory" style="font-size: 19px;">

A soma dos coeficientes do polinômio $P(x) = (1 - x + x^2 - x^3 + x^4)^{1000}$ é

(A) $1$.
(B) $5$.
(C) $100$.
(D) $500$.
(E) $1000$.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 9. UFRGS 2017

<div class="content-wrapper">
<div class="theory" style="font-size: 19px;">

As raízes do polinômio $P(x) = x^4 - 1$ são

(A) $\{i; -i; 0\}$.
(B) $\{1; -1; 0\}$.
(C) $\{1; -1; i; -i\}$.
(D) $\{i; -i; 1+i; 1-i\}$.
(E) $\{i; -i; -1+i; -1-i\}$.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 10. UFRGS 2016

<div class="content-wrapper">
<div class="theory" style="font-size: 19px;">

Considere o polinômio $p$ definido por $p(x) = x^2 + 2(n+2)x + 9n$.

Se as raízes de $p(x) = 0$ são iguais, os valores de $n$ são

(A) $1$ e $4$.
(B) $2$ e $3$.
(C) $-1$ e $4$.
(D) $2$ e $4$.
(E) $1$ e $-4$.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 11. UFRGS 2014

<div class="content-wrapper">
<div class="theory" style="font-size: 19px;">

Considere o polinômio $p(x) = x^4 + 2x^3 - 7x^2 - 8x + 12$.

Se $p(2) = 0$ e $p(-2) = 0$, então as raízes do polinômio $p(x)$ são

(A) $-2$, $0$, $1$ e $2$.
(B) $-2$, $-1$, $2$ e $3$.
(C) $-2$, $-1$, $1$ e $2$.
(D) $-2$, $-1$, $0$ e $2$.
(E) $-3$, $-2$, $1$ e $2$.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>