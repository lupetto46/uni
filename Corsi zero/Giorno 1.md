---
Data: 24-11-2024
---


# Giorno 1
## Concetti e notazioni
Per esistere, una funzione, si devono specificare le condizioni di esistenza quindi l'**Insieme di esistenza** o "**Dominio**" 
Una funzione dal terzo grado in poi non si può risolvere con le solite formule per esempio $\Delta= b^2 - 4ac$ 
Anche se in realtà è meglio abituarsi alle formule scritte con la notazione $a_2x^2 + a_1x + a_0$  invece di: $ax^2 + bx + c$

Ci sono infiniti più grandi di altri
Quanti numeri Naturali $ℕ$ ci sono? $\infty$
Quanti numeri ci sono tra $0$ e $1$? $\infty$
## Linguaggio matematico
Bisogna inoltre prendere consapevolezza che la matematica non ha contesto prendiamo quindi di esempio
$K \in ℝ,\ K > 0 \quad \rightarrow$ Comunque si segni $K$ esso é maggiore di 0
Si può quindi anche dire
$K\in ℝ, K>0, \exists h \in ℝ , h>0:, h > K$

Comunque si segni $K$ esso é maggiore di zero ed esisterà un numero $h$ maggiore di 0 a sua volta maggiore di $K$
## Polinomi
Gli zeri del polinomio indicano il valore che $x$ deve assumere per far restituire al polinomio $0$

Per poter essere risolto con delle normali formule risolutive il polinomio deve essere in **forma normale**
 > [!info] esempio
 > $3x^2-\frac{1}{2} + 2x + 2x^2 \cancel{+ x^3} \cancel{- x^3} - 1 =$ Non è in forma normale
 > $= 3x^2-\frac{1}{2} + 2x + 2x^2 - 1 =$
 > $= 5x^2 + 2x - \frac{3}{2}$ quindi in forma normale ovvero: $a_2x^2 + a_1x + a_0$

## Il segno opposto non il negativo
È importante ricordare che se si ha:
$sia\ A\in ℝ:-A\in ℝ$ 
Non significa che si ha il negativo $A$ ma che si ha il contrario di $A$ 

Un operatore da ricordare é il valore assoluto $|\cdot|$ il cui scopo é di restituire il valore positivo del numero che gli è stato inserito:
$$
|A|=\cases{A\ se\ A\geq0\\ -A\ se\ A < 0}
$$

## Trasformazioni del polinomio
Il polinomio si può tra sformare in vari modi ma come?
$a_2x^2 + a_1x + a_0 = 0$ Tutti i valori di $x$ che fanno ritornare al trinomio $0$
$a_2x^2 + a_1x + a_0 \geq 0$
$a_2x^2 + a_1x + a_0 \leq 0$
$y = a_2x^2 + a_1x + a_0$

Dando per scontato che 
$a_2\in ℝ,a_2 \neq 0$ 
$b, c \in ℝ$

## Il discriminante $(\Delta)$
Sul polinomio si può sapere tantissimo solo conoscendone il delta $\Delta$ o **discriminante** che ci permette di "predirne" il comportamento e ci permette di fare delle "**domande**" al polinomio
Questo può avere tre comportamenti
- $\Delta>0$
- $\Delta = 0$
- $\Delta < 0$

Ma per spiegarne le conseguenze prendiamo la funzione $y = a_2x^2 + a_1x + a_0$ e per semplicità diamo per scontato che $a_2 > 0$
La concavità della parabola sarà verso "l'*alto*" anche se a causa della decontestualizzazione della matematica ciò che si dice è che **ha la concavità verso l'asse le ordinate positive**

quindi avendo il $\Delta > 0$ allora si ha:
$Se\ \Delta>0\ si\ ha\ che\ \exists x_1,x_2 \in ℝ : a_2x^2 + a_1x + a_0 = a_2(x-x_1)(x-x_2)$

Mentre invece con $\Delta = 0$ si ha:
$Se\ \Delta =0\ si\ ha\ che\ a_2x^2 + a_1x + a_0 = (x+\alpha)^2, \alpha \in ℝ$ ***Sbagliato??***

> [!info] esempio
> $3x^2+\sqrt{3}x+\frac{1}{4}$
> $\Delta=\sqrt{3}^2-4(3)(\frac{1}{4})=3-3=0$
> Allora
> $3x^2+\sqrt{3}x+\frac{1}{4}=(x+\sqrt{3})^2$

È diverso il caso in cui $\Delta < 0$ in quanto:
Bisogna considerare in che insieme io stia lavorando
- Se sto lavorando nell'insieme dei numeri reali: $ℝ:a_2x^2+a_1x+a_0$ e non viene scomposto
- Se sto lavorando nell'insieme dei numeri complessi allora: $ℂ\ \exists z_1,z_2: a_2x^2+a_1x+a_0 = a(x-z_1)(x-z_2)$
	Esisteranno due numeri $z_1, z_2$

Ma come spiegare e mostrare questi risultati di delta:
Nel caso in cui $\Delta = 0$ allora si avrà solo un risultato (*o meglio si avrà lo stesso risultato molteplici volte in quanto $x_1\equiv x_2$*) e quindi si avrà il vertice ($-\frac{b}{2a}$) che toccherà l'asse delle ascisse
![[Pasted image 20240920181112.png]]
In questo caso:
$P(x)\geq 0, \forall x\in ℝ$
$P(x) > 0, \forall x \in ℝ \backslash\{ -\frac{b}{2a} \}$
$P(x) \leq 0, x= \{ -\frac{b}{2a}\}$
$P(x)<0,\ \emptyset$

Il caso in cui $\Delta > 0$ allora si avranno due risultati (quindi due zeri)
![[Pasted image 20240920182248.png]]
in cui
!Capire come scrivere!

Nel caso in cui invece $\Delta < 0$ quindi nessun risultato nell'insieme dei numeri reali
![[Pasted image 20240920182851.png]]

$P(x) \geq 0, \forall x \in ℝ$
$P(x) < 0, \emptyset$

