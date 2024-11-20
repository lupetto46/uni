### Definizioni
Ci sono varie definizioni riguardanti le funzioni su insiemi con operazioni
Avendo due *strutture algebriche* $(A,*_{_A}),\quad (B, *_{_B})$
E una funzione $f:A\longrightarrow B$
Se $f(a*_{_A}a')=f(a)*_{_B }f(a')$ allora si chiama omomorfismo di strutture algebriche*

Un omomorfismo $f:(A, *_{_A})\longrightarrow (B, *_{_B})$ è detto:
- *Monomorfismo* se $f$ è iniettiva
- *Epimorfismo* se $f$ è suriettivo
- Isomorfismo se $f$ è biiettivo

Se abbiamo una mappa tra due anelli:
$f:(A, +_{_A}, \cdot_{_A})\longrightarrow(B, +_{_B}, \cdot_{_B})$
Questa si chiama omomorfismo di anelli* se
$f(a+_{_A}a')=f(a) +_{_B}f(a'), \quad f(a \cdot_{_A} a')= f(a)\cdot_{_B}f(a')$

> [!info] Esempio
> 
> $\begin{align*}f:(ℤ, +)&\longrightarrow (ℤ,+)\\ x&\longmapsto 2x\end{align*}\quad$ è un omomorfismo di gruppi* quanto:
> $f(x+y)=2(x+y)=2x+2y=f(x)+f(y)$
>  Quindi scrivere $f(x+y)$ è la stessa cosa di scrivere $f(x) + f(y)$
>  
>  Mentre invece:
>  $\begin{align*}f:(ℤ, +, \cdotp)&\longrightarrow (ℤ,+, \cdotp)\\ x&\longmapsto 2x\end{align*}\quad$ non è un omomorfismo di anelli perché:
>  Anche se come prima: $f(x+y)=2(x+y)=2x+2y=f(x)+f(y)$
>  
>  $f(x\cdot y) = 2\cdot (x\cdot y)= \overbrace{2xy}^{\text{proprietà associativa}}\neq 4xy=f(x)\cdot f(y)$
>  La moltiplicazione da un risultato diverso tra $f(x\cdot y)\neq f(x)\cdot f(y)$ quindi ***non è*** *un omomorfismo di anelli*