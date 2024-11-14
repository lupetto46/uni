---
Data: 24-11-2024
---


# Il valore assoluto
importante ricordare che il risultato del valore assoluto prende il valore assoluto dell'intero argomento e non solo della $x$
$|argomento|=\cases{argomento\ se\ argomento\geq0\\-argomento\ se\ argomento <0}$
> [!example] esempio
> $|x^2+x+1|=\cases{x^2+x+1\ se\ x^2+x+1\geq0\\-(x^2+x+1)\ se\ x^2+x+1<0}$
> O ancora meglio
> $|x^2-1|$
> $x^2-1\qquad x=\pm1$
> $x^2-1\geq 0\qquad x\leq-1\wedge x\geq1$
> $x^2-1<0\qquad -1<x<1$
> Quindi:
> $|x^2-1|=\cases{x^2-1\ se\ x\leq-1\wedge x\geq1\\ -x^2+1\ se\ -1<x<1}$

## Proprietà del valore assoluto
Il valora assoluto ha delle proprietà:
$\forall a,b\inℝ$
1. $|a| \geq0\qquad |-a|=a\qquad a\leq|a|$
2. $|a|=0 \Longleftrightarrow a=0$
3. $|a|^2=a^2$
4. $|a\cdot b|= |a|\cdot|b|$
5. $|a+b|\leq|a|+|b|$
6. $|A-B|\geq ||A|-|B||$
7. $|A|\leq B \Longleftrightarrow -B\leq A \leq B$
8. $|A-B|=0\Longleftrightarrow A=B$
9. $|\frac{A}{B}| = \frac{|A|}{|B|}$

# Equazioni e disequazioni con valore assoluto
## Equazioni
$|A(x)|=K\qquad k\in ℝ$
Ci sono vari casi che si possono avere:
1. $K<0$ in questo caso sappiamo che il valore assoluto non può risultare un valore minore di zero quindi $\nexists x \in ℝ$
2. $K=0$ nel caso in cui $A(x)=0$
3. $K>0$ per ottenerlo allora devo porre $A(x)=\pm K$

Se l'uguaglianza e tra due valori assoluti allora le soluzioni sono le $x$ che annullano entrambi i membri

$|x-1|=|x^2-1|\qquad x=-1$

Se l'equazione trova la $x$ in posti fuori dal valore assoluto allora si deve fare la mappa dei segni del valore assoluto

## Disequazioni
Anche qui con $A(x)> K$ 
Troviamo varie situazioni
1. $K<0$ se $K$ è minore di $0$ il valore assoluto sarà sempre confermato in quanto qualsiasi numero sarà sarà sempre $\geq 0$ quindi la risposta è $\forall x \in ℝ$
2. $K=0$ per risolverla si deve porre $A(x)\neq 0$
3. $K>0$ si prendono gli esterni $A(x)<-K \vee A(x)>K$

Mentre invece se ho la disuguaglianza $A(x)<K$
1. $K<0$ non è possibile che $A(x)$ dia in valora minore di un valore minore di zero quindi $\nexists x \in ℝ$
2. $K=0$ anche qui $A(x)$ non può dare un valore minore di $0$ ma la diseguaglianza da che il valore deve essere *strettamente* minore di $0$ quindi anche qui $\nexists x \in ℝ$
3. $K>0$ per risolverlo invece si devono prendere i valori interni $-K<A(x)<K$ che alla fine non altro che svolgere il sistema $\cases{A(x)>-K\\A(x)<K}$

