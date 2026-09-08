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
## Encontro 01: Conjuntos e Estrutura dos Números Reais

<br><br>
*(Aguardando o início da transmissão)*
</div>

---

# 1. Noção Intuitiva de Conjuntos

Chamamos de **conjunto** a uma coleção de objetos. Os objetos que formam um conjunto são os seus **elementos**.

* Representação: Letras maiúsculas ($A, B, C...$)
* Pertencimento: Se $a$ é elemento de $A$, escrevemos $a \in A$.

Exemplo:
<div class="sem-bolinha">

* $A = \{3, 6, 7\}$
* $a \in A$
* $1 \notin A$
* $B = \{x \mid x \text{ é estado do Brasil}\}$

</div>

---

# 2. Subconjuntos e Conjunto Vazio

Dizemos que $A$ é um subconjunto de $B$ ($A \subseteq B$) se todo elemento de $A$ também pertence a $B$.

* **Conjunto Vazio ($\emptyset$):** É o conjunto que não possui elementos.
* **Nota importante:** O vazio está contido em qualquer conjunto ($\emptyset \subseteq A$).

<br>

Exemplo: Seja $A$ o conjunto formado pelo números que são pares e ímpares ao mesmo tempo. Represente este conjunto.
<br><br><br>

---

# 3. Conjuntos Numéricos

A evolução da contagem e a estrutura da reta real:

* **Naturais ($\mathbb{N}$):** $\{1, 2, 3, ...\}$
* **Inteiros ($\mathbb{Z}$):** $\{..., -2, -1, 0, 1, 2, ...\}$
* **Racionais ($\mathbb{Q}$):** $\{x | x = \frac{a}{b}, a, b \in \mathbb{Z}, b \neq 0\}$
* **Irracionais ($\mathbb{I}$):** Decimais infinitos e não periódicos ($\pi, \sqrt{2}$, entre outros).
* **Reais ($\mathbb{R}$):** $\mathbb{Q} \cup \mathbb{I}$

---

# 4. Exercício de Fixação (UFRGS - 2025)

Considere as seguintes afirmações sobre números e suas operações:

I. A soma de dois números naturais consecutivos é sempre um número ímpar.
II. A soma de dois números irracionais é sempre um número irracional.
III. Se $a > 1$, então, para qualquer valor inteiro de $n$, $0 < \frac{1}{a^n} < 1$.

Quais estão corretas?

* (A) Apenas I.
* (B) Apenas III.
* (C) Apenas I e II.
* (D) Apenas II e III.
* (E) I, II e III.

---

# 5. Diagramas de Venn e Operações

A visualização de conjuntos através de diagramas ajuda a resolver problemas de contagem complexos.
* **Interseção ($A \cap B$):** Elementos em comum.
* **União ($A \cup B$):** Todos os elementos de ambos.

---

# 6. Desafio das Marcas (Diagramas de 3 Conjuntos)

Em uma pesquisa de mercado sobre o uso de sabão em pó das marcas A, B e C, obteve-se:
* Marca A: 105 pessoas;
* Marca B: 200 pessoas;
* Marca C: 160 pessoas;
* A e B: 25 pessoas;
* B e C: 40 pessoas;
* A e C: 25 pessoas;
* A, B e C: 5 pessoas;
* Nenhuma das 3 marcas: 120 pessoas.

Quantas pessoas foram consultadas?

---

# 7. Dízimas Periódicas e Fração Geratriz

São números decimais infinitos que apresentam um padrão de repetição (período).

Exemplos para transformar em fração:
<div class="sem-bolinha">

* a) $0,4444...$
  <br>
* b) $0,131313...$
  <br>
* c) $1,222...$

</div>

---

# 8. Números Decimais

NÃO confundir dízimas periódicas e suas regras com números decimais.

Exemplo:
<div class="sem-bolinha">

* a) $0,4$
  <br>
* b) $0,44$
  <br>
* c) $0,13$
  <br>
* d) $1,22$

</div>

---

# 9. Módulo ou Valor Absoluto

Chamamos de módulo ou valor absoluto de um número $|x|$ a **distância** deste número até a origem (zero) na reta real.

Exemplos:
<div class="sem-bolinha">

* $|5| =$
* $|-5| =$
* $|x| < 3 \implies$

</div>

---

# 10. Intervalos Reais

Representações na reta numérica para subconjuntos de $\mathbb{R}$:

* Fechado $[a, b]$: $a \le x \le b$ (Bolinha cheia)
* Aberto $(a, b)$: $a < x < b$ (Bolinha vazia)

Desenho da reta:
<br><br><br>

---

# 11. Intervalos Reais

Exemplo:
a) $x \leq 3$
<br>
b) $x \geq 4$
<br>
c) $-2 < x < 2$
<br>
d) $-1 \leq x < 3$

---

<div class="center">

# Fim do Encontro 01
## Próxima Aula: Potenciação, Radiciação e Notação Científica

<br>

</div>