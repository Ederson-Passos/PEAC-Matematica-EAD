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
## AULA 20 - Números Complexos

*(Aguardando o início da transmissão)*
</div>

---

# 1. A Necessidade dos Complexos e a Forma Algébrica

<style scoped>
section { font-size: 19px; }
.example-box { font-size: 18px; margin-top: 5px; }
</style>

<div class="content-wrapper">
<div class="theory">

Por muito tempo, equações como $x^2 + 1 = 0$ não tinham solução, pois não existia número real cujo quadrado fosse negativo. Para resolver isso, criou-se a **Unidade Imaginária ($i$)**, definida como:
$$ i^2 = -1 \quad \text{ou} \quad i = \sqrt{-1} $$

Todo número complexo $z$ pode ser escrito na **Forma Algébrica**:
$$ z = a + bi $$
Onde:
- $a$ é a **Parte Real**: $\text{Re}(z) = a$
- $b$ é a **Parte Imaginária**: $\text{Im}(z) = b$ *(Atenção: o $b$ é um número real, o $i$ fica de fora!)*.

Se $a = 0$, dizemos que $z$ é um *imaginário puro*. Se $b = 0$, $z$ é um *número real*.

<div class="example-box">

**Exemplo 01:** Para que o número complexo $z = (2x - 6) + (x + 1)i$ seja um número real, qual deve ser o valor de $x$? E para que ele seja imaginário puro?

</div>

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 2. Igualdade e Operações Básicas

<style scoped>
.theory { font-size: 20px; }
.example-box { font-size: 16px; padding: 16px 12px; margin-top: 5px; }
</style>

<div class="content-wrapper">
<div class="theory">

Trabalhar com números complexos é como trabalhar com polinômios usando a letra $x$, mas com a regra de ouro: **sempre que aparecer $i^2$, troque por $-1$**.

- **Igualdade:** Dois complexos são iguais se, e somente se, suas partes reais forem iguais e suas partes imaginárias também. $(a+bi = c+di \iff a=c \text{ e } b=d)$.
- **Soma/Subtração:** Somamos "real com real" e "imaginário com imaginário".
- **Multiplicação:** Fazemos a propriedade distributiva (o famoso "chuveirinho") e usamos a regra do $i^2$.

<div class="example-box">

**Exemplo 02:** Dados os números complexos $z_1 = 2 - 3i$ e $z_2 = 1 + 4i$:
a) Calcule a soma $z_1 + z_2$.
b) Calcule o produto $z_1 \cdot z_2$. *(Lembre-se da regra de ouro!)*

</div>

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 3. O Plano de Argand-Gauss e o Módulo

<style scoped>
.theory { font-size: 19px; }
.example-box { font-size: 17px; padding: 16px 12px; margin-top: 5px; }
</style>

<div class="content-wrapper">
<div class="theory">

Podemos representar um complexo $z = a + bi$ como um ponto $P(a, b)$ no plano cartesiano, chamado **Plano de Argand-Gauss**. O eixo $x$ representa a parte Real e o eixo $y$ a parte Imaginária.

O **Módulo** ($|z|$) é a distância da origem $(0,0)$ até o ponto $P(a, b)$. Usando o Teorema de Pitágoras, temos a fórmula:
$$ |z| = \sqrt{a^2 + b^2} $$
*(Note que não colocamos o $i$ dentro da raiz, usamos apenas os números $a$ e $b$).*

Uma propriedade muito útil em provas de vestibular: $|z_1 \cdot z_2| = |z_1| \cdot |z_2|$.

<div class="example-box">

**Exemplo 03:** Calcule o módulo do número complexo $z = 3 + 4i$. Em seguida, sem fazer distributiva gigantesca, determine o módulo de $W = (3+4i)^2$.

</div>

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 4. Conjugado e Raízes Complexas

<style scoped>
.theory { font-size: 19px; }
.theory ul { font-size: 18px; margin-bottom: 16px; }
.example-box { font-size: 16px; padding: 16px 12px; margin-top: 5px; }
</style>

<div class="content-wrapper">
<div class="theory">

