## Approccio elementare
I numeri complessi si scrivono con il segno $ℂ$ 

Prendiamo come esempio più naturale è il caso della radice dei numeri reali 
$\sqrt[n]{a}\qquad a\geq 0$

Seguendo la matematica l'operazione tra due numeri reali dovrebbe restituire dare un numero reale

Ma nel caso in cui la $a < 0$?
In questo caso è necessario introdurre l'unità immaginaria $i$
Questa gode di una proprietà importante ovvero $i^2=-1$

Numeri come $2i$ $,-\frac{1}{2}i$ $,\sqrt{i}$ si chiamano numeri immaginari.

La somma tra numeri immaginari e numeri reali si chiamano numeri complessi.
$z=a+bi\inℂ$ con $a,b\in ℝ$

Di questa $z$ si dice:
- $Re(z)$ la parte reale
- $Im(z)$ la parte immaginaria

Se nel numero reale $z=a+bi\qquad b=0$ allora questo è un numero reale
Altrimenti se $z=a+bi\qquad a=0$ allora questo sarà un numero immaginario.

Un numero complesso si può anche scrivere come insieme di coppie ordinate di reali $(a,b)$ con $a,b\in ℝ$
### Il coniugato di $z$
Si indica con $\overline{z}=a-bi$ e gode di una certa proprietà, ovvero:
$z\cdot \overline{z}=(a+bi)(a-bi)=a^2-b^2i^2$ ma visto che $i^2=-1$ il risultato finale sarà:
$a^2+b^2$ quindi un numero reale

### Modulo di $z$

$|z|=\sqrt{a^2+b^2}$

### Operazioni con numeri complessi
$z=a+bi\qquad z_1=c+di$
- $z+z_1=(a+c)+i(b+d)$
- $z\cdot z_1=ac-bd+i(bc-ad)$
- $\frac{z}{z_1}=\frac{a+bi}{c+di}$ Qui si fa come se si stesse semplificando una radice quadrata al denominatore quindi $\frac{a+bi}{c+di}\cdot \frac{c+di}{c+di}=\frac{(ac+bd)+i(bc+ad)}{c^2+d^2}=\frac{ac+bd}{c^2+d^2}+i\frac{bc+ad}{c^2+b^2}$ ^de4687

## Adesso si definiscono le addizioni e le moltiplicazioni
Si definiscono le operazioni e si controlla se hanno tutte le proprietà di cui devono godere:
$z=a+bi\qquad z_1=c+bi\qquad a,b\inℝ\qquad c,d\inℝ$
- **Moltiplicazione**:
	- $z\cdot z_1=((ac-bd);(ad+bc))$ *Sta venendo usata la rappresentazione come coppie ordinate di numeri reali*
	- Ha la proprietà commutativa $z\cdot z_1=z_1\cdot z$
	- Ha la proprietà associativa $(z\cdot z_1)\cdot z_2=z\cdot (z_1\cdot z_2)$
	- $\exists$ un elemento neutro ovvero $(1;0)$
	- Ogni elemento è simmetrizzabile per $\forall z=(a;b)\in ℂ\exists z^{-1}(\frac{a}{a^2+b^2};-\frac{b}{a^2+b^2})\in ℂ$
- **Addizione**:
	- $z+z_1=(a+c;d+b)$
	- Ha la proprietà commutativa $z+ z_1=z_1+ z$
	- Ha la proprietà associativa $(z+ z_1)+ z_2=z+ (z_1+ z_2)$
	- $\exists$ un elemento neutro ovvero $(0;0)$
	- Ogni elemento è simmetrizzabile $\forall z=(a;b)\in ℂ \exists -z=(-a;-b)\in ℂ$

Ci sono inoltre altre proprietà come
$i^2=(0;1)(0;1)=((0\cdot0-1\cdot1);(0\cdot 1+0\cdot 1))=(-1;0)$

## Proprietà di $z$
### Proprietà del modulo di $z$
Riscriviamo il modulo di $z$:
$|z|=\sqrt{a^2+b^2}\qquad a+ib\in ℂ\qquad (a;b)\in ℂ$

1. $|z|\geq 0$. Nel caso in cui $|z|=0$ allora $z=0$ quindi $a=0,b=0\Rightarrow (0;0)$ 
2. $|z\cdot w|=|z|\cdot|w|$ di cui $w=c+id\qquad w(c,d)$
3. $|z|=|\overline{z}|$
4. $|z+w|\leq |z|+|w|$
5. $|z|\geq Re(z)\qquad |z|\geq Im(z)$
6. $|z|\leq Re(z)+Im(z)$

### Proprietà del coniugato 
1. $\overline{z}+\overline{w}=\overline{z+w}$
2. $\overline{z}\cdot\overline{w}=\overline{z\cdot w}$
3. $\overline{\overline{z}}=z$
4. $z=\overline{z}\Leftrightarrow z\in ℝ$
5. $z-\overline{z}=2Re(z)$
6. $z+\overline{z}=2Im(z)$
7. $z\cdot\overline{z}=|z|^2$

# Forme trigonometriche dei numeri complessi
Consideriamo una retta $s$ di origine $O$ detta anche polo del sistema di riferimento.

![Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna](data:image/png;base64,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)
Il segmento $\overline{OP}$ viene chiamato $\rho$ (rho) e l'angolo che spazza il segmento $\rho$ viene chiamato $\theta$ e aumenta di segno positivo se va in senso antiorario

