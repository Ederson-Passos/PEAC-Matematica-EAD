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
    /* Cria pontos de 2px a cada 30px de distância */
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

  /* 3. TIPOGRAFIA MINIMALISTA (Títulos pequenos no topo) */
  h1 {
    color: #8BE9FD; /* Um ciano suave para destacar sem cegar */
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

  /* 4. LISTAS INVISÍVEIS */
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
    margin-bottom: 25px; /* Espaço maior para escrever com a Wacom */
  }

  /* Classes utilitárias para quando quiser centralizar um texto */
  .center { text-align: center; }

---
<div class="center">

# Matemática Pré-Vestibular
## Encontro 02: Potenciação, Radiciação e Notação Científica

<br><br>
*(Aguardando o início da transmissão)*
</div>

---

# 1. Potenciação

A potenciação é uma multiplicação sucessiva. Seja $a \in \mathbb{R}$ e $n \in \mathbb{N}$:

$$a^n = \underbrace{a \cdot a \cdot a \cdots a}_{n \text{ vezes}}$$

Onde,
* $a$ é a **Base**
* $n$ é o **Expoente**

Exemplo:
<div class="sem-bolinha">

* $2^3=$
* $(\frac{2}{3})^4=$
* $(-3)^3=$

</div>

---

# 1.1 Propriedades Operatórias

Sejam $a, b \in \mathbb{R}$ e $m, n \in \mathbb{R}$:

* Produto de mesma base:
  $$ a^m \cdot a^n = a^{m+n} $$

* Quociente de mesma base:
  $$ \frac{a^m}{a^n} = a^{m-n} $$

* Potência de potência:
  $$ \left( a^m \right)^n = a^{m \cdot n} $$

* Distribuição no Produto/Quociente:
  $$ (a \cdot b)^n = a^n \cdot b^n $$
  $$ \left(\frac{a}{b} \right)^n = \frac{a^n}{b^n} $$

---

# 1.1 Propriedades Operatórias

Exemplo:
<div class="sem-bolinha">

* $10^2 \cdot 10^5 =$
<br><br>
* $\frac{10^5}{10^2} =$
<br><br>
* $(10^2)^5 =$
<br><br>
* 

</div>

___

# 1.1 Propriedades Operatórias

Com a propriedade do quociente de mesma base podemos determinar o resultado para potências de expoente 0, vejamos:

<br><br>
<br><br>

<div class="sem-bolinha">

* Assim, temos que para qualquer $a \in \mathbb{R}$ e $n = 0$:
  $$ a^n = 1 $$

</div>

___

# 1.2 Expoente Negativo

Para expoentes negativos podemos expandir a regra usando a propriedade do quociente de mesma base.

<br><br>
<br><br>

<div class="sem-bolinha">

* Regra prática: o expoente negativo inverte a base.
  $$ \left(\frac{a}{b} \right)^{-n} = \left(\frac{b}{a} \right)^n $$

</div>

---

# 1.2 Expoente Negativo

Exemplo:
<div class="sem-bolinha">

* $2^{-2} =$
  <br><br>
* $\left(\frac{2}{3} \right)^{-3} =$
  <br><br>
* $(0,5)^{-2} =$
* 

</div>

---

# 2. Radiciação

A radiciação é a operação inversa da potenciação. Sendo $a \in \mathbb{R}$ e $n \in \mathbb{N}$, com $n \ge 1$:

$$\sqrt[n]{a} = x \iff x^n = a$$

Onde:
* $n$ é o **Índice**
* $a$ é o **Radicando**
* $\sqrt{\phantom{x}}$ é o **Radical**

---

# 2. Radiciação

Exemplo:
<div class="sem-bolinha">

* $\sqrt{4} =$
  <br><br><br>
* $\sqrt[3]{-8} =$
  <br><br><br>
* $\sqrt[4]{\frac{64}{625}} =$

</div>

---

# 2.1 Propriedades Operatórias

Sejam $a, b \in \mathbb{R}$ (condicionados à existência da raiz) e $m, n \in \mathbb{N}$:

* Produto de raízes de mesmo índice:
  $$\sqrt[n]{a \cdot b} = \sqrt[n]{a} \cdot \sqrt[n]{b}$$

* Quociente de raízes de mesmo índice:
  $$\sqrt[n]{\frac{a}{b}} = \frac{\sqrt[n]{a}}{\sqrt[n]{b}}$$

* Potência de expoente fracionário (A ponte entre raiz e potência):
  $$\sqrt[n]{a^m} = a^{\frac{m}{n}}$$

* Raiz de raiz:
  $$\sqrt[m]{\sqrt[n]{a}} = \sqrt[m \cdot n]{a}$$

---

# 2.1 Propriedades Operatórias

Exemplo:
<div class="sem-bolinha">

* $\sqrt{2} \cdot \sqrt{8} =$
  <br><br>
* $\frac{\sqrt[3]{16}}{\sqrt[3]{2}} =$
  <br><br>
* $8^{\frac{1}{3}} =$
  <br><br>
* $\sqrt{\sqrt[3]{64}} =$

</div>

---

# 2.1 Propriedades Operatórias

Exemplo: Vamos simplificar as expressões.
<div class="sem-bolinha">

* $\sqrt{2} + \sqrt{8} =$
  <br><br>
* $\frac{3}{\sqrt{2}} =$
  <br><br>
* $\frac{4}{\sqrt{3}-1} =$
  <br><br>

</div>

---

# 3. Notação Científica

A notação científica é a padronização para escrever números muito grandes (Astronomia, Engenharia, Geologia) ou muito pequenos (Mecânica Quântica, Química) utilizando potências de base 10.

A forma canônica é:
$$N = m \cdot 10^e$$

Onde:
* $m$ é a **Mantissa** (condição: $1 \le m < 10$)
* $e$ é a **Ordem de Grandeza** (um número inteiro, $e \in \mathbb{Z}$)

---

# 3.1 Conversão (A Dança da Vírgula)

A regra mecânica para manter o equilíbrio numérico:
* Se a vírgula anda para a **esquerda** (você diminui o número), o expoente **aumenta** ($+$).
* Se a vírgula anda para a **direita** (você aumenta o número), o expoente **diminui** ($-$).

Exemplo: Converta para Notação Científica
<div class="sem-bolinha">

* $345.000 =$
  <br>
* $0,000078 =$
  <br>
* $145 \cdot 10^4 =$  

</div>

---

# 3.2 Operações em Notação Científica

Aplicamos as propriedades da potenciação separadamente: operamos mantissa com mantissa e potência com potência.

Exemplo: Calcule e expresse o resultado final em notação científica.
<div class="sem-bolinha">

* $(3 \cdot 10^5) \cdot (2 \cdot 10^4) =$
  <br><br>
* $\frac{8 \cdot 10^3}{4 \cdot 10^7} =$
  <br><br>
* $(2 \cdot 10^3)^3 =$

</div>