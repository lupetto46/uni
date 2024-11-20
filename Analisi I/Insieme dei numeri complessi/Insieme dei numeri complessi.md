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
  Approccio assiomatico : $z + z_1 = (a + c ; b + d)$
- $z\cdot z_1=ac-bd+i(bc+ad)$
  Approccio assiomatico : $z+z_1= (ac - bd ; bc - ad)$
- $\frac{z}{z_1}=\frac{a+bi}{c+di}$ Qui si fa come se si stesse semplificando una radice quadrata al denominatore quindi $\frac{a+bi}{c+di}\cdot \frac{c-di}{c-di}=\frac{(ac+bd)+i(bc+ad)}{c^2+d^2}=\frac{ac+bd}{c^2+d^2}+i\frac{bc+ad}{c^2+d^2}$ ^de4687