O **Conjugado** de um complexo $z = a + bi$, representado por $\overline{z}$, é obtido trocando o sinal APENAS da parte imaginária: $\overline{z} = a - bi$.
- Multiplicar um número pelo seu conjugado sempre gera um número real: 
  $$ z \cdot \overline{z} = (a+bi)(a-bi) = a^2 + b^2 $$

**Teorema das Raízes Complexas:**
Se um número complexo $z = a+bi$ for raiz de um polinômio com coeficientes reais, então o seu conjugado $\overline{z} = a-bi$ **obrigatoriamente** também será raiz desse polinômio. As raízes complexas sempre andam de mãos dadas em pares!

<div class="example-box">

**Exemplo 04:** Um polinômio do 3º grau com coeficientes reais tem como raízes o número $5$ e o número $1 + 2i$. Qual é, obrigatoriamente, a terceira raiz desse polinômio?

</div>

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 5. UFRGS 2023

<div class="content-wrapper">
<div class="theory" style="font-size: 18px;">

Considere as seguintes afirmações sobre números complexos.

I. O módulo de $z = 3 + 4i$ é $|z| = 5$.
II. Se $u = 1 + i$ e $v = 1 - i$, então $|u \cdot v| = |u| \cdot |v|$.
III. Para que $w = (x - 3) + (x + 4)i$ seja um número real, é necessário e suficiente que $x = 3$.

Quais estão corretas?

(A) Apenas I.
(B) Apenas III.
(C) Apenas I e II.
(D) Apenas II e III.
(E) I, II e III.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 6. UFRGS 2018

<div class="content-wrapper">
<div class="theory" style="font-size: 19px;">

Dados os números complexos $z_1 = (2, -1)$ e $z_2 = (3, x)$, sabe-se que $z_1 \cdot z_2 \in \mathbb{R}$. Então $x$ é igual a

*(Dica: A notação de par ordenado $(a,b)$ é apenas outra forma de escrever $a + bi$. Ou seja, $z_1 = 2 - i$)*

(A) $-6$.
(B) $-\dfrac{3}{2}$.
(C) $0$.
(D) $\dfrac{3}{2}$.
(E) $6$.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 7. UFRGS 2017

<div class="content-wrapper">
<div class="theory" style="font-size: 18px;">

Considere as seguintes afirmações sobre números complexos.

I. $(2+i)(2-i)(1+i)(1-i) = 10$.
II. $\left(\dfrac{7}{2} + \dfrac{1}{3}i\right) + \left(\dfrac{3}{2} + \dfrac{2}{3}i\right) = \dfrac{5}{2} + \dfrac{1}{2}i$.
III. Se o módulo do número complexo $z$ é $5$, então o módulo de $2z$ é $10$.

Quais afirmações estão corretas?

(A) Apenas I.
(B) Apenas II.
(C) Apenas III.
(D) Apenas I e III.
(E) I, II e III.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 8. UFRGS 2017

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

# 9. UFRGS 2016

<div class="content-wrapper">
<div class="theory" style="font-size: 18px;">

Considere as igualdades abaixo.

I. $(1 - 2i)(1 + 2i) = 5$, sendo $i$ a unidade imaginária.
II. $2^0 + 2^{-1} + 2^{-2} + 2^{-3} + \dots = 2$
III. $1 - 2 + 3 - 4 + 5 - 6 + \dots + 99 - 100 = 50$

Quais igualdades são verdadeiras?

(A) Apenas I.
(B) Apenas III.
(C) Apenas I e II.
(D) Apenas II e III.
(E) I, II e III.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 10. UFRGS 2010

<div class="content-wrapper">
<div class="theory" style="font-size: 19px;">

Um polinômio de $5^\circ$ grau com coeficientes reais que admite os números complexos $-2+i$ e $1-2i$ como raízes, admite

(A) no máximo mais uma raiz complexa.
(B) $2-i$ e $-1+2i$ como raízes.
(C) uma raiz real.
(D) duas raízes reais distintas.
(E) três raízes reais distintas.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>