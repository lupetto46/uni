Per eseguire le equazioni del tipo $x^n=z$
### Teorema delle radici $n$-esime di un numero complesso
Sia $z=\rho e^{i\theta}= \rho(\cos\theta+i\sin\theta)\neq 0$ le soluzioni delle equazioni $x^n=z$ sono:
$$
\begin{cases}
1.\ x_k=\sqrt[n]{\rho}e^{i\phi k}\qquad \phi_k=\frac{\theta+2k\pi}{n}\\
2.\ k\in [0;n-1]
\end{cases}
$$

Quest ci permette di capire che:
1. Sono le soluzioni di $x^n=z$
2. Sono *tutte* e le *sole* soluzioni dell'equazione di $x^n=z$

> [!info] Dimostrazione
> Sia $X\in ℂ$ una soluzione dell'equazione $x^n=z$
> Allora sappiamo che $X=\sigma e^{i\phi}$
> Ma quindi sappiamo che $\sigma e^{i\phi}=z=\rho e^{i\theta}$
> 
> Per dimostrare dobbiamo applicare il principio di identità infatti 
> - $\sigma^n = \rho$ $\sigma$ elevato $n$ deve essere uguale a $\rho$
> Di conseguenza $\sigma =\sqrt[n]{\rho}$
> - $\cancel{i}\phi=\cancel{i}\theta$ i due esponenti dei numeri di nepero devono essere uguali
> 
> Sappiamo inoltre che $\exists k\in ℤ:n\phi=\theta + 2k\pi$
> 
> Giungendo sapendo quindi che $\phi = \theta$
> $$
> \begin{align}
> n\phi&= \theta+2k\pi\\
> \frac{\cancel{n}\phi}{\cancel{n}}&=\frac{\theta + 2k\pi}{n}\\
> \phi&=\frac{\theta + 2k\pi}{n}
\end{align}
> $$
> Ora si dimostra che le soluzioni sono distinte solo per l'intervallo $[0;n-1]$. Quindi se la radice è base $5$ allora i risultati saranno nell'intervallo $[0;4]$
> 
> Per dimostrarlo possiamo fare la prova con $k =n$
> 
> Sostituendo $n$ a $k$ otteniamo quindi:
> $$
> \phi=\frac{\theta +n \phi}{n}=\frac{\theta}{n}+\frac{\cancel{n}\pi}{\cancel{n}}= \frac{\theta}{n}+2\pi
> $$
> Questo significa che siamo andati oltre il primo giro e che quindi tutti i valori che otterremo visto che $\theta$ è periodico di $360\degree$ saranno gli stessi valori del giro prima
> 
> Adesso dimostriamo che sono le *sole*
> Supponiamo per assurdo esistano due risultati $x_{k_1}=\sqrt[n]{\rho}e^{i\phi k_1}$ e $x_{k_2}=\sqrt[n]{\rho}e^{i\phi k_2}$
> Calcoliamo quindi il loro $\phi$:
> - $\phi_{k_1}=\frac{\theta+2k_1\pi}{n}$
> - $\phi_{k_2}=\frac{\theta+2k_2\pi}{n}$
> 
> Sappiamo quindi che:
> - $0\leq \phi_{k_1}\leq\frac{\theta}{n}+2k_1\pi$
> - $0\leq \phi_{k_2}\leq\frac{\theta}{n}+2k_2\pi$
> 
> Ma se ne calcoliamo la differenza otteniamo:
> $\phi_{k_1}-\phi_{k_2}=\cancel{\frac{\theta}{n}}+2k_1\pi\cancel{-\frac{\theta}{n}}-2k_2\pi=2(k_1-k_2)\pi$ che differiscono di esattamente un angolo giro tra loro rendendoli per noi identici

