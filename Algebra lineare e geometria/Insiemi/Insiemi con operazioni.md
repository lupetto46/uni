$S\neq\emptyset$ un operazione su $S$ è una funzione:
$*:S * S\longrightarrow S$
$(a,b)\longmapsto a*b$

La stella ($*$) indica un'*operazione generica*
> [!example] Esempio
> $+:ℕ*ℕ\longrightarrow ℕ$
> $(a,b)\longmapsto a+b$

### Proprietà delle operazioni
- Un operazione ***può*** essere associativa:
	- $\forall a,b,c\in S\qquad (a*b)*c=(b*c)*a=(c*a)*b$
- Un operazione ***può*** essere commutativa:
	- $\forall a,b,c\in S\qquad a*b=b*a$
- ***Può*** esistere un elemento $e_1$ : $\exists e_1\in S:\forall a \in S\quad e_1 * a= a$ chiamato elemento neutro sinistro
- ***Può*** esistere un elemento $e_2$ : $\exists e_2\in S:\forall a \in S\quad a*e_1= a$ chiamato elemento neutro destro
- ***Può*** esistere un elemento $e$ : $\exists e\in S:\forall a \in S\quad a*e=e*a=a$

**Lemma**: Un insieme $S$ con operazione $*$ : $(S,*)$ ammette un solo elemento neutro sinistro $e_1$, e solo un elemento neutro destro $e_2\qquad e_1=e_2$ 

> [!note] Dimostrazione
> $e_1=e_1*e_2=e_2$ in quanto $e_1=e_1*e_2$ perché $e_2$ è l'elemento neutro a destra
> $H_p$
> Avendo $(S,*)$ quanti elementi neutri ci sono?
> Supponiamo per assurdo che ci siano sia l'elemento neutro $e$ che e l'elemento neutro $e_1$:
> $e*e_1=e$
> Ma allo stesso tempo
> $e*e_1=e_1$
> Il che implica che: $e=e_1$ confermando che ce n'è solo uno