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
## AULA 10 - Análise Combinatória


*(Aguardando o início da transmissão)*
</div>

---

# 1. Fatorial de um Número Natural

<div class="content-wrapper">
<div class="theory">

O fatorial é uma operação matemática fundamental na Análise Combinatória. Representado pelo símbolo de exclamação (!), o fatorial de um número natural $n$ é o produto de todos os inteiros positivos menores ou iguais a $n$.

$$\Large n! = n \cdot (n-1) \cdot (n-2) \cdot \dots \cdot 1$$

*Casos Especiais:* Por convenção matemática e para garantir a validade das fórmulas combinatórias, definimos: $0! = 1$ e $1! = 1$.

<div class="example-box">

**Exemplo 01:** Calcule o valor numérico de $5!$ e de $6!$.
</div>

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 2. Operações e Simplificações com Fatoriais

<div class="content-wrapper">
<div class="theory">

Na Análise Combinatória, frequentemente nos deparamos com frações envolvendo fatoriais. A técnica essencial consiste em **expandir o fatorial maior até que ele alcance o fatorial menor** presente na expressão.

Isso permite o cancelamento algébrico dos termos repetidos, evitando a manipulação de números astronomicamente grandes durante os cálculos.

$$\Large \frac{n!}{(n-k)!} = \frac{n \cdot (n-1) \dots (n-k)!}{(n-k)!}$$

<div class="example-box">

**Exemplo 02:** Simplifique e calcule o valor da expressão: $\frac{10!}{7! \cdot 3!}$
</div>

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 3. Princípio Fundamental da Contagem (PFC)

<div class="content-wrapper">
<div class="theory">

Também conhecido como Princípio Multiplicativo, é o axioma base de toda a contagem.

Se uma decisão $d_1$ pode ser tomada de $n_1$ modos e, após isso, uma decisão $d_2$ puder ser tomada de $n_2$ modos, o número total de modos de tomar as sucessivas decisões é dado pelo produto cartesiano das escolhas:
$$\text{Total} = n_1 \cdot n_2 \cdot \dots \cdot n_k$$

<div class="example-box">

**Exemplo 03:** Uma senha bancária é formada por 2 letras distintas (alfabeto de 26 letras) seguidas por 3 algarismos (de 0 a 9) não podendo haver repetição. Quantas senhas são possíveis?
</div>

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 4. Permutação Simples ($k$ a $k$)

<div class="content-wrapper">
<div class="theory">

Corresponde ao reordenamento total de um conjunto finito. Usamos a permutação quando agrupamos **todos** os elementos do conjunto e apenas a ordem se altera.

$$\Large P_k = k! = k \cdot (k-1) \cdot \dots \cdot 1$$

* $k$: número total de elementos distintos a serem ordenados.
* Lembrete: $0! = 1$.

<div class="example-box">

**Exemplo 04:** De quantas formas distintas podemos dispor 5 livros diferentes em uma prateleira (anagrama da disposição)?
</div>

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 5. Arranjo Simples ($n$ a $k$)

<div class="content-wrapper">
<div class="theory">

É a seleção e ordenação de um subconjunto. Corresponde a escolher $k$ elementos a partir de um conjunto maior de $n$ elementos distintos, onde a **ordem da escolha importa** .

$$\Large A_{n,k} = \frac{n!}{(n-k)!}$$

*Atenção à nuance:* Se a ordem não importasse (ex: montar uma comissão), seria uma Combinação. No arranjo, os papéis/posições são distintos (ex: 1º, 2º e 3º lugar).

<div class="example-box">

**Exemplo 05:** Em uma corrida com 8 atletas, de quantas formas diferentes o pódio (ouro, prata e bronze) pode ser formado?
</div>

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 6. Permutação com Repetição

<div class="content-wrapper">
<div class="theory">

Quando o conjunto a ser ordenado possui elementos **indistinguíveis** (idênticos), as trocas entre esses elementos não geram novas configurações. Devemos "descontar" (através da divisão) as permutações internas desses itens repetidos.

$$\Large P_n^{n_1, n_2, \dots} = \frac{n!}{n_1! \cdot n_2! \dots}$$

