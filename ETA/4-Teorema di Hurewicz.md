Sia $X$ uno spazio topologico connesso per archi, allora esiste un omomorfismo funtoriale$$h_n:\pi_n(X)\to H_n(X),$$inoltre se $X$ è $(n-1)$-connesso allora:
- se $n=1$ la mappa è l'abelianizzazione a meno di isomorfismo,
- se $n>1$ allora $h_n$ è un isomorfismo e $\wt H_i(X)=0$ per $i<n$.

Esiste anche la seguente versione con le ipotesi invertite:
Sia $X$ connesso per archi e semplicemente connesso tale che $\wt H_i(X)=0$ per $i<n$, 
allora $\pi_i(X)=0$ per $i<n$ e $\pi_n(X)\cong H_n(X)$.
(*Applicando Hurewicz una volta troviamo $\pi_2(X)\cong H_2(X)=0$, quindi possiamo riapplicarlo. Procediamo così fino ad $n$*).

$\ul{dim}(\text{teorema}):$
La mappa è $h_n([f])=f_\ast(a)$ per $a$ generatore di $H_n(S^n)$.
$n=1$) C'è una mappa ovvia $$h_1:\pi_1(X,x_0)\to H_1(X)$$definendo $\sigma_\gamma(t,1-t)=\gamma(t)$ (verifica che cammini omotopi vanno in cicli omologhi!). 
Poiché $H_1(X)$ abeliano si fattorizza per $\pi_1(X,x_0)^{ab}\to H_1(X)$. 
Per mostrare che è un isomorfismo definisco una mappa $C_1(X)\to \pi_1(X,x_0)$ e vedo che induce $h'$ in omologia. Poiché $h'\circ h_1=id_{\pi_1(X,x_0)^{ab}}$ si ha che $h_1$ è iniettiva.
Se $\sum a_\sigma\sigma$ è un ciclo osserviamo che è raggiunto da $\sum a_\sigma h'\sigma$, infatti i cammini ausiliari che connettono i vertici di $\sigma$ a $x_0$ si cancellano perché $0=\sum a_\sigma(\sigma_1-\sigma_0)$.

$n>1$) Applicando [[2&4 -Teorema di Approssimazione CW|approssimazione CW]] supponiamo che $X$ sia un complesso CW (sappiamo che [[4-Equivalenza debole induce isomorfismo in omologia|equivalenze deboli inducono isomorfismi in omologia]]). 
Inoltre, poiché $X$ è $(n-1)$-connesso, possiamo considerare una struttura di complesso tale per cui $X^{n-1}=\cpa\ast$ (basta ripercorrere la dimostrazione di [[2&4 -Teorema di Approssimazione CW|approssimazione CW]] notando che non aggiungiamo celle quando $\pi_i(X,\ast)=0$). Da questa condizione sullo scheletro segue la condizione su $\wt H_\bullet(X)$ passando per l'[[2-Complesso cellulare|omologia cellulare]].
Poiché la coppia $(X,X^{n+1})$ è [[2&4 -inclusione di scheletri è n-connessa|(n+1)-connessa]] si ha dalla [[4-Successione lunga in omotopia|successione della coppia in omotopia]] che $\pi_{n}(X^{n+1})\cong \pi_n(X)$. 
Similmente per quello che sappiamo sugli [[2-Incollamento di n-celle|incollamenti]] e la [[1-Successione della coppia e della tripla|successione della coppia in omologia]] ricaviamo che $H_n(X^{n+1})\cong H_n(X)$.

Ci siamo ricondotti a mostrare la tesi per $X=X^{n+1}$ e $X^n=\bigvee_\al S^n_\al$.
Poiché $X^{n+1}$ è ottenuto da $X^n$ incollando $(n+1)$-celle esistono mappe di incollamento che si restringono sul bordo a $\vp_j:S^{n}_j\to \bigvee_\al S^n_\al$. A meno di omotopia [[2&4 -Teorema di approssimazione cellulare|supponiamole cellulari]], questo ci permette di definire$$\vp:\bigvee_jS^n_j\to\bigvee_\al S^n_\al.$$Osserviamo che $X^{n+1}$ è omotopicamente equivalente al [[4-Coni|mapping cone]] di $\vp$ ($(C\bigvee_j S^n_j)\bs \bigvee_j S^n_j$ sono le parti aperte delle $(n+1)$-celle).

Osserviamo che per $S^n$ la tesi vale ponendo $h_n([f])=f_\ast(a)$, dove $a$ è un generatore di $H_n(S^n)$ fissato (*$h_n([id])=a$, quindi surgettiva, iniettiva perché $\pi_n(S^n)\cong \Z$ quindi $h_n$ è determinata dall'immagine di un generatore e questo non può andare a zero perché $a$ sta nell'immagine*). 

Se $X=\bigvee S^n_\al$ la tesi vale per quanto detto sull'[[4-Omotopia di bouquet di sfere|omotopia del bouquet di sfere]] e la naturalità e additività di $H_n$.

In generale consideriamo il diagramma
```tikz 
\usepackage{tikz-cd} 
\begin{document} 
\begin{tikzcd} {\pi_n(\bigvee_jS^n_j)} & {\pi_{n}(\bigvee_\alpha S^n_\alpha)} & {\pi_{n}(\bigvee_\alpha S^n_\alpha,\bigvee_j S^n_j)} & 0 \\ {H_n(\bigvee_jS^n_j)} & {H_{n}(\bigvee_\alpha S^n_\alpha)} & {H_{n}(\bigvee_\alpha S^n_\alpha,\bigvee_j S^n_j)} & 0 \arrow[from=1-1, to=1-2] \arrow[from=2-1, to=2-2] \arrow[from=1-2, to=1-3] \arrow[from=2-2, to=2-3] \arrow[from=2-3, to=2-4] \arrow[from=1-3, to=1-4] \arrow[from=1-3, to=2-3] \arrow[from=1-2, to=2-2] \arrow[from=1-1, to=2-1] \end{tikzcd}
\end{document}
```
Per quanto detto le prime due mappe sono isomorfismi, quindi con un po' di diagram chasing ricaviamo che anche la mappa sulle coppie è un isomorfismo.
Per quanto detto $X=C_\vp$. A meno di allargare un pochino pensiamo a $C\bigvee_j S^n_j$ come ad un aperto di $X$ e notiamo che contiene i centri delle $(n+1)$-celle.
Applicando [[4-Escissione in omotopia|escissione in omotopia]] (*usando la [[4-Successione lunga in omotopia|successione della coppia]] per $(C\bigvee_j S_j^n, \bigvee_j S_j^n)$ e $(\bigvee_\al S_\al^n, \bigvee_j S_j^n)$ si ha che i $\pi_i$ dei primi si annullano per $i-1<n$ e quelli dei secondi per $i<n$, in definitiva $p+q-2=2n+1=2n-1>n$*) al primo gruppo ed [[1&3 -Teorema di Escissione|escissione in omologia]] al secondo ricaviamo isomorfismi $$\pi_n(\bigvee_\al S^n_\al,\bigvee_j S^n_j)\cong \pi_n(X,C\bigvee_j S^n_j)\overset{\text{coni sono contraibili}}\cong \pi_n(X,\ast)$$e$$H_n(\bigvee_\al S^n_\al,\bigvee_j S^n_j)\cong H_n(X,C\bigvee_j S^n_j)\overset{\text{coni sono contraibili}}\cong H_n(X).$$