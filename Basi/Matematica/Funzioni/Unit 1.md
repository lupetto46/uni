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

Ma come si trova l'inversa di $f$ ?
$$
\begin{align}
y&=2x+1\\
y-1 &= 2x\\
{y-1 \over 2} &=x
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
# Il grafico e come trovare le sue proprietà
## Suriettiva o Iniettiva
Prendendo una funzione $f: [a,b] \rightarrow ℝ$ 
![[Pasted image 20240809125204.png]]
Si può vedere che:
- **Non** è [[#iniettiva]] in quanto ci sono due punti con la stessa ordinata (scritti in blu)
- **Non** è [[#Suriettiva]] in quanto il punto $d$ non viene toccato nonostante il codominio sia $ℝ$


---
Mentre invece prendendo sempre la stessa funzione $f: [a,b] \rightarrow ℝ$ 
![[Pasted image 20240809125512.png]]
Si può vedere che:
- È [[#iniettiva]] in quanto non ci sono punti dell'asse $y$ che vengono toccati 
- **Non** è [[#suriettiva]] in quanto il punto $d$ (scritto in blu) non viene toccato nonostante il codominio sia tutto $ℝ$

---
Un altro esempio un po' più complicato è:
Prendendo sempre una funzione $f: [a,b] \rightarrow ℝ$
![[Pasted image 20240809125844.png]]
Si può vedere che:
- **Non** è [[#iniettiva]] in quanto la parte iniziale e la parte finale è dritta e quindi hanno lo stesso valore $y$ con diverse $x$
- È [[#suriettiva]] in quanto la funzione (come si vede dal tratteggiato agli estremi) continua per l'asse $y$ all'infinito prendendo quindi qualsiasi numero in $ℝ$

---
Prendiamo anche il caso in cui sia dominio che codominio sono finiti
$f: [a,b] \rightarrow [c, d]$
![[Pasted image 20240809130213.png]]
Si può vedere che:
- **Non** é [[#iniettiva]] in quanto ci sono dei punti che vengono toccati più di una volta
- Ma è [[#suriettiva]] in quanto tutta l'asse $y$ coperta dal codominio $[c,d]$ viene toccata dal grafico della funzione

## Pari o Dispari
### Pari
Una funzione $f: [-a,a] \rightarrow ℝ$ è detta **pari** se per ogni $x \in [-a, a]$ si ha $f(-x) = f(x)$

E lo si nota dal grafico in quanto questo viene specchiato rispetto all'asse delle ordinate
![[Pasted image 20240809130539.png]]

### Dispari
$f:[-a,a] \rightarrow ℝ$ è dispari se per ogni $x \in [-a, a]$ si ha  $f(-x)= -f(x)$

E lo si nota dal grafico in quanto viene specchiata sia dall'asse delle ordinate ($y$) che da quello delle ascisse ($x$)
![[Pasted image 20240809131202.png]]

## Crescente o Decrescente
### Crescente
Una funzione $f: [a,b] \rightarrow ℝ$ è **crescente** se per ogni $x \leq y \in [a,b]$ si ha
$f(x) \leq f(y)$ 
![[Pasted image 20240809131643.png]]
### Decrescente
Una funzione $f: [a,b] \rightarrow ℝ$ è **decrescente** se per ogni $x \leq y \in [a,b]$ si ha
$f(x) \geq f(y)$ 
![[Pasted image 20240809135326.png]]
## Grafico funzioni invertibili
Avendo