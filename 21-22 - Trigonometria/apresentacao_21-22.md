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
## AULAS 21 e 22 - Trigonometria

*(Aguardando o início da transmissão)*
</div>

---

# 1. Trigonometria no Triângulo Retângulo e Ângulos Notáveis

<style scoped>
section { font-size: 19px; }
.example-box { font-size: 18px; margin-top: 5px; }
</style>

<div class="content-wrapper">
<div class="theory">

No triângulo retângulo, relacionamos os lados (catetos e hipotenusa) com seus ângulos internos. Sendo $\alpha$ um ângulo agudo:
- **Seno:** $\sin(\alpha) = \frac{\text{Cateto Oposto}}{\text{Hipotenusa}}$
- **Cosseno:** $\cos(\alpha) = \frac{\text{Cateto Adjacente}}{\text{Hipotenusa}}$
- **Tangente:** $\tan(\alpha) = \frac{\text{Cateto Oposto}}{\text{Cateto Adjacente}}$

**Ângulos Notáveis ($30^\circ, 45^\circ, 60^\circ$):**
| Ângulo | $30^\circ$ | $45^\circ$ | $60^\circ$ |
|---|---|---|---|
| Seno | $1/2$ | $\sqrt{2}/2$ | $\sqrt{3}/2$ |
| Cosseno | $\sqrt{3}/2$ | $\sqrt{2}/2$ | $1/2$ |
| Tangente | $\sqrt{3}/3$ | $1$ | $\sqrt{3}$ |

<div class="example-box">

**Exemplo 01:** O topo de uma torre é visto sob um ângulo de $60^\circ$ por um observador a $30$ metros de distância da sua base. Desprezando a altura do observador, qual é a altura da torre?

</div>

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 2. Lei dos Senos e Lei dos Cossenos

<style scoped>
.theory { font-size: 20px; }
.example-box { font-size: 17px; padding: 16px 12px; margin-top: 5px; }
</style>

<div class="content-wrapper">
<div class="theory">

Para triângulos que não possuem ângulo reto (triângulos quaisquer), utilizamos as Leis dos Senos e Cossenos.

- **Lei dos Senos:** Usada quando conhecemos "dois ângulos e um lado" ou para encontrar o raio $R$ da circunferência circunscrita.
  $$ \frac{a}{\sin(A)} = \frac{b}{\sin(B)} = \frac{c}{\sin(C)} = 2R $$

- **Lei dos Cossenos:** O "Pitágoras tunado". Usada quando conhecemos "dois lados e o ângulo entre eles".
  $$ a^2 = b^2 + c^2 - 2bc \cdot \cos(\hat{A}) $$

<div class="example-box">

**Exemplo 02:** Em um triângulo, dois lados medem $5$ cm e $8$ cm e formam entre si um ângulo de $60^\circ$. Qual é a medida do terceiro lado?

</div>

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 3. Radianos e o Ciclo Trigonométrico

<style scoped>
.theory { font-size: 19px; }
.example-box { font-size: 17px; padding: 16px 12px; margin-top: 5px; }
</style>

<div class="content-wrapper">
<div class="theory">

O **Radianos** é uma medida de arco baseada no raio da circunferência. A relação fundamental de conversão é: **$180^\circ = \pi \text{ rad}$**.

O **Ciclo Trigonométrico** é uma circunferência de raio $1$ com centro na origem do plano cartesiano.
- O eixo horizontal ($x$) é o eixo dos **cossenos** ("com sono = deitado").
- O eixo vertical ($y$) é o eixo dos **senos** ("sem sono = em pé").
- O ponto da circunferência define um ângulo $\theta$ a partir do semi-eixo $x$ positivo, no sentido anti-horário.

Isso nos permite achar senos e cossenos de ângulos em qualquer quadrante! Lembre-se da regra de sinais:
- **Seno:** Positivo acima do eixo $x$ (1º e 2º quadrantes).
- **Cosseno:** Positivo à direita do eixo $y$ (1º e 4º quadrantes).

<div class="example-box">

**Exemplo 03:** Converta $120^\circ$ para radianos e determine o valor de $\sin(120^\circ)$ e $\cos(120^\circ)$.

</div>

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 4. Relações Fundamentais da Trigonometria

<style scoped>
.theory { font-size: 19px; }
.theory ul { font-size: 18px; margin-bottom: 16px; }
.example-box { font-size: 17px; padding: 16px 12px; margin-top: 5px; }
</style>

