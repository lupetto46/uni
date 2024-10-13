#algebra_lineare_e_geometria 
## Polinomi a una variabile
I polinomi nascono seguendo la necessità di completare delle equazione i cui dati non si conoscono e quindi vengono sostituiti all'interno dell'equazione come *variabili*

Consideriamo $K$ un [[Insiemi#^db328e|campo]]. Uno dei polinomi su $K$ a una variabile è:
$$
K[x]=\{\sum_{i=0}^{n}\underbrace{a_ix^i}_{_{monomio}}|a_i\in K, a_n\neq 0\}\quad \underbrace{(K[x], +, \cdotp)}_\text{anello del polinomio}
$$

Si possono anche applicare le funzioni a questi polinomi:
$$
f\in K[x], f=\sum_{i=0}^{n}a_ix^i, a_n\neq 0
$$
Quindi $f$ appartiene al campo $K$ con come variabile $x$: $K[x]$ 

Si può poi trovare il grado: $deg (f):=n, \quad deg(0):=-\infty$

> [!hint] 
> Nella maggior parte dei cari tratteremo $K=ℝ$


## Polinomi a più variabili
Nel caso dei polinomi a più variabili abbiamo :
Sempre il campo $K$ e una $r\in ℕ>1$
La forma di un polinomio è:
$$
K[x_0,x_1,\dots,x_r]=\{\sum_{(i_1,\dots,i_n)\in I}a_{i_1}\cdots a_{i_r}\cdot x^{i_1}\cdots x^{i_r}|\underset{a_i,\dots,_{i_r}\in K }{I\ \text{finito}}\}
$$

Per quanto riguarda il grado invece:
$$
f\in K[x_1,\dots,x_r],\quad deg(f)=max(i_1,i_2,\dots,i_r)\in I
$$

> [!cite] Proposizione
> Se ho $f,g$ un anelli di polinomi a più variabili $deg (f\cdot g)=deg(f)+deg(g)$

> [!done] Osservazione
> L'anello di polinomi non è un gruppo perché non esiste l'inverso delle variabili $\nexists x^{-1}$

$f\in K[x_1,\dots,x_n]$
$f\text{ è invertibile }\Longleftrightarrow f\in K$
## Funzioni polinomiali


Avendo $f\in K[x_1,\dots,x_n]$

$\begin{align*}f:ℝ^r&\longrightarrowℝ \\ (a_1,\dots ,a_r)&\longmapsto f(a_1,\dots,a_r)\end{align*}$

### Composizione tra funzioni polinomiali
Avendo due funzioni polinomiali:

$\begin{align*}g:ℝ&\longrightarrowℝ\qquad,\qquad &h:ℝ\longrightarrowℝ \\ a&\longmapsto g(a) &a\longmapsto h(a)\end{align*}$

Componendole otteniamo quindi:
> [!example] Esempio
> Se $g=2x,h=x+1\in ℝ[x]$
>
> $\begin{align*}g\circ h:ℝ&\longrightarrow ℝ\\ a&\longmapsto g(h(a))\end{align*}$ Quindi $g(h(a))=2(a+1)=2a+2$
>
> Quindi $g\circ h =2x+2$
> Mentre $h\circ g= h(g(a))=2x+1$

## Equazione polinomiali
Le equazioni polinomiali sono due equazioni poste a una uguale all'altra

Prendiamo quindi $f=g\quad f,g\in K[x_1,\dots,x_r]$
La soluzione di $f=g$ è una r-upla $(a_1,\dots,a_r):f(a_1,\dots,a_r)=g(a_1,\dots,a_r)$
Questo vuol dire che *risolvere $f=g$ vuol dire trovare* ***tutte*** *le soluzioni*

## Divisione di polinomi
Per adesso faremo delle divisioni tra polinomi a una variabile

$f,g \in K[x]$
Dividere $\frac{f}{g}$ significa trovare una $q,r\in K$ il cui grado $deg\ q<deg\ g:f=g\cdot q + r$

### Come dividere?
Ci sono ben due modi per dividere un polinomio per un altro polinomio
1. Il metodo normale:
	$f=x^4-3x^3+4x^2-5x+7\qquad g=x^2-x+2$
	
	Si deve prendere il valore per il quale moltiplicare il divisore per rimuovere 
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
	Disegni a penna](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAX4AAADACAIAAACMD58aAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAADg4SURBVHhe7Z0FeBTXFsfXLZts3EOMQHB3p0CBltdSe6Vur30tbam9tq9KvbSPulNvoVSR4u7uSYjrJll3nd2Rd2Z3CIEIkc0ms9zfl2+Ze2fYHbv/e861w6UoioNAIBDBhcf8i0AgEEEESQ8CgegGkPQgEIhuAEkPAoHoBpD0IBCB4YOzxoRfS5N/K3vjjIHJQrRMj5YerZtgthCIHo/SgS8eGld1Q/YejfNvpZ3JRbRAD5WeU0b3zC3KF0/qmDQC0eOJEPHsXlLE416dKj+oczG5iBboidKzusY2Y4tyTJzky3GJTBYC0eOZGC+NFvOW5Bu+KjHPTA5jchEt0OOGFP5Qbrlrn+qTMQkLc6OYLASCDVTYvHO2KWenhN2RrRgRI2FyES3Qs6Tn40LTo0c0305Iuru3gsnqDoosHvjMVYj8SQSiLYC1/leN/ceJSUwa0So9yOF66pgWdOe3KSndqzsA1F2Ljmi+LjUz6Z5KscXzS6V1RYUVv4xnw3xSZLp9bz2T6Fau7RUu4XNnbFF+VGiyeUkmF9ECPcXquWZH3Vql7YG+kV+M7f72Hai+4POPatvPk5L9OT2QN/MMf1TZxsbB286VCrjvjIhndlxObKl3PHNct2FGapJUwGQFi3Kb98qtNWXXZTPpcxzVu3+tsqaHCR/ph1oMWqNHWD1XbFGuU9o+HpPQE3QHgOrLiJEyAW+Hyslk9TDg5d6tdm6emfbZ2MTH+kfvUV+m/Slnzdi0RFnwdQdc8seOaBb1i2bSjRgVK/nfyHikO5ek+6Xn+p11UIpWTElRCHn3HlBN3lQzf2cds6/78FIUQVHvnzX2/qv8s2ITk9tjsHvJl4bEgsUD258WmaYkyvz5lxvg1nCZzQDgxMkXTuq+LbUw6Rb4vcp24666q9PkSF86Qzc7XL4mFcvwaLHSiV+ZHDYpQTYsWjxxY43u5t4CbgBfqo5zRO++c1/9DxOTR8f2xD6LV0/rTxqxVdNSmPRlxoeFphKL59OxCUy6czx+VJsdLgRTt8CM/XdQzF1N2hzByXon3wCfzw2KmZ7UKbnHKeq104ZXhsYy6cuP7rR67tmv2lrv+GNK8uvD445fnfHluMTbsiLAlB0aLe6A7nxfZllaYPy8uLW24X/ubrc9BYozIkaicuFMuicBxaDY6vl+wuXbpRIj5mvdAXs0+SZsUrzsr2kpS0fFf1tmuW5nHagMs893t8esr0qXC7fNSuuk7gB6N7GsxOwhO1jxnzFhq2tsP5VbzB62jvjvNqsHVKDaji+fnAz1DJPl47syS/9I0ZhYKZNuG/cfVIO1nCoTaty4hM/9vLk2I62bmLW15tS8TCbdBk4bsb9qbN+Wmg/MTU8Lu+A8ewIpv5dJ+Vybl/xlckonC8O6WvtOldNNUNFi3sQEGVigzI6eDVgoz5/UHZybzqQ7x4OH1BhB3ZwZMct3+WBRflJk+mBUAp8HumMcECl+ZmA0fPoP7jz3HVCPjJH8u28kk25Cld2bIb/4rTthcD9zXGfyELkKkULIL7Ji22f1YvaxC5Ce4HPtjtpJG6s1LrA6A8P8HbX5Jjds1Du9/VaV+zObsmB33UL69SKZdKvcva9+xN+Vzx7XVto8TFYXgLfpXJoH/qs2EPfwpZO6YWsrPy40fldqfjffMHebcvrm6nfyDMzuc5wy0Hf4IuAESq0Yk2gZqKL/uauOSbSMGSMKzZjB3da7UmTGUn8rZRKB4McyM5wqk6CoD84aw34uyvqjbG2jzEABPwQvJJNoArzJMb+UMIlG3LCzdlmJyb99XO/q81eLb3sPJ9hWD1iY1++sc+Dkn9NSokR0K2lgWV9r/7rU0krbx1PHtPs0rsVDY2ennK/Ya534x4WmJSPimHSweOCgGlzLQDVVdIy1Sju4Emunp0aLzz+OnWqn2oUvyIxg0hzOYb3r6WO6r8Yl9j030rLAjP1SaQUr9aUhsQ/0abHq9tN3VcWHoxMa3/NmuWVPfbnNA/Yp1OrhAl6cRKAQ8eQCnlzIi5fw4YWZliSbknDevoN3l/dDkXlBHziMyQoQxw3uz4pNezWu27IiwLaaEC99Y3g7Xg+4XZvqHHYvyecCdLtGvFSwqEmzdP/VlfflKMCt26Zy/DgpCYx98AbqnHiYgAf/UenwHp+XIeJd0Pgwe6vy1WFxw2PEH541gTK+MjTunpxuHgfXMYIqPXacvGFnHUFxVk1PgfeJyQ0cv1fZnjiq+WJc4lWpciarOf6str12Rg9e/YtDYuGFhvLz5hnD7dkRTw+MYY4ICk8f16pdRLODX+HF5XK4jRu2VS78k0IT2Ni3Zwf4Pfu0yFRk8YAWxzSSnmZZWmD8qND01vC4nAjRslLzbrXz1qyIO7MV6U2cgovQuYkx66sqrr94CEzrmD2ExkVYvSS8NuBUat24ESPgHCqvz5Y1enmy/ixfNS11SHTA/CADRiw+pYeXZFH/qKcGxPC5HIuHvGFXHbi0/x3Upjdkc73jjTOGOSlhoJXw30F6cJIDp3xfDi3QR/XuXWpnnhnLM2FwZ/pHCm/NUoCLlyQVQBUIyvLDxCS45CX5Bqii4YDXh10gLo8e0eSE0/cfXuBH+kWxeMy9z/YJMGBJrlNebKA6cfKKzTWzt9bABpPVTqrtns119o/OGu/br2KyGvFHlTX5t9Kcv8pnbK5ZfEoHdjuzozngFF44oU3+tXTChmo4pV1qB7Ojo3xTYma22gZ4N+BytnQrZm2peeOMnklQ1Nt5+sRfS8H1A0+EyQoojxxWRywvvmd//W+VUNJbezprlTa4yYoVxXBKrR/ZGHDKsv8sYxIdAl6n63fWDl1bubzcwmSdA27jxlo7kwgE9+5XPXNMe0zvYtI+wAAZtKZiRcXFv94sfyttS/LOP77G3LanbvLG6hdP6lZVW+F93lZvn7+jltnno+EnwAWGczhrxi46k/sPqOC/HNA6mTRr4S9evJgRocDxV40N1HpiI8MYmLZZWWL1LMhSTL0wvxXKbJ7TJmy7yvFZsRkK3g/l1gq7l8fljoqVDI2+uKu7f6QYqqk7shUDIsWlNu+/D6kVQv7IFnrEwYa1eMm9WheYfGCFZYWLhjX5wnZx8576yQmyxLaNbQPr+vGj2l8mJ6fKmj9+SqJspc+X0bjxBw+pwfwGU+7mzAhpF5iKwJwUOVTIULf/XWv/zzEt2P9QXTdtVgfz8LkTuhszwuFerVM6oJbOVbTJ1jhjxMAgnZYYBk4cvANHDW6o3rPD21RdgwXx+BHt+jr7gkzFl+MSB0Vd/IvgMGbIhYOb5HeYPhEiuANJMkFjay5CyOsVJvxfgRFsognxl3iB4RtaOubJY9ojV2fMSAqDW6cQ8eHFg6c8Jk7aYHL6L3C3xrlH43xhMD10K7nRSwIlAqzUbbN69cBOj/bSJQ4XmOU1Du//Rp4f2j9obWW51fPm8PjH+rdjFNa9B1RGjEwLEwyJEkNp7N22l9UPGMzvnzXum9N838fLp/Qb6+yvDYu7MjkMHvM3pZZym+fu3gq/SdwBBq2p/GhMwrQ2DO3zkNTIdVXPD475Z8b5lpSmgId14866w3r3nb0VX49v9yBvsOor7J4RMZJMuQhs/rYDrs1XJeZvSs1j4+jWjYaBwm/mGeCWvjMi7ookur1mXa0dvNRre8kv6aU+eVS7Q+0stmDj42VwJiCjsRI+yPRtWRdfPngZO1VO+ITKAFA5cXhGFTYvFNT56fKWnOj7DqhBdx4Nyug+0GUnTnWmbW6/1jUhvk29t6eNWLNe5IwtyikJ0heHsH5AUJdID7y+UzfX3NNbsTA3CvzzkeurbV5i68y0pqZKwHET1O9V1t+rbWVWz/ujE5p2EsOb/dAhDZSB90fFRzZq596rca6vdbzdzpZmrZsotGAunPqo0AjfBjJxyW7pZ4/rnAT50ejWXt9vSy0vn9LBty3IjHg7zwD3E1SgXd26oKdfl5gr7V4wNKD2zo0Qt7fAvHJaD0KwazbdcVtk8dyxr37N9AumSsE3Lzqi6asQv9qGcXGD11ZunJGW0oKV52fI2kqwLGQCrpDHPWvxFJiwgZFisAIkfG60mP9mC628TxzVRol4QSuK8D43bo8PPuBPgDP+1oh4abuqlJ5HVzUzQ5lcsKcuQSLYrqKd0kNXZWRdOH4ngIBNDjUk2KJnzR6oJ8H0uD49/N4W7Je38gxmDxmozqzb99Y7cEoq4CodeJXd83Bu1CWtgLiVpZtmpoFE6tw4nAlYAeDCMPt8gK1XbPGA1jR05XxRbF6Sb1gxOXlcXPuGO/kB4fC5Ce34v3ACW+odTx3TYrf3heQOlRP8vuL5Wf69DcBVzN9Z++mYxEs+XPjvo2KkbemL2VTneO2MPlchem5Q7EVjvprlpVN6D0G1t85AdDtd2MMFr+/I9VUOnLwzK/LhfpFdtHgSWDH37lcly4SpMgEUgKmJsq7os28LmX+Wr25DV8uNu+r0GAFVFlSeYChZoNxwOA1T5Odtrx0YJX6rSQ2/XeWQ8nnj2yMfbeF/BcYKmyc7XAQiYvIQUGGA41lq9Yh53MmJMnAJ/5HGuDlOnJ5P69/uAPAy/Oug+vsJSa2L1OJT+t+qrK8MjbtIjlsBPEGtC/+gVSsS0QPpQunJ/qtC68a/GZ8IxsiqGhufS/cWD44WQ2UewCGhPYcfyi13tr/n20NSsStLrbf08SefP6EDt7TtBa/zfFNqVrkIAZcjF/JACnuFCXIiRF0xF/zTIlOcRHBTy5f23Amdxo2/PTzePy22jSwtMILB2+z4dURPpquk5+njuv/lG7bMSpvha5UEzpiwwzpXvhkbFi1pOjHvsoVuRt1S094xLyHJe2eNCzIj2qt6oGhH9e7v0dqAbKNLpGd9rf3q7bULcyM/GYPqokvw0il6AMhrw1BTRQf5ttSypd6xckrzi7qBKlXZvSSHAhcSHMYwAQ+kLUkmYHsbbQgQeOk5onfP3aZ8eUgsWs2kLaT9XrZrdnpb2lMRzdKK9OjcxKC1ldMSZUIe10tSDpzECErtwvUYIeJxwa2LFfOjxPxIIT9cSM/VAD2SCrgSHk/M58IBAh6Hz+WCRglg2/fJfG83gZMUTnEa5rrDFZEUBbKK+4bI+nYxhRn+gSRk+lJtAi7Of7Hw6dv2JX13AO4e3A0hjwMbAi59W4Rcrv8W+e4SfQAoO+RI2iPoAZYeO05O3Fh9c0bEs20bco4we4jGffyI9tK61fNTuaXZqScWDz0zQ+smjBhh8dITNWxewkVQTpzCCBIj6SINZRtKNUFyCLqEU/7RRi3R+lLMASlloAJQzhsKt18Z/ZroVwRI+nc16EjbgROESwDxgsv0bdMboF1w7X5dgzvgEzu/0tGfHsj33RZ6m6CTcNNkAi6YlvAHG1I+DzQ9UsSLFvNB6O/Lgc3z5xRg6bl7v0ou4H08BnU3IIIESM/mevuvUy7TxdJ6FCBDLoIEBxdMEIeXNjNtOAmVqwEjtC7i3hxF40HYgZQe+I1hf1ctn5Qc8D5gBKIlwK5ZVWP/63Jdp5G9BHJOEDgOlddnI91BBBPwLMBNYBII9tAl0xERiKDB5dKr9iBYB5IeBALRDSDpQSAQ3QCSHgS7oShOox5nBGvoQdJzwuD+pdLKJBCItkFQVLsGsCB6CD1Feg7rXfN21J4yYkwagWgbOMXpIdEiEe2iR0hPocVzx17Von5RwY8JgQgBkPKwke6XHouHvGe/6saM8CAHhEAgEN1It0nPE0e11+6ohY0Fe+r6KUSvo6nbiB6Di6Cq7edDHiO6gu6Rnj+rbfu1zt+mpty0u07C530bolHDwaDLN6PWK5Zhx8n+qyvuOaBaV2tnshBdQLClB57r8yd0L5/SPzUg5oGDaquHDkPK7AsEtU784cMasKfuO6A+oHUxud3ElnrH7XtVs7cqf61CPXddRcDbeeQC3prpqYMixVoXwWQhuoBgSw88VwMdVRL/zzHNIa1LLuRf43O7AsWDB9WZcuGDuVFDo8VXbKkptniYHd3BjRnhJ+dlwMk8fUxX58SZXESPR+vGwTC/tUm4HkQA6QaHK1LEE/C4tS4iQSqYlxa2R+NkdgSCe3MUTw6IFnK5y0rMs5LDEqTdvBSO2oUfN7jT5cLW48AgOkNgDZ9XT+ufPa5bMiJejMYLdSXdID3fllqtXvLT0QmbZqbBz1+bFsgl0K/tRX8bKM7YOOkJgxucL39+xyi3eRfsqR/6d+XY9dVQDTK5bWbxKf2wv6u8JLVmOlrSoasIeM86SXHGxUkNGPK2upYuWZu5FZYWGF84qYsQ8kU8enU1J07mX5PVrggEbWG3xllo9hRZsDMm7LYsRVvCPzXL/QfVw6Il0xJlZTbPu/nG3b54eG1kv9Y1d5sSpzjpYYKXh8a2HmsU0WF+KKdXKVx+LpoQgi0E1er5ptT89HHtmumpmn/2rrqh948Tk4ZGSwKuO8CHZ015JixFJny8f3SHdQcYHSsZGSPJVYh6h4ss3vZVgxPipZZb+tTckP3DxORrAmrZIS4C+UVsJHjSs7rGdt8B9YrJybN8oYHBjx4XL209YN4BrevbUguTaA9/TUv5dGzCfwZGzzsXwa5j3JcTOSqWjly4otI6+Vws0HYRI+bDN7RruWxEuyDI82sSd5hXT+sf6YRv/nuV7eNCU8GlBlJ8VGiKXVla1K1dHz2HYEgPPJK9Guete1WfjElo7HcIuNx3RsQzieb4u9YOf/BcmXSXoXMTP5VbluQbmPSFfFZs2lRnX9yGqN7Pn9D9I6AddohLQnLaPX301yqrHT+/jvt/jmnhFW0ppvslWVVjW1pgXFllHbu+GmQFfHxmRyM21jmmbqo5qndtn9ULjGgm9/ImwNKzU+2U/lz83lkjk+ZwXjipu++A5o59qqcHRi/MbV94HBdOTkqQNg7FuazEXGa7oNKotntv31v/xpnmVaMVfqm0Lj6lX7CnfsS6qtHrq3ZpnGObi2j+br7xxzLrdxOSmgb5B6Os4Xf3a13wbsELDWadPwcRHEBDBO0MU3NQ6xq1rgokA7b/dUBt9ZK/TkkJF3awLMzvFQ4m9kejE65PDwdxuWe/qrH5g1PUY0c08PevPpE/TUq+ZFzsy4cAS8+0RNn6K9J+rbTetU/lISnwsMptXi9J/iNN/nIbrIaLoGNr8C84Q42beDvvvK6BOzZmQ/XAKPHzg9s9/wsqKDjDu3orfpyYVHl99jfjk6Y0cakWHdHsVDt+n5rcbKTmnAgRWHMLD2nA2L5hVx28Wx+OTpB3IjA5ogN0wNn6YHTC2yPiFx3RDl1bBYrz5bjOBqocESOBP4yk4iSCmzMjrttZV2qlK8jdGufIdVVOgjpyVQYaJXQRXdLDBUoPlcmmOsfMZJnZQ8LT7VgHxJ37VLNTwhZkXvDMHj6sOW5wvzI0dkOt/ZDO/f7o+HHNWSudpMbhBec/VSaECo3JaoGBayr0bnLDjNThMXSrECLIfFlihvfhq3bKB7jYc7Ypiy2eX6YkX53aqQZBP2Dv37irrvy6bIWI90WxGYz9ualhf1bb3xsV/0CfSOYgRCPaKj2vndaDTwEb/SLF/RUiqOH9+S1x937VKSNW68RTZYJjV2e0yxsHxamye+F/FFmwFJkgXS4Ci6mxpfpxofG5k/okieD3aclDogJf4MEUf+a47v4+kZMTZBFCHtgxXF/lmnVhjFC1CwfjLlbCT5TxC83er8cntjdeOKLzgA9+tJ3So3UTV29XzkmR5ypE4FCfmJfB7GgDKhc+dG1lpIgPL2SsmB8u5C8ZEXfGhF23sxbe0oZwg1dsVu7TOp/oH/0WWgemBdoqPT+VW0R8Oq6g1UNuUzmeHBDdrA/i59EjGqhVxsZJnz+hjRbzf5+aMia2HYZJtd0LbhqU9ZdO6q5JCx8cLfZ3ivk5onffua/+xowIuYD7ebF5bor8jt4R7fr+SwIXu6HOUe/EDRjhwEkRj46HC+rz1IDoBrPZfxo3ZUSA/QXJN/MMYOV9PyHpInlCdDVgYpwyur9oj/TM3qocHSd91ffgoI4Ex/m59gTLteOkxkWUWD3wbkBxyAwX/uuA6vH+TFOm0uGFurN3hGhRv6gnjmp7h4vAMG8cdRPBANITWL4pMY9bX7Wq2sb5vnB1jQ2Sib+Wrq2xMbvbw9XblJvr7EziHP1WlX9RbPJvmzD8g7PGseurVlRY/DnBociMwUV9XsSchp+PzhonbqjC6cDXiODxaZHxoYNqJtEG4I26aVctk6CoQjMW+0tJpc3DpNvJshKT/Ofi5eXnX78rNtdAlckkKOrJo5oRf1f+VW1l0ohz8BcvXsyIUIB4+rjujmzFU8e0rw+PuzNbMSxG0k8heuCQem6qvL2jB78rs1yRJEuXn7cjQMv0GAnOsz9OuYTPA9vq9izFoChJMOuVT4tNUxNlj/a7oMNuTJxUxOclywRgGzJZiK7nkM5t9hLgPTHpS5EdLro6LVx47nUBf5mgOF+VmK9MCZO1/8Gtq7Uf0Loq7J4qu9dFUOCDb653LBuf1NDpBgZ7Wphwt8bZ2HJHAIFvZgYLdq/GNTc17KPR5xtoy2wesDyZRJsBofHPyWrMb1W2mxp1t3cLnxSZThmxr8d3tmcE0XneO2usc+BLR7U2QOySfFRoGhMn6bDbDnKzQ+U8bXQf1ruTpPw3h8c1fW8RFxF46Vl4SFNowXZc2Y7pTghEh1mSbzB7yLc6OiAwsIABpXR4MxrZ6YiWCLBrAObAhjr79xNDc9VBRA8EJzkN3lO3w+dykO60kUBKz3GD+5HDms/GJvYKQ3cfESQwkkJT5NhIIKXn0SOa14fFzUlBzWmI4OHESRmSHhYSMOn5ptScHibswIQGBKIzuHBKiroUWUjAntm9OZFo5iSiKThFeUgKPhv+Atuv4SKQ1cNKumQOF6K7wAjK6iUxkvIQlM1LUhzKgVNQOHGSA0knQUJWAw1PXsLnyoU8hYgXJeJHCHlNxyURPvkwe0j4EjtO6t0EfJo9hBOnwN+BT0g6cNLuJQmKA78CG3Ck/2A3ZDUhUsSPEsEv8hVCXriQB79Ofwp4/labxkLSMDvUf7apYcI4CX9CvDRJKoAvhsNv2VM/v1d44+UNEKwASU8PBawDf+nVuenJHFo34aJLO2nxkrDhL9Kw10VQFg8B+Ub6k4CcCCEfCrCIxw0TcPlcrkzAlfLpdfhhAzSlcV9Qw5OHLwGxsHgJIwaaQjm85PnFbHwIuBwxyJOAFyXmg4kRKxHAl8eI+fDN/q+VCUA44Cd4Qt/vwgZISThk+gQFfqexmngpWsXgt+Bs4ZxBK2mpwumLBbVsOJJ74Zx0eFEhB86twIwVWz1w+SCp669IW1pgvCdHEZApoIhggqSnI4AcRIv5xwwuE0aXWPgEdQCDAgoDWBlgIEARghwXFGMwCggSjBHI8V5UoBtV6X7gMDge/qAQQtGCAgw2iG+OIi9WwocSDjYCWApS32Q6KPNwAJ0p4kWKeCAECiG/K1ab7eHM2KJ8aUhMx9aQRHQjSHpaBPSl0IJV2r21DrzG4YWkyoVD0uAmRHxutIiu2EGAQAug5IME+EwDuvIHi8NX+dOZUp9RAGYI5FxyDiEcBgfD14KsgPGCWjDawrC/q36elNTKZGZEzwRJDw3YKYVmT74ZK7d5KmzeMpvHNy+Z6qcQZfpCaPWSC+PE/GSZIEMuihGDlXHZGRc9lvQ/yo9enRF/+Zl7bCdkpYegwH+h3R+MpFzg+xCUv3XA7CGdvoZSjRsHc0bp9JZZvWDU9IkQ9Y8U9w4XZoWLssOFuQoRGhjJCiJWlBgX5NCLmiBYBWukx0a3g9KtkhZfP4vOTS+mY/TQObABThDshXwjRvjbVkBowL+R8WlnB/6kPq8nWsQX+5yaGDE/SSZIkgp6hQl6h4syw4VoRRU2Ak88Z1WF+qbeTBrBHgIvPXacNIEoYHSfi8VD95iA0QFCAE4NmBuQBGMEDsMpDt356x/34dsLCcgA1YBt+PT30YK14qC/kBTxuRFCutk1km5k4YPXEysWRIshhw+fdCOrr2MYXCFfnw7IDdNTiwhhqu3e2duUhddmMWkEe2iT9IApAS6JHowLjABXxd8bCp9+QwP0BTboT9oGoTVC4Wt/jfI1xMqFPCmfBzYF/PnbXP2hrOFDyOPyOHQ4AdgQ8+i+VD6X3oBvANWQ0VpD6wg95IRueUUjVhEXc1Dneu6EbidaJoGFNCM9BWbstBErsnoqbPQCSEoHDr5IolQQS1sWtKaAcSH3dcTAhu+TzvdbHLCBPJfOUOfEvywxr6iwlF2XzWQhWmZ1je2XSuuvU1BIe/ZxsfTM3AJSQw6JFucqxNnhwky5MF0uDMkALyoXDmZaz4nHVm7z/lBu+a7UfE9O5MLcKNRl0xa+KTWfMGCXjBqC6IGwppk5sLybb/yuzAyu3FMDYnarnZDTja/vGRP2Q5llVY3t7t6K+/pEorAWbeedfIMdp/wLvCPYxWXagDIyVnJjRgRBcR44qEoLE3SL7jxxVDtoTWX0L6VTNlWDP3tiXsaLQ2KR7rQLI0ZGi1AjICu5TB+bh6QO6VzhAt7oWOnGOgeTG0Tm76zdWu9w4uSiflGzkuWZ4UI0TLEDgNecJENizUouO+nRuYnHj2pfPKm7LycyJ0JUbvMEuVl8v9Z1+17V+lrHvTmKwvlZGeHCAjN2Gc69Cgj1dIxJNPKTlVxe0vNtqWXixmq5gLtvTvqNGeHgdm2e2StoXbO7Nc5b99b/64BqVKzEcHPOjOSwKZtqdqic742KbxruPVBU2b2vnta/d/Z8oPpQQu3CU5DVw04ul2bmMybsrTyD1Us+NyhmQnzgY7S3zk6186sSc74J+3dfuveKyfWFeD5ucOdfk8mkAw34I5M2Vj+UG7W6xv7JmITBUaE2xzJmZanmn73RLAo2EgrS80Wx+fdqa4WNDtN+U0bE202iXL+bb3w73/Di4JjH+kevqLDeci54cec5bcQ+LDTmmzEhjzsrOezlIRd3tYBRs6zUDC7VA30uEJ3g8NIpPUFSbwyP86+q1Ua2qRyvnza8OCTmiqR2L7N9QOtaXmHl8+jFwPpEiEbFSPp22fAFENapm2qK56OhzKyE9Q4XvH9flJieHxR7cG767tm9iizY+lq7f5fZQ/yttM/eqjxpdB+Ykw6688YZA2iQf2+72KNxgrQxiUbcvKduWLRk2bikD0YllFk9SwvO+zUgOjftrnvqmHZyguzMPzL9unNY7/LvDQ7b6h1Xp9FraLWiO08f1x7UnT+rN/MMzxzXPdIvqlndAd/t+RM6JtEcmeHCYTFiEB34xbVK2+xtyqF/V8IXOvEmixV1mnonjjoEWQxYPWznuN7l3/jorDHjjzLXubDnMzZXy38ufi/f6E8uydMPXF1Rbu1IdO0Bqys21l4c/R2A/Iao8LAxb7sSNnaoHDO31GT+Wf5+AfPTfr4qNqX+Vlpkxph01/PBWWPkipL5O2qXFhiq7c1f+Dcl5gcPqmBD68Jv2lV717562PDvagp81crK9oW3P6xzLTqsvm1PHZMOHOuUtsbR0xHsIvAx17uCLfWOWLGgpemgSTLBTrVz0RGN2kUsn5QcK+HD8XfuU/VViIdGSz4pNjoJaq/GtaLS+sfUlJyIjtj/7xQYwZkKazKqO0zIK7J4/Evk7dO6jhncG2rtv1Ta4iQCtQv/s9pmwIje4aIYMf/1M4Y/qm3LJ6UMCGKDy9g46bODYvg8bp4Je+CQ2o6T05vYMsNiJO+fNYE59mGhaUK87L1R8U0vs9zm/a7Msl/r+rnCEiUWeEiqjaPAf6m0vnRKJ+bzXh0WFy0OcC/ePo3L5iXnoqVR2Qk72noePaL5uNA0KlbS17eqzn8HnQ+5U+fE384zgMuwqF/U7dkKguI8d0K3qsYGSnGrr02n2OK594DqkM51dWr4Q7mR7Y26P2OLckK8FH59ZKy42o5vnZXW7Do+X5eaHz2siZcK4Nwe6BPpzwRn8PNi84eFxngxf2pS2MejE7pxMj2czH+P6yJEvMax8P2UWD2j1lX1VYh2z06XNneG4DyC9+QgqN8qrQ/2jboyJWxaYvNdcqBfoLnwTrkJarfGCX7WValhi/pFp3dBTM5386FSIZu2ryFYATusnjkpcqi9R8dKwaKx49T4c11UXxSbb9pdNzVR9tOkZDBwwKy4bW99okSwYnLymDjmmG/LzKdN2MaZqUIe97Ni8/IKK2wMarPpIeHzoBSBm3Z9RsS7I+PTmuiOxUNet7P2g0LzTRnhUHRHxkiYHRxOuJBX6/BuqHWCjaB0eFNkwg60uX5aZDqscx/R039QmOFaRsV2pIcOTubaXuGPHNbM7xWuuHD4Ii2sMZJEqeC1M3owIfs0MQwzw4WzU+TZ4UL4dbjVmS3ryFmzx0tRRoz4s8YGh8Evmj0k3PCuWMB0c71DIeKNO/egEeyCHdIDCHjcZJlgYKS4QXfyzdiTx7QrJ6dclSoHy+3xI1ow7+/NiXxlaGxDTLgCMwbGyJrpqWArQYm9u7cCzP69GicUJP8BlwTKDPxisdUzOErS9C0HY2fONqXdS62ckvz0wBj/iiJQyP17j+rd9xxQ/zktBWrm1DDhkjyDDiMmxrdvCM+qGrvJvyyJl155PlLEb6xuzbK0wAgnHE0vJMDYMHB/YKPG4QWXMFosuEgIVlZax8fLnhwQDceDCXlI7wL3tqlxB15bjQO/pldrYWfAfYPPd/KN741KeGt43KQEGThEXaE7ANi2mXLRsOhL3A1Ez4TdnesPH9bsVjtLbR4vQYn5PC6XAzUzmDygUP4DwExYVmL+eVJnYxOCXWDD6TFBTJrDOWFwv5lngNIoE/CgeveSlAEjtG78npzIhsN0buKhQ+rfpzJLOkASnMEPR8d39dpDB7Su78osJ4zuMqvHQ9JLr4FmCbjcKDFvemLY8snJFzlV62rtk+JlYEH4k3DHlpWavx6f1LFxQFM21TycGxWEwFi37q3/Z0bEP3xdeAjWwfpxPf89oVtTY1s8NBZqVymfF5y2lPfOGt84Y3h1aOzC3KiDOhfYF3qMiBHze84SHA34ny5IT3DuzKY6xw61450R8Uy6K5m7TfnC4NgGKxjBLlgsPeBMPXZEmy4XvjsyLipYcy+NGPHYUa3VQ7wxPK6L/Ai243fugkD/NZWP5EY92Jdp1Eewi661/LuO1TW2mVuUV6fJvx6fGDTd0bqJqZtr0sMEq6enIt1pieDoDmDxELWOZsZ5IlgBK6Xns2LT40e1X41PXNQvqFMT4iV8cLJeG3bxRA1Et0BQdMxFJoFgG+x7cm/lGX4qt66ZntotYbavbbV/BxFMSIpy4wSTQLANlknPm3mGHSrnH1NTQm8SNqK9kByO0xdPCcFG2CQ9S/INm+ocP01KQku0IAAexbF7Az8rFREc2CQ9I2IkO6/slYgmKyN8cLkgPcjqYStskp4ZSWHBGZyCYAU4RYeuZRIItsG+ZmYEwg+ojj92NoKNIOlBsBUuh54jwiQQbANJD4Kt8DjcLlj7EBEkkPQgWAlBcXg8LoHaelgLkp5uxuIhPy40TdxYvbrGxmQh2gC4WkIuLUAIloKkp9sotHiePa4buKaiyOJ5Y3gcGifdLtwEKeJxkfKwl8tdeuw4+cxxnQEL6nj8gzrXg4fU87YrZQLu/rnpn45N6LoQgKGK3UuKu3jZI0SXclk/vKUFxn6rKuAljgn0iuUtsV3luGVP/cJDmmiR4PNxiS8NiW12pWfEJTF5yDA+F2kPewmFEIAd4KNC06dFpuExksf6R43p0FLH7QVE58sSc7Xde19OpFTA+6TQFCniRYh4v01h1jBEtIvN9Y4leUYul9o+K0hxqxGB5fKSntv31pfavFD+JyVIF+ZGBcfN2a91fVxoKrF6Huwb+a9zwSoAm5fMXV1Rd2NvJo1oD58UmfZrnXo3uXVWGpOFYBWXkcX6e5XtkM5dZfPMSpaBrREE3SkwY/cfVN+2t35CvPTEvIzGugN8U2oej6IpdJQzJixJKjy37D2CfVwW0gN2xzU7at/KMyRJBdOSwtbVOn4qtzD7ugadm3jqmHbs+upUmaDo2qxHLlzSDKeoF0/qVtfY3w7KGsYhyT6NMzNcKOYh6WErIS49Zg+x6IhmzjblxHgZ2B3LJyfNS5UPj5Zo3V3YpbUk39BvdQVBcUquy3ppSKy4Sc18/wH1KSM2Nk56QOtksnoAKhf+WbGJSfR4nhscK+RyuzGkIqKThLL0LCsxD1hT6cCpgmugguSNXl91xRblGqXtpozwJwdEMwd1GvDjNtU5tqkcsA3G1JC1laeN2JaZae+Pigcjy39MA1C84fOLcYn/7hsZJ+GDOfbEUa1/V/cCVzF7q9LsYc3EhNuyImxeMuJcyDME6wjNZuYCM/biSX2l3fvykBj/UL3DepdcwAv4Wu6fF5u3qxxQAE4asBqHJzdS/OzAmHktRIZ6M8+woda+b046k+56QBNnp1w60DN4f9tUzteHxV7RJCJ7T+alU3onTv5vJHJaWUkIVhpLC4yD11b2VYhOzstoGCI8JlbaFTEkhkaLqxxeEY/rIMhx8bL+CrFfd8D8OW5w+4/x8+ppfZ4JWzUtlUl3iKeOaUHsmMSlAL/vu7LzB8/bXvtuvpFJnKPa7p2/s07tIjbOSGWX7gBWD9EQ6BXBOkLqyZ0yuudsA5fKvuPKXm8NZ+JGgNu1W9NVTSrgMeWbPFFi/tlrMz8YHb/vXNvNHo0LXJhaJ+1eeUjqjn2qOif+y+RkcLL8B3SMXyut1/Zq02L4cGKvnja8NCSWSXM4ExOkm+rthRYPk/YNNZq5VTkmVrJsfGJksAIKBRCLl1Qg6WEtbHpyM7coma3meO+sccS6qkgRb8/sXg0d58+d0P1QbsmUB37E8J/VtvEbqk8Y3IfnpoPMCbjc5RXW6YmM4bBkRJybIAesrrh+Vx2clZjH/XJcon9XB4Bv/qTI9PIpvdlLPnRIfe2O2iu21Fy5tbW78cJJ3dKR8Y0NvWcGxsxNkU/fXPNHNT1P9bsyy9xtta8MjX22UTRndmHCiAgh+xQT4YdNbT3hy0tst/ZhEhzOwkOaCrtHyOMOjZKcMbl1GPHm8LiHD2lWT0/NDqe15v6DaiNGfD8xSd7RyT5v5RmmJ8mgAPO5XOm5zpQah/f1M4bTRvfTA2OuT6cduiN69/tnjThJNYRX9wPuDAiEkM91eMkUmWBSgmxCvPSq9sfwuWe/CqySWAkfLLiHc6NGxkqiRPwYMb+l5fHh9OAkvxqX+G0p7fcNjhY/cG5I0fpa+3+OaROlgkq794eJSZPZPHds6qaaRf2j5qNpt+ykp1s9L57UKVaUDF5beeXWWhGP88ppPfzhFAXuDJSuh/pGpcqEb+YZwOjYPycdjJ05qWELD6kLzNh1O+sEXM4fU1M6rDuAi6AePazJ+asid1UF2BGQA4V5wgZ6tM7hqzL8ugPGyM2766AMX6Q7dpy8eU/9gqyIvH9kVlyf/d6ohASpYGWldf7OOuaINvPthKT3RsU/NyhmbJwU/uAyB0eJW9Id8PKW5BnSZIKsP8sP6lwjYiTgpjH7OBwQPvqUzFiEiOfE2d3DoHXj8RIUI4CtsMDqUblwUJl9Ghc4Hf7a2+8jfFxogir9lMkNRVHK5709gmncAY14O884KFL08+TkADYtmzwEuG+VNu+LQ2LBePFngg/YL1J0Z7YCZCVRygcF9OcDnxXTp/fN+CQmfY4quzejow7gvw+qr0wJa72e31TneOmUbmZS2B3Zir4KEdylQgv22VjG3dumcjx+RLtmeuoJoxsuB455YTBbHa6YlaWHr0rvHS5i0ghWwRqH67QRW3hY3dAzva7W/uRR7YyksFnJYS+e0i0bn+ifBQoG0awtyr4KcbyEv7zCAsbIXb0VnXcrtqsc/z2hm50if3Xo+YZb4H8FRtCXWofXgBHwFycRPNg3cmEuPXYZ5HKvxnVrVoT/yIAA/mN0OyfZT99cA0ZTg9gtLTCaPYQ/drPahb94Uk9yqI9HJ8jYtgCFm6CkPxeDA94ZqxbRjbCpreeLYvO/+9JWD9g1Xxabr0+XV9px8Ike7x81MkaS5lt94q59KoWI9+HoBNj2kNSP5ZYNtY6/pnVqdvjXpeZ3841vDo/ze1itoHR4I4R8OAEm3QOAG/L9xPOWF9wuvRv33ys/r57WnzJinbxFwafU6hm3oVp/cw6TRrANlg0ppBedOKAOF/LATbhrvwojKKiu/R2sq6alpsgEab+XTYiXrZyS7Ds8AEDJBONl6aj4EA61XGzxgGvGJFjCTrXziaPak/MymDSCbbBJen6usD50SP384JhnBgapeeKpY1oQO5YOewltlldYV1Ra11/RqSGaiG6ENdIDKvC30v7RmIQrk4M06NaOkw8cVH83IUnU3dOjCy0e8C8q7fRKQyoXDrYefLYrGIP/Avz/oeFiuByuVMAVcLmxEn6smJ8sE/QOF/WJEA2MajrjtcextMAIt+Xr8R0fLYXoXlggPSABd+xVgVf1xbjEqFC3PmqdeInFU+PwVti9ZVZPkcWTZ8KywoXZ4cJMuaiXXJAiE0aJeGCFtaV1FcSF2WoC7IAH7yJIL0np3ITeTSid8IveEqunwIyBAGXKhelyYa8wYTwIk4QPjq1cAL9L/6qUz4sW88KF/A4rFDzTOgeuduMmjHARFIhp41h+fB4H5B40ETxrmYAb5rtU/yT1aDHfPyn32eM6yHjj3Jh1BOtggfRct7Oud4TwnRBa2gYKHtgvoDK1Dm8dfDpx+FS78Cq7V8bn5kSI0sJAaIS9I0T9FKKBkeIgGyE4RZVavRU2T7UD7CzcgBE6N+7EKQdOmj30YiMgFkaMgKsAdZALeQohKBFtN8VI+JFCPuSATDScM07Cf6SsXsKEkXqMqHd6NW7C7iXTwgQJUkG0iA+Wl4TPE4BMnrtKnKS7COA/2rwk/IrbJ0ygkvCpdRMgf//MiDhrxsbEScH7Zv4Pgm2wQHrmblNumMHWRTCVPvsFNKXS5oWSXOvAK+0es4dMDaPtlxSZAOrwVJkgNUyYJOVnyIXsalQCawWkweQhjBip9ZkwJg8JeoGRtCHjPwbMVbCYIoS0pRYn4SdKBODZdWYuG/hZy0rMP5ZbxsVJ/0ZtPayFTc3MPR9wlArMnnwTVmbzVNi8RRZMKuClh9GeC1gxoCxQ1cNG475tRMfov7ri+4nJo2MlTBrBNpD0dJxSq6cY/nxtwGU2b7FPaHIVogGR4pxwETiJ/RTiTk5VR7RExIqS4vlZTRdjQ7AFJD2Xxk1Q5T4rhm79tXnpnibfBjhK2eHCvgpx3wgkNEHF4iGjV5YQd+QyaQQLCTXpISimhRJvdF3+5svG1+nfCQfbvKSLIJ045SRIE0ZA0uyhGy+0bkLjwjVuQu2iG4Czw0XgLqWHCbLCRVl0Z5MQctDCwN1FgRm7antt1fXZTBrBQtgtPcsrrGuUNiNGWr10p4kDp7wkJeJzBVwOj8slfZcG+gL/ECTl3/Bv+/87n8eVC7gyAU/Kpz8jRfxIEd1fAxsJUkGSlP5MlgrSu2C5H0Rn2FzveP20fm8Ql5pFBBx2S88ZE6Z141G0ZPAjhLxwX7cusw8RunxXZtlUZ/8VBW5lM6itB8E+luQblA78kzH0JGEES+lBc6wRiDaicxPxqEWf5SDpQbAPLS09qFud3SDpQbAPrQtPkCKrh90g6UGwDx2GrB7Wg6QHwT4M7V8oFtHTQNKDYB86NxGLpIflIOlBsAyLh/QQFJqzwnaQ9CBYhtaNJ6I2ZvaDpAfBMrRuOugQk0CwFiQ9iHZj85Lzd9atqLDu17qKLR6lw2vHSWZf16On450hq4f1oIkUIcuLJ3X+UH8d4808w3O+KK/N8m2pZafaUefEdW4CIykTRuAUJ1JET8SV8HmfjEkYfy5Aa8D5qdyyrhZN4GI9SHpCkwIz9uAhzZ7ZvZh0E3wDgluzHSJWlFhv6cMkmgMsHXh3xHyuP2LHdpXjg7MmUKK7cxT++NRdxGfFppMGbBmKRcFykMMVmgyIpEM/T9lU82e1jck6x5Z6x+ytynfzDUy6Q4DpEb68BORJ/FNxzMrSxN9Kb9hVL+FzXx4a26W6A1g9ZIQ/6iOCzaBHGLL8MTXlX30il+QbrttZd9zghpwzJuz+g+r/ntDdlq14Z2TzET6cOIlT9EJrYQKe1QtuVPNG8YzkMNdtffE7cldMTlYIeTOS5O+OiMsOF31ebKq2e5mDugarl4xCg3rYD3K4Qp+lBcYlecZEGV/vJp4YEP3UgGhmR3MM/7uq0IIJeVwnQcr4dKStW7MiWlqe4vUzhhUVlqWjEuakBCkuI7DwkCZXIXqkXxSTRrATZPWEPm6CMnhwCZ+XIuNfMoTDiXkZYM5Yb+lzdYp844xU04KclnTnP8e0R/SuXbPTg6k7gMVLh+JiEgjWgh5hKHNY7xqzvuqsBSu4JuvIVelPDIi5fa/ql0ors7tVosV8A0YH/GuWd/ONJVbPqmmpwV83x+Ih2RWtDNEsSHpCmT+qbLdmKZZPSgYPBZILMiN+m5q8+JS+wIz5D2iFJwdE/yNNziSasPSs8eMxCd2yGq3Zg+aOhgJIekKZ14bFPXphm8iYWCkIUK82xCAcEClmtpqgdHilfG5bvqQrMHtIJD0hAGpmRrCMtN/Ljs/LRAuksh1k9SBYBlg9CjSuh/2gR4hgE06c5PPoIdRMGsFakPQg2ITFS0ah7q2QAEkPgk0YMUKBBvWEBOgpItiE1UsqhMjqCQWQ9CDYBEgPmjsaGqCniGATTpwME6CXNhRATxHBJuxeUiZA3VuhAJIeBJtADlfIgJ4igk1YvGjuaIiApAfBJmy09KCXNhRATxHBJhyomTlUQE8RwSbsXlKO2npCAvQUEWzCRdCLRjMJBJtBTxHBJnzjelDneiiApAfBJpw4hRyu0AA9RQSbcBOklI9e2lAAPUUEm8BICo1mDg2Q9CDYhJugkNUTGqCniGATGC09yOoJBZD0INiEh6RESHpCAiQ9CDaBk5QESU9IgKQHwRooDofkcARcJD2hAJIeBALRDSDpQbAJ9L6GDOhRIlgDSXF4yNsKFZD0IFgDRpAo+F/IgKQHgUB0A0h6EKzBgaPxhKEDkh4Ea/CFHkULM4cIXIqimE0EAoEIFsjqQSAQ3QCSHgQC0Q0g6UEgEN0Akh4EAhF0OJz/AxKGyOgUlHjhAAAAAElFTkSuQmCC)
	Il risultato è quindi $\underbrace{x^4-3x^3+4x^2-5x+7}_f=\space\underbrace{(x^2-x+2)}_g\underbrace{(x^2-2x)}_q\space+\underbrace{(-x+7)}_r$
1. Il metodo di Ruffini:
   Il metodo di Ruffini è fattibile solo nel caso in cui $g$ assume la forma di $g=x-\alpha$
   Per esempio $f=-3x^4+2x+6\qquad g=x-1$
   Si mette in colonna con la forma:
	   
	
	|     | $-3$ | $0$  | $0$  | $2$  | $6$  |
	| --- | ---- | ---- | ---- | ---- | ---- |
	| $1$ |      | $-3$ | $-3$ | $-3$ | $-1$ |
	|     | $-3$ | $-3$ | $-3$ | $-1$ | $5$  |
	Quindi il risultato è:
	$f=g\cdot (risultato)+resto$ che in questo caso è:
	 $-3x^4+2x+6 = (x-1)\cdot(-3x^3-3x^2-3x-1)+5$
	 
	Passaggi:
Si mettono in colonna:
 Nella prima riga i coefficienti delle $x$ quindi avendo:
$f=a_4x^4+a_3x^3+a_2x^2+a_1x+a_0\qquad g=x-\alpha$
La colonna sarà:

|           | $a_4$                  | $a_3$                | $a_2$                | $a_1$                | $a_0$                |
| --------- | ---------------------- | -------------------- | -------------------- | -------------------- | -------------------- |
| $-\alpha$ |                        | $r_4\cdot-\alpha$    | $r_3\cdot-\alpha$    | $r_2\cdot-\alpha$    | $r_1\cdot-\alpha$    |
|           | $a_4\cdot -\alpha=r_4$ | $\uparrow + a_3=r_3$ | $\uparrow + a_2=r_2$ | $\uparrow + a_1=r_1$ | $\uparrow + a_0=r_0$ |


Quindi seguendo il teorema di ruffini la divisione tra due polinomi esiste solo se esiste una $q$ che moltiplicata a $g$ mi fa $f$

$f,g\in K[x], \frac{g}{f} \Longleftrightarrow \exists q\in K[x]: f=q\cdot g$

## Radice di $f$ (o zeri) 
Avendo $f\in K[x],a\in K$
$a$ si dice una radice (o zero) di $f$, se $f(a)=0$

Seguendo il teorema di Ruffini:
$f(\alpha)=0 \Longleftrightarrow x-\alpha|f(x)$

> [!info] Definizione: Molteplicità di uno zero
> Sia $f\in K[x]$ un polinomio. E $a \in K$
> Definiamo la molteplicità dello zero come:
> 
> $m_f(a)=max\{r\geq0:(x-\alpha)^r|f(x)\}$

