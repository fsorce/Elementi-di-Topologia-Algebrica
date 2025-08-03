Sia $X$ uno spazio topologico e $A\subseteq X$. Per $n\in\N$ definiamo il sottocomplesso delle ==catene di Eilenberg== come$$C_\bullet(X)\supseteq C^{(n,A)}_\bullet(X)=\ps{\sigma:\Delta^i\to X\mid \text{facce di dimensione minore di $n$ vanno in $A$}}_\Z$$Se $(X,A)$ è $(n-1)$-connessa allora l'inclusione $C_\bullet^{(n,A)}(X)\subseteq C_\bullet(X)$ è una equivalenza omotopica.
(intuitivamente costruisci l'inversa a meno di omotopia con [[2&4 -Teorema di approssimazione cellulare|approssimazione cellulare]]).

Sia $f:X\to Y$ una equivalenza omotopica debole, allora $f_\ast:H_i(X)\to H_i(Y)$ è un isomorfismo per ogni $i$.
$\ul{dim}:$ A meno di sostituire $Y$ con il [[4-Mapping Cylinder|mapping cylinder]] supponiamo che $f$ sia una inclusione.
Segue dalla [[4-Successione lunga in omotopia|successione della coppia]] che $(Y,X)$ è $n$-connessa per ogni $n$, quindi per il fatto sopra con le catene di Eilenberg la mappa indotta dall'inclusione$$H_i(C^{(n,X)}_\bullet(Y))\to H_i(Y)$$è un isomorfismo per ogni $n$ e per ogni $i$. 
Se $i<n$ allora per definizione $C^{(n,X)}_\bullet(Y)=C_\bullet(X)$, quindi scegliendo $n=i+1$ si ha che l'inclusione induce proprio un isomorfismo $H_i(X)\to H_i(Y)$, ma l'inclusione è $f$.


Segue che preso uno spazio qualunque $Y$, se $X\to Y$ è una sua [[2&4 -Teorema di Approssimazione CW|approssimazione CW]] allora $H_\bullet(K)\cong H_\bullet(X)\cong H_\bullet(Y)$, quindi per calcolare l'omologia possiamo sempre ricondurci a complessi CW.