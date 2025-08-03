Siano $A$ un [[2-Complessi CW|complesso CW]] e $Y$ uno spazio topologico. Fissiamo un intero $k\geq -1$ e una mappa continua $f:A\to Y$ tale che $$f_\ast:\pi_i(A)\to \pi_i(Y)\text{ è un isomorfismo per $i<k$ e surgettiva per $i=k$}$$(nel caso $k=-1$ ignoriamo questa condizione).
Allora per ogni $n>k$, potenzialmente anche $n=\infty$, esistono un complesso $X$ che ha $A$ come sottocomplesso e una mappa $F:X\to Y$ che estende $f$ e tale che $$F_\ast:\pi_i(X)\to \pi_i(Y)\text{ è un isomorfismo per $i<n$ e surgettiva per $i=n$.}$$Inoltre $X$ è ottenuto da $A$ [[2-Incollamento di n-celle|incollando]] solo celle di dimensione compresa tra $k$ ed $n$ (inclusi).

$\ul{dim}:$ 
Osserviamo che se $d>k$ allora incollare $d$-celle non modifica i gruppi di omotopia di dimensione $i<k$:
Se $f:S^i\to X$ rappresenta un elemento di $\pi_i(X)$, per [[2&4 -Teorema di approssimazione cellulare|approssimazione cellulare]] questa è omotopa ad una mappa $f':S^i\to A$. 
Similmente se $g$ e $g'$ sono omotope tramite $H:S^i\times I\to X$ allora l'omotopia è omotopa ad una seconda omotopia $H':S^i\times I\to A$, in quanto $i+1\leq k<d$.

Procediamo per induzione su $n$:
$n=0$) Necessariamente $k=-1$ in questo caso. Per ottenere la tesi dobbiamo costruire $X$ in modo da rendere $F_\ast$ surgettiva.
Se $f_\ast$ non è surgettiva aggiungiamo una $0$-cella ad $A$ per ogni ccpa di $Y$ non raggiunta da $f$, estendendo $f$ a $F$ in modo da mappare questo punto aggiunto nella ccpa appropriata.

$n=1$) Supponiamo $f_\ast:\pi_0(A)\to \pi_0(Y)$ surgettiva (se non lo è procediamo come sopra). 
- Rendiamola iniettiva: supponiamo che $a,b\in A^0$ distinti vengano mappati nella stessa ccpa di $Y$, allora incolliamo ad $A$ una $1$-cella che li collega e definiamo $F$ su questa cella in modo che venga mappata in un cammino da $f(a)$ a $f(b)$. Sia $\wt A$ il complesso ottenuto con questi incollamenti.
- Rendiamo surgettiva $F_\ast:\pi_1(\wt A)\to \pi_1(Y)$: Se un loop non viene raggiunto, ne incolliamo uno a $\wt A$ con punto base nella ccpa appropriata e lo mappiamo tramite $F$ nel loop mancante.

$n>1)$ Supponiamo che $f_\ast:\pi_i(A)\to \pi_i(Y)$ sia un isomorfismo per $i<n-1$ e surgettiva per $i=n-1$.
A meno di fattorizzare attraverso il [[4-Mapping Cylinder|mapping cylinder]], supponiamo $f:A\to Y$ inclusione.
Ricordando che $\pi_1(A)\subseteq \pi_1(X)$ [[4-Azione del gruppo fondamentale|agisce]] su $\pi_i(X)$, possiamo dotare $\pi_i(X,A)$ della struttura di $\pi_1(A)$-modulo.
Fissiamo$$(\Phi_j,\vp_j):(D^n,S^{n-1})\to(Y,A)$$generatori di $\pi_n(X,A)$ come $\pi_1(A)$-modulo. Per ognuno di questi [[2-Incollamento di n-celle|incolliamo]] una $n$-cella ad $A$ usando le $\vp_j$ come funzioni caratteristiche. Otteniamo un $X\supseteq A$ ed estendiamo $f$ a $F:X\to Y$ ponendo che $F$ sulla cella $j$ si comporti come $\Phi_j$.
Se $x_j:(D^n,S^{n-1})\to (X,A)$ è l'incollamento di una delle $n$-celle sopra notiamo che $[x_j]\in \pi_n(X,A)$ e che $F_\ast[x_j]=[(\Phi_j,\vp_j)]$. 
Sviluppiamo ora le [[4-Successione lunga in omotopia|successioni esatte in omotopia]] di $(X,A)$ e $(Y,A)$:

```tikz 
\usepackage{tikz-cd} 
\begin{document} 
\begin{tikzcd} {\pi_n(A)} & {\pi_n(X)} & {\pi_n(X,A)} & {\pi_{n-1}(A)} & {\pi_{n-1}(X)} & 0 \\ {\pi_n(A)} & {\pi_n(Y)} & {\pi_n(Y,A)} & {\pi_{n-1}(A)} & {\pi_{n-1}(Y)} & 0 \arrow[from=1-1, to=1-2] \arrow[from=2-1, to=2-2] \arrow[from=1-2, to=1-3] \arrow[from=2-2, to=2-3] \arrow[from=1-3, to=1-4] \arrow[from=2-3, to=2-4] \arrow[from=1-4, to=1-5] \arrow[from=2-4, to=2-5] \arrow[from=2-5, to=2-6] \arrow[from=1-5, to=1-6] \arrow["{F_\ast}", from=1-5, to=2-5] \arrow["{=}"{marking, allow upside down}, draw=none, from=1-1, to=2-1] \arrow["{=}"{marking, allow upside down}, draw=none, from=1-4, to=2-4] \arrow["{F_\ast}", from=1-2, to=2-2] \arrow["{F_\ast}", from=1-3, to=2-3] \end{tikzcd}
\end{document}
```

dove $\pi_{n-1}(X,A)=0$ per [[2&4 -Teorema di approssimazione cellulare|approssimazione cellulare]] e il [[4-Annullamento in gruppi di omotopia relativi|criterio di annullamento per gruppi di omotopia relativi]] e $\pi_{n-1}(Y,A)=0$ perché per ipotesi $\pi_{n-1}(A)\to \pi_{n-1}(Y)$ è surgettiva e $\pi_{n-2}(A)\to \pi_{n-2}(Y)$ è un isomorfismo.

Per costruzione $F_\ast:\pi_n(X,A)\to \pi_n(Y,A)$ è surgettiva (prendiamo ogni generatore su $\pi_1(A)$).

Poiché $\pi_{n-1}(A)\to \pi_{n-1}(Y)$ è surgettiva, per commutatività anche $\pi_{n-1}(X)\to \pi_{n-1}(Y)$ è surgettiva.

Studiando il diagramma ricaviamo subito che $F_\ast:\pi_n(X)\to \pi_n(Y)$ è surgettiva.

Sia $u\in \pi_{n-1}(X)$ e per surgettività sia $u'\in \pi_{n-1}(A)$ una sua preimmagine. Se $u\in \ker F_\ast$ allora per commutatività $u'\in \ker f_\ast=\imm \Delta$, quindi esiste $u''\in \pi_n(Y,A)$ la cui immagine tramite la mappa di bordo è $u'$. Per surgettività di $F_\ast:\pi_n(X,A)\to \pi_n(Y,A)$ troviamo $u'''\in \pi_n(X,A)$ la cui immagine tramite la mappa di bordo è $u'$ per commutatività, ma quindi per esattezza $u$ si ottiene a partire da $u'''$ componendo due mappe successive di una successione esatta, quindi è la classe banale, cioè $F_\ast$ è iniettiva.