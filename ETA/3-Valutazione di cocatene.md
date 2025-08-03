Consideriamo $C^\bullet(X)=Hom(C_\bullet(X),\Z)$ e per ogni $i$ definiamo $\ps{,}:C^i(X)\times C_i(X)\to \Z$ nel modo ovvio.
Pensiamo ora a $C^\bullet(X)$ come ad un complesso di catene con gradi negativi e definiamo$$\e:C^\bullet(X)\otimes C_\bullet(X)\to \Z[0]$$ponendo $\e_i=0$ per $i\neq 0$ e $\e_0=\oplus_{i\in \Z}\ps,:\bigoplus_{i\in \Z}C^i(X)\otimes C_i(X)\to \Z$. (passa tutto al tensore per linearità delle cocatene).

La mappa $\e$ è effettivamente un morfismo di catene
$\ul{dim}:$ Vogliamo mostrare che $d_n\e_n=\e_{n-1} d_n$. La mappa di bordo di $\Z[0]$ è la mappa nulla, quindi vogliamo semplicemente mostrare $\e_n d_{n+1}=0$. 
Se $n\neq 0$ la tesi è ovvia, quindi supponiamo $n=0$. 
$$\begin{align}
\e_0 d_1(\al\otimes c)=&\e_0(\delta\al\otimes c+(-1)^{-|\al|}\al\otimes \del c)=\\
=&\delta\al(c)+(-1)^{|\al|}\al(\del c)=\\
=&(-1)^{|\al|+1}\al\circ \del(c)+(-1)^{|\al|}\al(\del c)=0
\end{align}$$

Segue che $\e$ induce una mappa $H_\bullet(C^\bullet(X)\otimes C_\bullet(X))\to \Z[0]$, ma per [[3-Formula di Kunneth|Kunneth]] questa induce una mappa $H^\bullet(X)\otimes H_\bullet(X)\to \Z[0]$, in particolare $H^i(X)\otimes H_i(X)\to \Z$.