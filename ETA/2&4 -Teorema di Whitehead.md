Sia $f:X\to Y$ una mappa tra [[2-Complessi CW|complessi CW]] che induce un isomorfismo $f_\ast:\pi_i(X)\to\pi_i(Y)$ per ogni $i$, allora $f$ è una equivalenza omotopica.

$\ul{dim}:$ [[2&4 -Teorema di approssimazione cellulare|A meno di omotopia]] supponiamo $f$ cellulare. 
Osserviamo che possiamo fattorizzare $f$ in $r\circ j:X\to M_f\to Y$ attraverso una inclusione nel [[4-Mapping Cylinder|mapping cylinder]] e una retrazione. Per il [[2&4 -Mapping cylinder di mappa cellulare è complesso|lemma su mapping cylinder di mappe cellulari]] sappiamo che $j$ è cellulare. Poiché $r$ è una equivalenza omotopica possiamo limitarci a studiare $j_\ast:\pi_i(X)\to \pi_i(M_f)$. 
Quindi, senza perdita di generalità, sia $f$ una inclusione cellulare.

Considerando la [[4-Successione lunga in omotopia|successione della coppia]] $(Y,X)$ si ha che $\pi_i(Y,X)=0$ per ogni $i\in\N$ (*le mappe della succesione sono indotte dall'inclusione e queste inducono isomorfismi per ipotesi. L'annullamento segue per esattezza*).
Osserviamo che $id_Y:Y\to Y$ è una mappa cellulare che manda $X\subseteq Y$ in $X$, quindi [[2&4 -Costruzione di omotopie relative da CW|esiste una omotopia]] da $id_Y$ ad una mappa $Y\to X$ che ristretta a $X$ continua a comportarsi come $id$, cioè $X$ è un retratto per deformazione di $Y$ e quindi in particolare $X\simeq Y$.


Dal teorema di Whitehead segue immediatamente che se $X$ è uno spazio tale che $\pi_i(X)=0$ per ogni $i\in\N$ allora $X$ è omotopicamente equivalente ad un punto, cioè è contraibile.