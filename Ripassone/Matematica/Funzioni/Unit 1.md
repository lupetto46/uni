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
Ma non è suriettiva in quanto ci sono numeri che non sono il quadrato di nessun numero
Come per esempio $2, 3\ o\ 5$

# Funzioni invertibili
Una funzione invertibile è una funzione in cui $A \rightarrow B$ può diventare $B \rightarrow A$
E deve soddisfare quindi  queste condizioni:
$f:A\rightarrow B$
$g:B\rightarrow A$ tale che:
- $a\in A:\ g(f(a))=a$
- $b\in B:\ f(g(b))=b$

Una funzione é inoltre invertibile solo se [[#Biiettiva]]

## Esempio
$f:ℝ\rightarrow ℝ, f(x)= 2x+1$
è biiettiva (lo abbiamo visto prima)
$g: ℝ \rightarrow ℝ$

$g(f(x))=x\ \forall x \in ℝ\qquad\qquad f(g(y))=y\ \forall y \in ℝ$

Ma come si trova l'inversa di $f$
$$
\begin{align}
&y=2x+1\\
&y-1 = 2x\\
&{y-1 \over 2} =x
\end{align}
$$

La nostra $g$ sarà quindi ${y-1 \over 2}$
# Il piano cartesiano
Serve per rappresentare tutti i punti in modo numerico
![[Pasted image 20240809001739.png]]
proviamo a fare il grafico di $f:[a,b] \rightarrow ℝ$ : 
Considerando il prodotto cartesiano $[a,b] \times ℝ \subseteq ℝ \times ℝ$ il grafico è un sottoinsieme: $g(f) = \{(x,y) \in [a, b] \times ℝ: y=f(x)\}$ 
Ovvero si prendono solo le coordinate il cui risultato della funzione per la prima coordinata è uguale alla seconda coordinata
![[Pasted image 20240809003806.png]]
Lezione 2 Unit 1 pagina 10