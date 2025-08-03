Dato un [[2-Complessi CW|complesso CW]]  finito $(X,K)$, la sua caratteristica di Eulero è $$\chi(K)=\sum_{n\in\N}(-1)^n\rnk C_n(K).$$Mostriamo che in realtà questo è un invariante topologico che non dipende dagli scheletri scelti. Più precisamente mostriamo che$$\chi(K)=\sum_{i\in\N}(-1)^i\rnk H_i(X).$$$\ul{dim}:$ Per l'isomorfismo tra [[2-Complesso cellulare|omologia singolare e cellulare]] sostituiamo $H_i(X)$ con $H_i(K)$ nella tesi. 
Procediamo per induzione su $n$ massimo indice tale che $C_n(K)\neq 0$.
$n=0$) Ovvio in quanto $\chi(K)=\#\text{c.c.p.a.}$ in questo caso.
$n>0$) Consideriamo le successioni$$\begin{gather}0\to H_n(K)\to C_n(K)\to B_{n-1}(K)\to 0\\0\to B_{n-1}(K)\to Z_{n-1}(K)\to H_{n-1}(K)\to 0\end{gather}$$e notiamo che sono esatte: la seconda è esatta per definizione di omologia. Poiché $n$ è la dimensione del complesso, $B_n(K)=0$, quindi $H_n(K)=Z_n(K)$ e l'esattezza della prima successione segue dal teorema di isomorfismo.
Consideriamo ora il complesso $C'$ che otteniamo da $C=C_\bullet(K)$ eliminando il gruppo in grado $n$.$$\begin{align}
\chi(K)=&\sum_{i=0}^n(-1)^i\rnk(C_i)=\sum_{i=0}^{n-1}(-1)^i\rnk C'_i + (-1)^n\rnk C_n=\\
=&\sum_{i=0}^{n-1}(-1)^i\rnk C_i' + (-1)^n(\rnk H_n(K)+\rnk B_{n-1}(K))=\\
=&\sum_{i=0}^{n-2}(-1)^i\rnk H_i +(-1)^{n-1}(\rnk Z_{n-1}(K)-\rnk B_{n-1}(K))+(-1)^n \rnk H_n=\\
=&\sum_{i=0}^{n}(-1)^i\rnk H_i
\end{align}$$dove abbiamo usato il fatto che $H_{n-1}(C')=Z_{n-1}$.