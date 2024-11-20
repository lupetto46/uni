$\ker (f) =\left\{v\in V\mid f(v) = 0\right\} \subseteq V$
Quindi il kernel di $f$ è l'insieme di tutte le $v\in V$ tali che $f(v) = 0$

$Im\ f= \left\{w\in W \mid \exists v \in V:f(v) = w\right\} \subseteq W$
Quindi l'immagine di $f$ è l'insieme di tutte le $w$ immagini di $f$

> [!success] Proposizione 1
> $$
> f:V\longrightarrow W \text{ omomorfismo}
> $$
> $\ker f$ è un sottospazio di $V$
> $Im\ f\subseteq W$ è un sottospazio di $W$

> [!success] Proposizione 2
> $$
> f: V\longrightarrow W \text{ omomorfismo}
> $$
> $V = <v_1,\ldots,v_m>$
> Allora
> $Im\ f=<f(v_1), \ldots, f(v_m)>$
> %%Inserire la dimostrazione scritta negli appunti%%

> [!success] Osservazione
> Se $\{v_1, \ldots, v_m\}$ base di $V \centernot{\implies}\{f(v_1), \ldots, f(v_m)\}$ base di $Im(f)$

Similmente al [[#^a5f396|teorema del rango]]:
$dim(\ker(f)) =: null(f)$
$dim(Im(f)) =: rk(f)$

> [!success] Teorema
> $null(f) + rk(f) = dim(v)$

$$
\begin{align}
&U,V,W\text{ tre spazi vettoriali su }K\\
& f:U \longrightarrow V, \qquad g: V\longrightarrow W\\
\end{align}
$$

$$
\begin{align}
g\circ f: U &\longrightarrow W\\
u& \longmapsto g(f(u))
\end{align}
$$


> [!success] Lemma
> Se $f,g$ sono applicazioni lineari allora $g\circ f$ è un'applicazione lineare

$V$ uno spazio vettoriale
$f:V\longrightarrow V$ è un applicazione lineare e un endomorfismo

Sia $V,W$ spazi vettoriali

$L(V,W)=\{V\longrightarrow W\text{ applicazioni lineari}\}$
Che è allo stesso momento uguale a
$Mor(V,W)$ e $Hom(V,W)$

$L(V,V)= End(V)$