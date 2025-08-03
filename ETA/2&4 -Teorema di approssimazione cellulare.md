Una mappa $f:X\to Y$ tra [[2-Complessi CW|complessi CW]] è cellulare se per ogni $n\in\N$ $f(X^n)\subseteq Y^n$.

Il teorema di approssimazione cellulare afferma che ogni mappa tra CW-complessi $f:X\to Y$ è omotopa ad una mappa cellulare.
$\ul{dim}:$ Prima ricorsivamente che esistono delle omotopie $H^n:X\times I\to Y$ tali che 
- $H^0_0=f$
- $H^{n-1}_1=H^n_0$ per $n\geq 1$
- $H^n_1(X^i)\subseteq Y^i$ per ogni $i\leq n$
- $H^n$ è costante su $X^{n-1}$
Trovate delle tali omotopie è questione concatenarle in $$H(x,t)=\begin{cases}
H^i(x,2^{i+1}(t-(1-2^{-i}))) & t\in [1-2^{-i},1-2^{-i-1}]\\
H^i(x,1) &t=1,\ x\in X^i
\end{cases}$$dove sappiamo che la mappa è ben definita per la seconda e quarta proprietà che chiediamo alle omotopie, mentre per la prima e la terza proprietà vediamo che $H$ è effettivamente una omotopia da $f$ ad una mappa cellulare.

$n=0$) Per ogni punto $x_0\in X^0$ fissiamo $y_0\in Y^0$ nella stessa ccpa di $f(x_0)$ e un cammino $\gamma_0$ da $f(x_0)$ a $y_0$. Grazie a questi cammini definiamo una omotopia da $f|_{X^0}$ alla mappa che manda $x_0$ in $y_0$.
Poiché l'[[2&4 -Inclusione di scheletri è cofibrazione|inclusione di scheletri]] $X^0\subseteq X$ è una cofibrazione, possiamo estendere l'omotopia a $X$ ponendo come dato iniziale $f:X\to Y$. Questo definisce $H^0$ omotopia da $f$ a $\wt f$ tale che $\wt f(X^0)\subseteq Y^0$. Le altre proprietà richieste sono vacuamente rispettate.

$n>0$) Senza perdita di generalità supponiamo $f(X^i)\subseteq Y^i$ per ogni $i<n$ (partiamo da $H^{n-1}_1$). Sia $$\vp_\al:(D^n_\al,S^{n-1}_\al)\to (X^n,X^{n-1})$$una [[2-Incollamento di n-celle|mappa di incollamento]]. Per quanto detto $f\circ \vp_\al:(D^n_\al,S^{n-1}_\al)\to (Y,Y^{n-1})\subseteq (Y,Y^n)$. Ricordando che $(Y,Y^n)$ è una coppia [[2&4 -inclusione di scheletri è n-connessa|n-connessa]], la mappa $f\circ \vp_\al$ rappresenta un elemento banale di $\pi_n(Y,Y^n)$, quindi per la [[4-Annullamento in gruppi di omotopia relativi|caratterizzazione della banalità in omotopia]] si ha che $f\circ \vp_\al$ è omotopa ad una mappa $(D^n_\al,S^{n-1}_\al)\to (Y^n,Y^{n-1})$ tramite una omotopia che non dipende dal tempo su $S^{n-1}_\al$.
Considerando ora l'unione su tutte le $n$-celle troviamo una omotopia $\wt H$ tra $f|_{X^n}$ ed una mappa $X^n\to Y^n$ tale che $\wt H|_{X^{n-1}}$ non dipende dal tempo.
[[2&4 -Inclusione di scheletri è cofibrazione|Ricordando]] ora che l'inclusione $X^n\subseteq X$ è una cofibrazione, possiamo estendere $\wt H$ con dato iniziale $f$ per trovare $H^n$ omotopia costante su $X^{n-1}$ da $f$ ad una mappa $H^n_1$ che manda gli scheletri negli scheletri corrispondenti fino alla dimensione $n$. 