* $n$: total de elementos.
* $n_1, n_2$: quantidades de elementos repetidos de cada tipo.

<div class="example-box">

**Exemplo 06:** Quantos anagramas possui a palavra **MATEMATICA**?
</div>

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 7. Permutação Circular

<div class="content-wrapper">
<div class="theory">

A permutação circular ocorre quando organizamos elementos distintos ao redor de um círculo (como em uma mesa redonda ou roda ciranda). Como não há um "início" ou "fim" fixo, rotações da mesma formação são consideradas idênticas.

Para evitar a contagem de disposições repetidas por rotação, fixamos um elemento como referencial e permutamos os demais:
$$\Large P_c(n) = (n-1)!$$

<div class="example-box">

**Exemplo 07:** De quantas formas distintas 6 diretores de uma empresa podem se sentar ao redor de uma mesa circular de reuniões?
</div>

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 8. Combinação Simples

<div class="content-wrapper">
<div class="theory">

A combinação simples trata da seleção de subconjuntos onde a **ordem dos elementos não importa** (diferente do Arranjo). A escolha do subconjunto formado por Ana e Bruno é idêntica à escolha de Bruno e Ana.

Para calcular, tomamos o total de arranjos e dividimos pela permutação dos elementos escolhidos (para eliminar as redundâncias de ordenação):
$$\Large C_{n,k} = \binom{n}{k} = \frac{n!}{k!(n-k)!}$$

<div class="example-box">

**Exemplo 08:** Em uma sala de aula com 10 estudantes, de quantas maneiras o professor pode selecionar uma comissão de 4 alunos para um projeto?
</div>

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 9. UFRGS 2024

<div class="content-wrapper">
<div class="theory" style="font-size: 22px;">

Qual a quantidade de números possível de se formar com quatro algarismos distintos, de 1 a 9, que são múltiplos de 5?

<br><br>

(A) $84$ <br>
(B) $112$ <br>
(C) $168$ <br>
(D) $210$ <br>
(E) $336$

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 10. UFRGS 2022

<div class="content-wrapper">
<div class="theory" style="font-size: 19px;">

Uma biblioteca está elaborando etiquetas de identificação para os livros do acervo de tal forma que, em cada etiqueta, são usadas quatro letras distintas, de um alfabeto de 26 letras, e quatro algarismos também distintos, de 0 a 9. Assinale a alternativa que apresenta o número total de etiquetas distintas produzidas.

<div style="text-align: center; margin: 15px 0;">
  <div style="border: 4px solid #E0E0E0; display: inline-block; padding: 10px 20px; font-size: 28px; font-weight: bold; letter-spacing: 5px; color: #8BE9FD;">
    E M A T 9 5 0 1
  </div>
</div>

(A) $26 + 10$ <br>
(B) $26 \cdot 10$ <br>
(C) $A_{26,4} \cdot A_{10,4}$ <br>
(D) $A_{26,4} + A_{10,4}$ <br>
(E) $10A_{26,4} + 26A_{10,4}$

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 11. UFRGS 2019

<div class="content-wrapper">
<div class="theory" style="font-size: 16px;">

Um aplicativo de transporte disponibiliza a visualização de um mapa com ruas horizontais e verticais que permitem realizar deslocamentos partindo de A e chegando a B, conforme a figura abaixo. O número de menores caminhos possíveis que partem de A e chegam a B, passando por C, é:

