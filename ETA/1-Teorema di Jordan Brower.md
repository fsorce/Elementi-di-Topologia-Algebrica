Sia $K\subseteq S^n$ omeomorfo a $S^{n-1}$, allora $S^n\bs K$ è composto da due componenti connesse per archi, inoltre $K$ è il bordo di entrambe.

lemma 1: Sia $Y\subseteq S^n$ omeomorfo a $I^k$ per $0\leq k\leq n$, allora $\wt H_\bullet(S^n\bs Y)=0$.
$\ul{dim}:$ Se $k=0$ allora $Y$ è dato da un punto e $S^n\bs\cpa{pt}\cong \R^n$ che è contraibile.

Sia ora $k>0$. Consideriamo $Y_+$ e $Y_-$ dati tagliando $Y$ a metà secondo l'identificazione con $I^k$. In questo contesto $Y_+\cap Y_-\cong I^{k-1}$.
Applicando [[1&3 -Mayer Vietoris|Mayer Vietoris]] troviamo la successione$$0\to H_i(S^n\bs Y)\to H_i(S^n\bs Y_+)\oplus H_i(S^n\bs Y_-)\to 0$$dove gli zeri seguono per ipotesi induttiva. 
Se per assurdo $H_i(S^n\bs Y)\neq 0$ allora contiene una classe $u_0$ non banale, che nell'isomorfismo si trasforma in $(u^+_0,u^-_0)$, con almeno una delle due non nulla. Senza perdita di generalità supponiamo $u_1=u^+_0\neq 0$.
Reiterando quanto fatto troviamo una successione di classi non nulle $u_j$ e una successione $Y^j$ (per esempio $Y^1=Y_+$). 

Per il [[1-Lemma sulla compattezza dei supporti delle catene|lemma sulla compattezza dei supporti]] esiste $C\subseteq S^n\bs Y$ compatto tale che esiste $u'\in H_i(C)$ con $u'\mapsto u_0$ tramite inclusione.
Sempre per il [[1-Lemma sulla compattezza dei supporti delle catene|lemma sulla compattezza dei supporti]], poiché $C\subseteq S^n\bs Y^\infty$ (dove $Y^\infty=\bigcap Y^j$), esiste un compatto $C\subseteq K\subseteq S^n\bs Y^\infty$ tale $u'\mapsto 0$ in $H_i(K)$ (per ipotesi induttiva $H_i(S^n\bs Y^\infty)=0$).

Per compattezza $K$ incontra solo un numero finito dei $S^n\bs Y^j$ (aperti che nella loro totalità lo coprono in quanto $K\subseteq S^n\bs Y^\infty$), quindi esiste $m$ tale che $K\subseteq S^n\bs Y^m$, quindi $u_m=0$ necessariamente, assurdo.

---
lemma 2: Sia $Y\subseteq S^n$ omeomorfo a $S^k$ per $0\leq k< n$, allora $\wt H_\bullet(S^n\bs S^k)\cong \Z[n-k-1]$
$\ul{dim}:$ Se $k=0$ allora $Y$ è dato da due punti, quindi $S^n\bs Y\cong \R^n\bs \cpa{pt}\simeq S^{n-1}$.

Sia ora $k>0$. Dividiamo $S^k$ in $I^k_+\cup I^k_-$ calotte che si intersecano in un $S^{k-1}$. Applicando [[1&3 -Mayer Vietoris|Mayer VIetoris]] ricaviamo la successione esatta$$\to \under{=0}{H_{i+1}(S^n\bs I^k_+)\oplus H_{i+1}(S^n\bs I^k_-)}\to \under{=\begin{cases}\Z & i+1=n-(k-1)-1\\ 0&\text{altrimenti}\end{cases}}{H_{i+1}(S^n\bs (I^k_+\cap I^k_-))}\to H_i(S^n\bs Y)\to \under{=0}{H_i(S^n\bs I^k_+)\oplus H_i(S^n\bs I^k_-)}\to $$da cui la tesi visto che $i+1=n-(k-1)-1\coimplies i=n-k-1$ (gli annullamenti seguono dal lemma precedente e la scrittura esplicita per ipotesi induttiva)


$\ul{dim}\text{ (Teorema)}:$ Basta applicare il lemma 2 con $k=n-1$ per trovare la prima parte.

Consideriamo ora la questione del bordo. Siano $C_1$ e $C_2$ le due ccpa. Poiché $S^n\bs Y$ è localmente connesso per archi si ha che le due ccpa sono aperti di $S^n$, quindi il loro bordo è contenuto in $Y$ 
(*$\del C_1=\ol C_1\bs \rg C_1=\ol C_1\bs C_1$, se questo insieme contenesse un punto non in $Y$ allora sarebbe un punto di $C_2$, quindi per apertura di $C_2$ ammetterebbe intorno in $C_2$, assurdo visto che appartiene a $\ol C_1$ e $C_1\cap C_2=\emptyset$*).

Mostriamo ora che tutti i punti di $Y$ appartengono al bordo. Sia $y\in Y$ e sia $N$ un suo intorno aperto in $S^n$. $N\cap Y$ è un suo intorno aperto in $Y$. Dividiamo $Y$ in $A$ e $B$ dischi omeomorfi a $I^{n-1}$ tali che $A\subseteq N\cap Y$ contiene $y$ e $A\cap B\cong S^{n-2}$.

Per il lemma 1 si ha che $S^n\bs B$ è contraibile (in particolare connesso per archi), siano allora $x_1\in C_1$ e $x_2\in C_2$ qualsiasi e colleghiamoli tramite un cammino $\gamma:[0,1]\to S^n\bs B$. Poiché $N$ è aperto, $\gamma\ii(N)$ è un aperto di $[0,1]$ e per costruzione $N\cap S^n\bs B\neq \emptyset$. Osserviamo ora che $\gamma\ii(A)$ è un chiuso di $[0,1]$, quindi compatto, in particolare ammette massimo $t_1$ e minimo $t_0$. Poiché $A\subseteq N$ si ha che $t_0,t_1\in \gamma\ii(N)$.

Poiché $\gamma\ii(N)$ è aperto esistono tempi minori di $t_0$ e maggiori di $t_1$ ma sempre contenuti in $\gamma\ii(N)$. Poiché $(S^n\bs B)\bs N\subseteq S^n\bs Y$ necessariamente $\gamma$ sui tempi appena citati deve andare in $C_1$ e $C_2$ rispettivamente.