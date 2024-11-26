---
Time: 2024-11-26 12:17
---
$A \subseteq ℝ$
- $x_0\in A, x_0$ si dice *interno* ad $A$ se $\exists\delta\in ℝ^+_*\mid I_\delta (x_0) \subseteq A$
![[Pasted image 20241126120307.png|600]]
Se $A$ è formato solo da punti interni si dice *aperto*. L'insieme dei punti interni di $A$ si indica con $\overset{\circ}{A}\subseteq A$

$A = (a;b) = \overset{\circ}{A}$
$A = [a;b]$

- Sia $x_0\in ℝ, x_0$ è un *punto esterno* ad $A$ se $\exists \delta \in ℝ^+_* \text{ tale che }I_\delta(x_0)\cap A \neq \varnothing, \quad I_\delta(x_0) \subseteq ℝ - A$
- $A$ si dice chiuso se $ℝ-A$ è *aperto*
	- Per convenzione $ℝ$ e $\varnothing$ sono sia aperti che chiusi
- $x_0 \in A$ è un *punto isolato* di $A$ se $\exists I_\delta(x_0)\mid I_\delta(x_0)\cap A =\{x_0\}$
- Se i punti di $A$ sono tutti isolati, $A$ si dice *insieme discreto*. Ciò avviene negli insiemi $ℕ$ e $ℤ$ perché non ci sono altri numeri tra due numeri (per esempio tra $1$ e $2$ non c'è $\frac{1}{2}$)
- Sia $x_0\in \overline{ℝ}$
  $x_0$ si dice *punto di accumulazione per $A$* se $\forall I_\delta(x_0), \delta \in ℝ^+_*:I_\delta(x_0)\cap A \neq \{x_0\}$
- L'insieme dei punti di accumulazione di $A$ si chiama derivato di $A$, $D(A)$
- $A$ si dice *perfetto* se $D(A)=A$, quindi i suoi punti sono tutti d'accumulazione.
  $ℕ$ per esempio ha un solo punto di accumulazione $+\infty$