<div style="text-align: center; margin-top: 10px; margin-bottom: 5px;">
<svg viewBox="-10 -10 230 170" width="300">
  <line x1="0" y1="0" x2="210" y2="0" stroke="#E0E0E0" stroke-width="1.5"/>
  <line x1="0" y1="30" x2="210" y2="30" stroke="#E0E0E0" stroke-width="1.5"/>
  <line x1="0" y1="60" x2="210" y2="60" stroke="#E0E0E0" stroke-width="1.5"/>
  <line x1="0" y1="90" x2="210" y2="90" stroke="#E0E0E0" stroke-width="1.5"/>
  <line x1="0" y1="120" x2="210" y2="120" stroke="#E0E0E0" stroke-width="1.5"/>
  <line x1="0" y1="150" x2="210" y2="150" stroke="#E0E0E0" stroke-width="1.5"/>
  <line x1="0" y1="0" x2="0" y2="150" stroke="#E0E0E0" stroke-width="1.5"/>
  <line x1="30" y1="0" x2="30" y2="150" stroke="#E0E0E0" stroke-width="1.5"/>
  <line x1="60" y1="0" x2="60" y2="150" stroke="#E0E0E0" stroke-width="1.5"/>
  <line x1="90" y1="0" x2="90" y2="150" stroke="#E0E0E0" stroke-width="1.5"/>
  <line x1="120" y1="0" x2="120" y2="150" stroke="#E0E0E0" stroke-width="1.5"/>
  <line x1="150" y1="0" x2="150" y2="150" stroke="#E0E0E0" stroke-width="1.5"/>
  <line x1="180" y1="0" x2="180" y2="150" stroke="#E0E0E0" stroke-width="1.5"/>
  <line x1="210" y1="0" x2="210" y2="150" stroke="#E0E0E0" stroke-width="1.5"/>
  <circle cx="0" cy="150" r="4" fill="#8BE9FD" />
  <text x="-12" y="154" fill="#8BE9FD" font-size="12">A</text>
  <circle cx="210" cy="0" r="4" fill="#8BE9FD" />
  <text x="216" y="4" fill="#8BE9FD" font-size="12">B</text>
  <circle cx="90" cy="60" r="4" fill="#FFB86C" />
  <text x="96" y="56" fill="#FFB86C" font-size="12">C</text>
</svg>
</div>

(A) $28$ &nbsp;&nbsp;&nbsp;&nbsp; (B) $35$ &nbsp;&nbsp;&nbsp;&nbsp; (C) $100$ &nbsp;&nbsp;&nbsp;&nbsp; (D) $300$ &nbsp;&nbsp;&nbsp;&nbsp; (E) $792$

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 12. UFRGS 2017

<div class="content-wrapper">
<div class="theory" style="font-size: 22px;">

Tomando os algarismos ímpares para formar números com quatro algarismos distintos, a quantidade de números divisíveis por 5 que se pode obter é:

<br><br>

(A) $12$ <br>
(B) $14$ <br>
(C) $22$ <br>
(D) $24$ <br>
(E) $26$

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 13. ENEM 2019

<div class="content-wrapper">
<div class="theory" style="font-size: 20px;">

Uma pessoa comprou um aparelho sem fio para transmitir músicas a partir do seu computador para o rádio de seu quarto. Esse aparelho possui quatro chaves seletoras e cada uma pode estar na posição 0 ou 1. Cada escolha das posições dessas chaves corresponde a uma frequência diferente de transmissão.

A quantidade de frequências diferentes que esse aparelho pode transmitir é determinada por:

<br><br>

(A) $6$ <br>
(B) $8$ <br>
(C) $12$ <br>
(D) $16$ <br>
(E) $24$

</div>
<div class="resolution">Resolução:</div>
</div>

---

# 14. ENEM 2021

<div class="content-wrapper">
<div class="theory" style="font-size: 19px;">

Uma pessoa produzirá uma fantasia utilizando como materiais: 2 tipos de tecidos diferentes e 5 tipos distintos de pedras ornamentais. Essa pessoa tem à sua disposição 6 tecidos diferentes e 15 pedras ornamentais distintas.

A quantidade de fantasias com materiais diferentes que podem ser produzidas é representada pela expressão:

<br><br>

(A) $\frac{6!}{4!2!} \cdot \frac{15!}{10!5!}$ <br>
(B) $\frac{6!}{4!2!} + \frac{15!}{10!5!}$ <br>
(C) $\frac{6!}{2!} + \frac{15!}{5!}$ <br>
(D) $\frac{6!}{2!} \cdot \frac{15!}{5!}$ <br>
(E) $\frac{21!}{7!14!}$

</div>
<div class="resolution">Resolução:</div>
</div>

---