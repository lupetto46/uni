### Definizione
Prendiamo un insieme $V$ e due operazioni $(V, +, 0)$ un gruppo abeliano questo è considerabile spazio vettoriale se:
- $\forall v,w,u\in V, (v+w)+u=v+(w+u)$ l'addizione è associativa
- $\forall v \in V ,\quad v+0=v \qquad 0+v = v$  esiste un elemento neutro dell'addizione
- $\forall v \in V, \exists v' \in V : v+v'=0\qquad  v'+v=0 \qquad (v' := -v)$ esiste un elemento inverso
- $\forall v, v' \in V, \quad v+v'=v'+v$ l'addizione è commutativa

Inoltre assumiamo di avere una moltiplicazione sul campo $K$:

$$
\begin{align*}
    K &\longrightarrow V \\
    (\lambda, v) &\longmapsto \lambda \cdot v
\end{align*}
$$

E vogliamo che $\forall \lambda \in K, \forall v \in V, \lambda V\in V$
- $\forall \lambda\in K, \forall v, v' \in V,\qquad \lambda \cdot (v+v')=\lambda \cdot v + \lambda \cdot v'$ la moltiplicazione è distributiva rispetto alla somma da sinistra
- $\forall \lambda, \lambda' \in K, \forall v \in V, \qquad (\lambda + \lambda') \cdot v = \lambda \cdot v + \lambda' \cdot v$ la moltiplicazione è distributiva rispetto alla somma anche da destra
- $\forall \lambda, \lambda' \in K, \forall v \in V, \qquad (\lambda \cdot \lambda') \cdot v = \lambda \cdot (\lambda' \cdot v)$ 
- $\forall v \in V \quad 1 \cdot v = v$ esiste l'elemento neutro della moltiplicazione

Un insieme V con queste proprietà su un campo $K$ è detto spazio vettoriale su $K$ di cui:
- Gli elementi di $V$ sono detti vettori
- Gli elementi di $K$ sono detti scalari

#### Esempi
L'esempio più base che si può fare con ciò di cui abbiamo già parlato sono le matrici. 

Infatti se consideriamo solo le matrici quadrate di ordine $n$ con le operazioni di somma e prodotto per uno scalare, queste formano uno spazio vettoriale.
$$(M_{n,n}, +, 0)$$
è un gruppo abeliano e quindi uno spazio vettoriale su $K$.

Altri esempi di spazi vettoriali su $K$ sono:
- $\{0\}$ chiamato spazio vettoriale nullo
- $K^n = \{(x_1, \dots, x_n) \mid x_i \in K\}$
	In quanto a questo spazio vettoriale si può dire che:
	- $(x_1, \dots, x_n) + (y_1, \dots, y_n) = (x_1 + y_1, \dots, x_n + y_n)$ e quindi si fa una somma componente per componente
	- $\lambda \cdot (x_1, \dots, x_n) = (\lambda x_1, \dots, \lambda x_n)$ e quindi si moltiplica ogni componente per lo scalare

Possiamo quindi notare come si somiglino: $K^n \cong M_{n,1}\cong M_{1,n}$

---
Un esempio un po' più complesso invece è:
Avendo $AX=0 \text{ sistema lineare omogeneo}, A\in M_{n,n}(K)$

$\Sigma_0 = \{\text{soluzioni di } AX=0\}$

avendo $\lambda \in K\qquad A(\lambda X) = \lambda (AX) = \lambda 0 = 0 \implies \lambda X \in \Sigma_0 \iff \Sigma_0$ è uno spazio vettoriale su $K$

---
Un altro esempio è:
$K[x]_n =$ polinomi su $K$ in una variabile $x$ di grado al più $n$

Avendo $f: \sum_{i=0}^n a_i x^i$ se si moltiplica la $f$ per uno scalare $\lambda \in K$ si ottiene: $\lambda f: \sum_{i=0}^n \lambda a_i x^i$