Il nostro punto $P$ ha coordinate $P(\rho;\theta)$ con $\rho>0\qquad \theta\in[0,2\pi]$


## Piano di Argand-Gauss
Per unire questa cosa ai numeri complessi si mette in un sistema di assi cartesiane in cui come ascissa c'è la retta dei numeri reali e come ordinata c'è l'asse immaginaria
![Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna
Disegni a penna](data:image/png;base64,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)

Di cui la coppia $(a;b)$ sono:
$$
\cases{a=\rho\cos\theta\\ b=\rho\sin\theta}
$$

Per poi unire definitivamente le due cose dicendo che 
$$
z=a+bi=\rho(\cos\theta+i\sin\theta)
$$

Ottenendo quindi una relazione tra le coordinate cartesiane e le ordinate polari
Ma adesso poniamo tutti e due i membri elevati al quadrato
$a^2=\rho^2\cos^2\theta$
$b^2=\rho^2\sin^2\theta$
$a^2+b^2=\rho^2(\underbrace{\cos^2\theta+\sin^2\theta}_{1})$
Quindi $\rho=\sqrt{a^2+b^2}=|z|$

Quindi tornando alla formula prima 
$$
\begin{cases}
a=\rho\cos\theta\qquad \cos\theta=\frac{a}{\rho}=\frac{a}{\sqrt{a^2+b^2}}\\
b=\rho\sin\theta\qquad \sin\theta=\frac{b}{\rho}=\frac{b}{\sqrt{a^2+b^2}}
\end{cases}
$$

### Quando due numeri complessi in forma trigonometrica sono uguali?
quando avendo
$z=\rho(\cos\theta+i\sin\theta)$
$z_1=\rho_1(\cos\theta_1+i\sin\theta_1)$

Sono uguali quando $\theta= \theta_1$ oppure gli angoli differiscono di $2k\pi$ (*un giro completo*)

Questo perché 
- $\sin(\theta+2k\pi)= \sin\theta$
- $\cos(\theta+2k\pi)=\cos\theta$

## Operazioni con le formule di De Moivre
### Prodotto
Avendo:
$z=\rho(\cos\theta+i\sin\theta)\qquad z_1=\rho_1(\cos\theta_1+i\sin\theta_1)$


$z\cdot z_1=\rho(\cos\theta+i\sin\theta)+\rho_1(\cos\theta_1+i\sin\theta_1)=$
Seguendo le proprietà:
- $\cos(\alpha+\beta)=\cos\alpha\cos\beta-\sin\alpha\sin\beta$
- $\sin(\alpha+\beta)=\cos\alpha\sin\beta+\sin\alpha\cos\beta$

Otteniamo che è uguale a
$=\rho\cdot\rho_1[\cos\theta\cos\theta_1+i\sin\theta_1\cos\theta+i\sin\theta\cos\theta_1-\sin\theta\sin\theta_1]$
$=\rho\cdot\rho_1[(\overbrace{\cos\theta\cos\theta_1-\sin\theta\sin\theta_1}^{\cos(\theta+\theta_1)})+i(\overbrace{\sin\theta_1\cos\theta+\sin\theta\cos\theta_1}^{\sin(\theta+\theta_1)})]$

### Potenza di numeri interi
Avendo questa proprietà:
$z\cdot z_1=\rho\cdot\rho_1[({\cos\theta\cos\theta_1-\sin\theta\sin\theta_1})+i({\sin\theta_1\cos\theta+\sin\theta\cos\theta_1})]$

Possiamo ricavare nel caso in cui $z_1=z$ che:
$z^2=\rho^2(\cos2\theta+i\sin2\theta)$
Ottenendo la proprietà: $z^n=\rho^n(\cos n\theta+\sin n\theta)\qquad n\in ℤ,n\neq0$

> [!todo] Dimostrazione
> Utilizziamo la tecnica per induzione perché stiamo dimostrando una proprietà in funzione di numeri interi
> 
> $z^n=\rho^n(\cos n\theta+\sin n\theta)\qquad n\in ℤ,n\neq0$
> 
> Inizialmente consideriamo i casi in cui $n>0$
> $n=1$ otteniamo:
> $z=\rho(\cos\theta+i\sin\theta)$ che è vera.
> 
> Adesso vediamo il caso in cui $n=k+1$
> $z^{k+1}=\rho^{k+1}(\cos(k+1)\theta+i\sin (k+1)\theta)$
> $z^k\cdot z=\rho^k(\cos k\theta+i\sin k\theta)\cdot \rho(\cos \theta+i\sin \theta)=$
> $=\rho^{k+1}(\cos k\theta\cos\theta+i\cos k\theta\sin\theta+i\sin k\theta \cos\theta-\sin k\theta\sin\theta)=$
> $=\rho^{k+1}(\cos(k+1)\theta+i\sin(k+1)\theta)$
> 
> Adesso vediamo i casi in cui $n<0$
> poniamo $n=-m$
> $$
> z^{-m}=\frac{1}{z^m}=\rho^{-m}\frac{1}{(\cos m\theta+i\sin m\theta)}
> $$
> Qui possiamo [[#^de4687|semplificare]]
> $$
> \begin{align}
> &\rho^{-m}\frac{(\cos m\theta-i\sin m\theta)}{\underbrace{\cos^2m\theta+\sin^2 m\theta}_1}=\\
> =&\rho^{-m}(\cos (-m)\theta+i\sin (-m)\theta)=\rho^n(\cos n\theta+i\sin n\theta)
> \end{align}
> $$
> 
> Finendo così la dimostrazione
