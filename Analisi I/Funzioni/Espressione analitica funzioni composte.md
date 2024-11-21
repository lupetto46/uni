---
Time: 2024-11-21 19:42
---
$\text{dom } (g\circ f)=\{x \in \text{dom } f: f(x) \in \text{dom }g\}$
$\text{Im } f \cap \text{dom }g \neq \emptyset$
$f:[0;+\infty)\to ℝ\qquad g:ℝ\to ℝ$
$f(x)= \sqrt{x}\qquad g(x) =-x^2 - 3$

$(g\circ f)(x) = g(f(x)) = -(\sqrt{x})^2-3=-x-3$
$x\xrightarrow{f}\sqrt{x}\xrightarrow{g} -x - 3$

La composizione non è commutativa infatti:
$(f\circ g)(x)=f(g(x))= \sqrt{-x^2 - 3}$
$\text{Im }g\cap\text{dom }f=\emptyset \implies (-\infty;-3]\cap[0;+\infty)\neq \emptyset$

> [!success] Definizione 1
> Sia $f_i:A\to A, A\neq \emptyset,\forall a\in A \text{ la legge }f(a)=a$
> $f:A\to B$
> $f^{-1}:B\to A$
> $f\circ f^{-1}(b) = f(f^{-1}(b))=f(a)=b=I_B$
> $(f^{-1} \circ f)(a) = f^{-1}(f(a))=f^{-1}(b)= a= I_A$