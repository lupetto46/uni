Si scrive $A \subseteq B$ se tutti gli elementi di $A$ sono anche elementi di $B$

## Iniettiva
Per ogni elemento **distinto** di $A$ o dominio ci sarà una corrispondenza con un elemento **distinto** di $B$ o codominio
## Suriettiva
Per **ogni** elemento di $B$ o codominio ci sarà una corrispondenza con un elemento **qualsiasi** di $A$ o dominio
## Biiettiva
Quando è sia [[#Iniettiva]] che [[#Suriettiva]]
## Esempio funzione
La funzione:
$f: ℕ \rightarrow ℕ,\ f(x)=2x+1$ 
è [[#iniettiva]] in quanto $2x_1 +1 = 2x_2 +1$
Ma non [[#suriettiva]] in quanto $2x +1=y$ implica che $2x = y - 1$ 
Di conseguenza la $x$ sarà sempre pari e la $y$ sarà sempre un risultato dispari
Questo vuol dire che del **Codominio** $ℕ$ corrisponderanno solo i numeri dispari al **Dominio**

## Esempio funzione con esponente
Prendiamo di esempio:
$f: ℝ \rightarrow ℝ,\ f(x)=x^2$
Non è iniettiva in quanto per esempio
$f(-2)=4$ e $f(2) = 4$
Due valori **distinti** di $x$ danno quindi lo stesso risultato
Non è nemmeno suriettiva in quanto per esempio $-4 \neq f(x) \forall x\in ℝ$   
Quindi non esistendo un numero in cui viene dato $-4$ non può essere iniettiva 

Mentre invece:
$f:ℕ \rightarrow ℕ,\ f(x)=x^2$
è iniettiva in quanto non ci sono numeri negativi
Ma non è su