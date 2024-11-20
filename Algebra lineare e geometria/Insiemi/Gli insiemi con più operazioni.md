### Definizione di anello
Per essere un anello è un insieme non vuoto con due operazione $+$ e $\cdot$ devono essere:
1) $(S,+)$ sia un gruppo abeliano con elemento neutro $0$
2) $(S,\cdotp)$ un semigruppo
3) $\forall a,b,c\in S,\quad a\cdot(b+c)=a\cdot b+a\cdot b,a\cdot(b+c)=a\cdot b+a\cdot c$
4) Se la moltiplicazione è commutativo l'anello si chiama commutativo
5) Se la moltiplicazione ammette un elemento neutro $1$ l'anello si dice unitario
6) $(S,+,\cdotp,0)$ è un anello. Siano $a,b\in S: a\cdot b=0$ oppure $b\cdot a= 0$ allora $a$ e $b$ si dicono **divisori dello zero**
7) Se $(S, +, \cdotp, 0)$ non ha divisioni dello zero si dice un dominio di integrità
8) Se $(S\backslash\{0\}, \cdotp)$ è un gruppo abeliano con elemento neutro $1\neq 0$ allora $(S, +, \cdotp,0,1)$ si dice **un campo** (Un anello commutativo in cui ogni elemento diverso da 0 è invertibile rispetto alla moltiplicazione) ^db328e

> [!note] Esempio
> $(ℤ, +, \cdotp, 0, 1)$ è un anello commutativo unitario è quindi dominio di integrità perché non ci sono numeri diversi da zero che se moltiplicati hanno $0$, ma non è un campo.
> $(ℚ, +, \cdotp, 0, 1)$ è un campo
> $(ℝ, +, \cdotp, 0, 1)$ è un campo
> $(\frac{ℤ}{nℤ}, +, \cdotp, \overline{0}, \overline{1})$ è un campo se $n$ è primo
> $(\frac{ℤ}{nℤ}, +, \cdotp, 0, 1)$ è "solo" un anello commutativo unitario se $n$ non è primo