<div class="content-wrapper">
<div class="theory">

Ao aplicar o Teorema de Pitágoras no triângulo retângulo formado dentro do ciclo trigonométrico de raio 1, obtemos a **Relação Fundamental da Trigonometria**:
$$ \sin^2(x) + \cos^2(x) = 1 $$

Dela e das definições, derivam outras identidades que frequentemente ajudam a simplificar expressões ou gráficos no vestibular:
- $\tan(x) = \frac{\sin(x)}{\cos(x)}$
- $\sec(x) = \frac{1}{\cos(x)}$ (Secante)
- $\csc(x) = \frac{1}{\sin(x)}$ (Cossecante)
- $\cot(x) = \frac{\cos(x)}{\sin(x)}$ (Cotangente)

<div class="example-box">

**Exemplo 04:** Se $\sin(x) = \frac{3}{5}$ e $x$ está no segundo quadrante ($90^\circ < x < 180^\circ$), qual é o valor de $\cos(x)$ e de $\tan(x)$?

</div>

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 5. Funções Trigonométricas (Gráficos, Período e Imagem)

<style scoped>
.theory { font-size: 19px; }
.example-box { font-size: 17px; padding: 16px 12px; margin-top: 5px; }
</style>

<div class="content-wrapper">
<div class="theory">

As funções $f(x) = \sin(x)$ e $f(x) = \cos(x)$ formam ondas periódicas perfeitamente delimitadas.
- **Imagem:** A onda oscila entre um máximo e mínimo. O padrão é $[-1, 1]$.
- **Período:** É o tamanho que a onda leva para completar um ciclo. O padrão é $2\pi$.

Uma função geral tem o formato: $f(x) = a + b \cdot \sin(cx + d)$.
- $a$: desloca o gráfico para cima ou baixo.
- $b$: altera a amplitude da onda (estica verticalmente).
- $c$: altera a velocidade (espreme horizontalmente). O novo período é $P = \frac{2\pi}{|c|}$.

<div class="example-box">

**Exemplo 05:** Dada a função $f(x) = 3 + 2\sin(4x)$, determine a Imagem e o Período do seu gráfico.

</div>

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# 6. Seno e Cosseno da Soma e Diferença

<style scoped>
.theory { font-size: 19px; }
.example-box { font-size: 17px; padding: 16px 12px; margin-top: 5px; }
</style>

<div class="content-wrapper">
<div class="theory">

Às vezes, precisamos calcular senos e cossenos de ângulos que não estão na tabela, mas que são somas ou subtrações de ângulos notáveis (ex: $75^\circ = 45^\circ + 30^\circ$).

- **Seno da Soma/Diferença:** *(Minha terra tem palmeiras, onde canta o sabiá...)*
  $$ \sin(a \pm b) = \sin(a)\cos(b) \pm \sin(b)\cos(a) $$

- **Cosseno da Soma/Diferença:** *(Coça A, Coça B, troca o sinal)*
  $$ \cos(a \pm b) = \cos(a)\cos(b) \mp \sin(a)\sin(b) $$

<div class="example-box">

**Exemplo 06:** Calcule o valor exato de $\cos(15^\circ)$, lembrando que $15^\circ = 45^\circ - 30^\circ$.

</div>

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# Questão 01 - UFRGS 2025

<div class="content-wrapper">
<div class="theory" style="font-size: 18px;">

Na figura do material (ou considere as medidas a seguir), ABCD é um paralelogramo tal que suas diagonais medem $\overline{AC} = 16$ e $\overline{BD} = 10$ e formam um ângulo de $60^\circ$.

As medidas dos lados do paralelogramo ABCD são:

(A) 6 e 12.
(B) 7 e 15.
(C) 6 e $2\sqrt{17}$.
(D) 7 e $\sqrt{129}$.
(E) 9 e $\sqrt{129}$.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# Questão 02 - UFRGS 2024

<div class="content-wrapper">
<div class="theory" style="font-size: 18px;">

Na figura da lista, $ABC$ é um triângulo equilátero de lado 6. O ponto $D$ é ponto médio do lado $\overline{AC}$, e a medida de $\overline{EB}$ é 2.

O perímetro do triângulo $AED$ é:

(A) $5 + \sqrt{5}$.
(B) $7 + \sqrt{5}$.
(C) $10 + \sqrt{5}$.
(D) $7 + \sqrt{13}$.
(E) $10 + \sqrt{13}$.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# Questão 03 - UFRGS 2022

