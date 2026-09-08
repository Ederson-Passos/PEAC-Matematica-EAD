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
## Encontro 03: Razão, Proporção e Matemática Financeira

<br><br>
*(Aguardando o início da transmissão)*
</div>

---

# 1. Razão e Proporção

## O que é uma Razão?
A razão entre dois números $a$ e $b$ (com $b \neq 0$) é simplesmente o quociente entre eles. Usamos a razão para comparar grandezas.

$$\text{Razão} = \frac{a}{b} \quad \text{(lê-se: } a \text{ está para } b)$$

Razões especiais no dia a dia:
* **Velocidade Média:** $V_m = \frac{\Delta S}{\Delta t}$
* **Densidade:** $d = \frac{m}{v}$
* **Escala:** $\frac{\text{Medida no desenho } (d)}{\text{Tamanho real } (D)}$

---

# 1.1 Exemplo: Escala

**Dica de Ouro:** Escala é sempre numa relação linear (comprimento). Se a questão falar de Área, a escala deve ser elevada ao quadrado!

<br>

Num mapa de escala $1:500.000$, a distância entre duas cidades é de $4$ cm. Qual a distância real entre elas?

<div class="sem-bolinha">

* </div>

---

# 1.2 Proporção e a Propriedade Fundamental

Uma proporção é a igualdade entre duas razões:
$$\frac{a}{b} = \frac{c}{d}$$

**Propriedade Fundamental:** O produto dos meios é igual ao produto dos extremos.
$$a \cdot d = b \cdot c$$

Exemplo: A razão entre o número de alunos e o número de professores numa escola é de $20$ para $1$. Se a escola possui $400$ alunos, quantos professores trabalham na instituição?

<div class="sem-bolinha">

* </div>

---

# 2. Grandezas Proporcionais

Duas grandezas podem relacionar-se de duas formas:

* **Diretamente Proporcionais (DP):** Quando uma aumenta, a outra também aumenta na mesma proporção. A razão (divisão) entre elas é constante.
    * *Ex:* Quantidade de pães comprados e o valor total a pagar.

* **Inversamente Proporcionais (IP):** Quando uma aumenta, a outra diminui na mesma proporção. O produto (multiplicação) entre elas é constante.
    * *Ex:* Velocidade de um carro e o tempo de viagem.

---

# 3. Regra de Três Simples

É o método prático para resolver problemas de proporção envolvendo apenas 2 grandezas.

**Exemplo 1 (Grandezas DP):** Se um carro consome 12 litros de gasolina para percorrer 180 km, quantos litros consumirá para percorrer 300 km?

<div class="sem-bolinha">

* </div>

---

# 3. Regra de Três Simples

**Exemplo 2 (Grandezas IP):** Um veículo com velocidade de $60$ km/h faz um percurso em $4$ h. Se a velocidade fosse de $80$ km/h, quanto tempo levaria para completar o mesmo trajeto?

<div class="sem-bolinha">

* </div>

---

# 3.1 Regra de Três Composta

Envolve 3 ou mais grandezas. A análise é feita comparando as colunas, sempre isoladamente, com a coluna da incógnita ($x$).

**Exemplo:** Se $4$ pedreiros constroem um muro em $15$ dias trabalhando $6$ horas por dia, em quantos dias $6$ pedreiros construirão o mesmo muro trabalhando $8$ horas por dia?

<div class="sem-bolinha">

* </div>

---

# 4. Porcentagem

A porcentagem é uma razão cujo denominador é 100.
$$20\% = \frac{20}{100} = 0,20$$

**Fator de Multiplicação (O segredo para ser rápido):**
* Se um produto sofre um AUMENTO de $i\%$, o fator é $(1 + i)$.
* Se um produto sofre um DESCONTO de $i\%$, o fator é $(1 - i)$.

---

# 4. Porcentagem (Fatores)

**Exemplo 1 (Aumento):** Uma mercadoria custa R\$ $80,00$ e sofre um aumento de $15\%$. Qual o novo preço?
<div class="sem-bolinha">

* </div>

<br><br>

**Exemplo 2 (Desconto):** Um sapato de R\$ $120,00$ está com $20\%$ de desconto. Qual o valor final?
<div class="sem-bolinha">

* </div>

---

# 5. Matemática Financeira

O montante final ($M$) é sempre o Capital ($C$) mais os Juros ($J$).
$$M = C + J$$

## 5.1 Juros Simples
Neste regime, o juro rende de forma linear sobre o capital inicial (Progressão Aritmética).

$$J = C \cdot i \cdot t$$

*(A taxa $i$ e o tempo $t$ devem estar sempre na mesma unidade)*

---

# 5.1 Juros Simples

**Exemplo:** Qual o juro gerado por um capital de R\$ $5.000,00$ aplicado a uma taxa de $2\%$ ao mês durante um ano?

<div class="sem-bolinha">

* </div>

---

# 5.2 Juros Compostos

Aqui, o juro rende sobre o montante do mês anterior (Progressão Geométrica, crescimento exponencial). É o sistema usado por bancos.

$$M = C \cdot (1 + i)^t$$

**Exemplo:** Um capital de R\$ $1.000,00$ foi aplicado a juros compostos de $10\%$ ao mês. Qual o montante após 2 meses?

<div class="sem-bolinha">

* </div>

---

# 5.3 A Armadilha das Taxas (ENEM)

**Atenção:** Nunca use Regra de Três para tempo e taxa em Juros Compostos!

* **Em Juros Simples:** 10% ao mês $= 120\%$ ao ano. (São proporcionais).
* **Em Juros Compostos:** 10% ao mês $\neq 120\%$ ao ano. A taxa real anual será muito MAIOR devido aos "juros sobre juros".

Para converter, igualamos os **Fatores de Multiplicação**:
$$1 + i_{\text{anual}} = (1 + i_{\text{mensal}})^{12}$$

---

# 5.3 Taxas Equivalentes (A Prova)

**Exemplo (A Armadilha do Cartão de Crédito):** Um banco cobra juros compostos de $10\%$ ao mês no atraso da fatura. Qual é a taxa percentual real cobrada ao final de **2 meses**?

<div class="sem-bolinha">

* </div>

---

<div class="center">

# Fim do Encontro 03
## Próxima Aula: Geometria Plana I: Polígonos e Triângulos

<br>

</div>