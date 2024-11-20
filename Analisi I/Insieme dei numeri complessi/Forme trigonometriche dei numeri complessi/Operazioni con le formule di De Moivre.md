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
Ottenendo la proprietà: $z^n=\rho^n(\cos n\theta+\sin n\theta)\qquad n\in ℤ$

> [!todo] Dimostrazione
> Utilizziamo la tecnica per induzione perché stiamo dimostrando una proprietà in funzione di numeri interi
> 
> $z^n=\rho^n(\cos n\theta+\sin n\theta)\qquad n\in ℤ$
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
> Adesso vediamo con $n=0$
> $z^0 = \rho^0(\cos 0 + i \sin 0) = 1$
> 
> Adesso vediamo i casi in cui $n<0$
> poniamo $n=-m$
> $$
> z^{-m}=\frac{1}{z^m}=\rho^{-m}\frac{1}{(\cos m\theta+i\sin m\theta)}
> $$
> Qui possiamo [[Insieme dei numeri complessi#^de4687|semplificare]]
> $$
> \begin{align}
> &\rho^{-m}\frac{(\cos m\theta-i\sin m\theta)}{\underbrace{\cos^2m\theta+\sin^2 m\theta}_1}=\\
> =&\rho^{-m}(\cos (-m)\theta+i\sin (-m)\theta)=\rho^n(\cos n\theta+i\sin n\theta)
> \end{align}
> $$
> 
> Finendo così la dimostrazione