<div class="content-wrapper">
<div class="theory" style="font-size: 18px;">

No retângulo ABCD, representado na figura da lista, os três ângulos destacados com vértice em C são iguais (dividindo o ângulo reto em três partes). 

A área do triângulo sombreado AEC, em relação à área total do retângulo, corresponde a:

(A) $\frac{1}{2}$.
(B) $\frac{1}{3}$.
(C) $\frac{2}{5}$.
(D) $\frac{3}{5}$.
(E) $\frac{2}{3}$.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# Questão 04 - UFRGS 2022

<div class="content-wrapper">
<div class="theory" style="font-size: 18px;">

Na figura da lista, o triângulo ABC é equilátero de lado 4. O ponto D pertence ao lado AB, o ponto E pertence ao lado BC, o ponto F pertence ao lado AC, e os segmentos AD, BE e CF têm medida $x$.

A função $A(x)$ que expressa a área do triângulo equilátero DEF, para $0 \le x \le 4$, é:

(A) $A(x) = \frac{\sqrt{3}}{2}(3x^2 - 6x + 8)$.
(B) $A(x) = \frac{\sqrt{3}}{2}(3x^2 + 12x + 16)$.
(C) $A(x) = -\frac{\sqrt{3}}{4}(3x^2 + 12x - 16)$.
(D) $A(x) = \frac{\sqrt{3}}{4}(3x^2 + 12x + 16)$.
(E) $A(x) = \frac{\sqrt{3}}{4}(3x^2 - 12x + 16)$.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# Questão 08 - UFRGS 2018

<div class="content-wrapper">
<div class="theory" style="font-size: 18px;">

Na circunferência de raio $1$, representada na lista, os pontos $M$ e $N$ são tais que o arco de extremidades $A$ e $M$ mede $\frac{\pi}{2}\,rad$ e o arco de extremidades $A$ e $N$ mede $-\frac{\pi}{3}\,rad$.

A distância entre os pontos $M$ e $N$ é:

(A) $\sqrt{2 - \sqrt{3}}$.
(B) $2 - \sqrt{3}$.
(C) $\sqrt{2 + \sqrt{3}}$.
(D) $1$.
(E) $2 + \sqrt{3}$.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# Questão 10 - UFRGS 2017

<div class="content-wrapper">
<div class="theory" style="font-size: 18px;">

Se $a$ e $b$ são ângulos agudos e complementares, o valor da expressão $\sin^2(a+b) - \cos^2(a+b)$ é:

(A) 0.
(B) 1.
(C) 2.
(D) $\sqrt{2}$.
(E) $\sqrt{3}$.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# Questão 16 - UFRGS 2015

<div class="content-wrapper">
<div class="theory" style="font-size: 18px;">

Considere as funções $f$ e $g$ definidas por $f(x) = \sin x$ e $g(x) = \cos x$.

O número de raízes da equação $f(x) = g(x)$ no intervalo $[-2\pi, 2\pi]$ é:

(A) 3.
(B) 4.
(C) 5.
(D) 6.
(E) 7.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# Questão 17 - UFRGS 2014

<div class="content-wrapper">
<div class="theory" style="font-size: 18px;">

O gráfico da função $f$, definida por $f(x) = \cos x$, e o gráfico da função $g$, quando representados no mesmo sistema de coordenadas, possuem somente dois pontos em comum.

Assim, das alternativas abaixo, a que pode representar a função $g$ é:

(A) $g(x) = (\sin x)^2 + (\cos x)^2$.
(B) $g(x) = x^2$.
(C) $g(x) = 2^x$.
(D) $g(x) = \log x$.
(E) $g(x) = \sin x$.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>

---

# Questão 26 - UFRGS 2010

<div class="content-wrapper">
<div class="theory" style="font-size: 18px;">

Dentre as opções a seguir (presentes graficamente na lista de exercícios), a que pode representar o gráfico da função definida por $f(x) = (\sin x + \cos x)^2 + (\sin x - \cos x)^2$ é a alternativa:

*(Nota: Para resolver no quadro, expanda a função algébricamente para descobrir a forma de onda resultante e a correlacione com as opções).*

(A) Gráfico de onda periódica simétrica no eixo Y (cosseno modulado).
(B) Reta horizontal acima do eixo x.
(C) Reta diagonal passando pela origem.
(D) Curva senóide partindo da origem.
(E) Reta vertical deslocada do eixo y.

</div>
<div class="resolution">
<h3>Resolução:</h3>
</div>
</div>
