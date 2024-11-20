$(S, *)$ è detta *struttura algebrica* 
- Se $*$ è associativa, $(S, *)$ è chiamato semigruppo
- Se un semigruppo $(S, *)$ ammette un elemento neutro è chiamato monoide
- Un semigruppo / monoide $(S,*)$ si dice **commutativo** o **abeliano** se l'operazione è commutativa
- Avendo un monoide $(S, *): a\in S$ diciamo che questo elemento è invertibile se $\exists b\in S: b*a=e=a*b$ in tal caso $b$ si dice l'inverso di $a$
- Un monoide di cui ogni elemento è invertibile è chiamato gruppo 

Per esempio sono gruppi:
$(ℤ,+,0),(ℚ\backslash\{0\},\cdot,1)$
$(ℚ, +, 0), (ℝ\backslash\{0\},\cdot, 1)$
$(ℝ, +, 0)$

È un gruppo anche:
$(\frac{ℤ}{2ℤ},+, \overline{0})$

perché
- L'invertibile di $\overline{0}$ è $\overline{0}$ in quanto = $\overline{0}+\overline{0}=\overline{0}$
- E l'invertibile di $\overline{1}$ è $\overline{1}$ in quanto $\overline{1}+\overline{1}=\overline{2}$ che visto che stiamo parlando di $n\ mod\ 2$ scrivere $\overline{2}$ è la stessa cosa di scrivere $\overline{0}$

Questo si può fare anche con la moltiplicazione:
$(\frac{ℤ}{3ℤ},\cdotp,\overline{1})$

$\overline{0}\cdot\overline{0}=\overline{0}$
$\overline{0}\cdot\overline{1}=\overline{0}$
$\overline{1}\cdot\overline{0}=\overline{0}$
$\overline{1}\cdot\overline{1}=\overline{1}$
$\overline{1}\cdot\overline{2}= \overline{2}$
$\overline{2}\cdot\overline{1}= \overline{2}$
$\overline{2}\cdot\overline{2}= \overline{0}$
$\overline{1}\cdot\overline{2}= \overline{2}$
$\overline{2}\cdot\overline{2}= \overline{4} = \overline{1}$

Tuttavia $(\frac{ℤ}{4ℤ}\backslash\{0\}, \cdotp, \overline{1})$ non è un gruppo in quanto:
- L'inverso di $\overline{2}$ sarebbe $\overline{2}$ ma non è fattibile in quanto $\overline{4}=\overline{0}$ che nell'insieme che in questo caso è $\frac{ℤ}{4ℤ}\backslash\{0\}=\{\overline{1},\overline{2}, \overline{3}\}$ non esiste

Questo implica quindi che negli insiemi con modulo e come operazione la moltiplicazione è un *gruppo solo se il numero del modulo è un numero primo* ad esempio:
$(\frac{ℤ}{Pℤ},\cdotp,\overline{1}) =>$ in cui $P$ è un numero primo


|            | Addizione | Moltiplicazione | Generale |
| ---------- | --------- | --------------- | -------- |
| Operazione | $+$       | $\cdot$         | $*$      |
| Inverso    | $-a$      | $a^{-1}$        | $a^{-1}$ |
| Neutro     | $0$       | $1$             | $e$      |
