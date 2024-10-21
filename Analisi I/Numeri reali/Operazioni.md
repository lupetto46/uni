# Proprietà di Archimede
$\forall x,y \in ℝ^*_{_+} \exists n\in ℕ^*:nx\geq y$
Che significa che esiste sempre un multiplo di  $x\inℝ^*_{_+}$ maggiore di $y\in ℝ^*_{_+}$

> [!question]- Cosa sono quei segni negli insiemi?
> Il $*$ indica che si sta prendendo tutto l'insieme escluso lo zero quindi $ℝ^*=ℝ-\{0\}$
> Il $+$ indica invece che si stanno prendendo solo i valori $\geq 0$ quindi i numeri positivi
> Al contrario il $-$ indica invece che dell'insieme si stanno prendendo solo i numeri negativi
> Possono andare in coppia per dire di prendere i numeri *strettamente* maggiori o minori di zero

Questo è utile per esempio quando si stanno prendendo disuguaglianze tra segmenti:
$\overline{AB}<\overline{CD}\exists n\inℕ:n\overline{AB}>\overline{CD}$

# Densità di ℚ in ℝ
$\forall \alpha, \beta\in ℝ, \alpha < \beta\exists r\in ℚ:\alpha<r<\beta$
Per ogni alfa e beta in ℝ con alfa minore di beta esiste un numero r in ℚ tale che r è compreso tra alfa e beta
questo dice che tra due numeri reali esiste sempre un numero razionale
Questa proprietà viene anche chiamata densità di $ℝ-ℚ$ in $ℝ$ 

Questo è diverso dall'elemento di separazione di $ℝ$ che dice che:
$\forall \alpha,\beta \in ℝ,\alpha < \beta \exists \delta\in ℝ: \alpha<\delta<\beta$
Tra due numeri reali c'è sempre in mezzo un numero reale

## Potenze con esponente reale
$\forall a \in ℝ\wedge \forall n\in ℕ, n\neq 0$
Si definisce potenza n-esima
$a^n=\cases{a\qquad se\ n=1\\a\cdot a\cdot a\cdot a\cdot\ \dots\ \cdot a\qquad se\ n>1}$
### Proprietà della potenza
Ho scritto solo quelle che non sapevo o che non sono semplici.
- $n<m\cases{a^n<a^m\qquad se\ a>1\\a^n>a^m\qquad se\ 0<a<1}$
- $0\leq a<b\qquad a^n<b^n$

# Radice, potenza e logaritmo
## Esistenza e unicità della radice n-esima aritmetica
Siano $n\in ℕ, n\geq2,y\in ℝ_{_+}\exists^{1}x\in ℝ_{_+}:x^n=y$
Questo dice quindi che $\sqrt[n]{y}=x$

Ma adesso prendiamo un valore $r=\frac{m}{n}\in ℚ,\qquad m\in ℤ,n\inℕ^*$

Di cui $(a^r)^n=a^{rn}$
Ma $r = \frac{m}{n}$ quindi $a^{rn}=a^{\frac{m}{\cancel{n}}\cancel{n}}=a^m$

Abbiamo quindi $a^{\frac{m}{n}}=a^r=\sqrt[n]{(a^{\frac{m}{n}})^n}=\sqrt[n]{a^m}$

## Esistenza e unicità del logaritmo
Sia $a\in ℝ\qquad a >0\qquad a \neq 1$
$\forall y>0\exists^1x\in ℝ:a^x=y\Leftrightarrow \log_a y = x$

### Proprietà
$a^{\log_ay}=y$
$\log_aa^x=x$
$\log_a1=0$
$\log_aa=1$
$\log_a x\cdot y=\log_a x + \log_a y$
$\log_a \frac{x}{y}=\log_ax-\log_ay$
$\log_a\frac{1}{x}=-\log_ax$
$\log_ax^n=n\log_ax$
$\log_nb=\frac{\log_ab}{\log_an}$

