La mappa naturale ovvia $EZ_0:C_0(X\times Y)\to C_0(X)\otimes C_0(Y)$ si estende ad un morfismo di complessi che induce un isomorfismo in omologia.
$\ul{dim}:$ Vogliamo applicare il [[1-Teorema dei funtori liberi-aciclici|teorema dei funtori liberi e aciclici]] usando i funtori $Top\times Top\to \Cc\Hc_+$ dati da $C_\bullet(\cdot)\otimes C_\bullet(\cdot)$ e $C_\bullet(\cdot\times\cdot)$. Come modelli possiamo scegliere 
- $B_{n,k}=(\Delta^k,\Delta^{n-k})$ e $b_{n,k}=id\otimes id$ per il primo funtore e 
- $B_n=(\Delta^n,\Delta^n)$ e $b_n=\Delta$, dove $\Delta:\Delta^n\to\Delta^n\times\Delta^n$ è la mappa diagonale. 
Queste scelte rendono liberi e aciclici entrambi i funtori (ovviamente liberi e per aciclicità basta [[3-Complessi contraibili e aciclici|ricordare]] che $\Delta^n$ è contraibile).
In omologia di grado $0$ troviamo mappe naturali $EZ_0$ e la sua inversa $Q_0$, che per il teorema si estendono a morfismi naturali.
Sempre per il [[1-Teorema dei funtori liberi-aciclici|teorema]] notiamo che, poiché $EZ_0$ e $Q_0$ sono inverse, $EZ_0\circ Q_0=id$ e $Q_0\circ EZ_0=id$, quindi $EZ\circ Q$ e $Q\circ EZ$ sono morfismi omotopi all'identità.
Passando in omologia si ha dunque che $EZ_\ast$ è invertibile, cioè è un isomorfismo.

Esiste anche la seguente versione relativa del teorema: 
le mappe orizzontali inducono isomorfismi in omologia

```tikz 
\usepackage{tikz-cd} 
\begin{document}
\begin{tikzcd} 0 & 0 \\ {C_\bullet(A\times Y)+C_\bullet(X\times B)} & {C_\bullet(A)\otimes C_\bullet(Y)+C_\bullet(X)\otimes C_\bullet(B)} \\ {C_\bullet(X\times Y)} & {C_\bullet(X)\otimes C_\bullet(Y)} \\ {C(X\times Y)/(C(A\times Y)+C(X\times B))} & {C_\bullet(X,A)\otimes C_\bullet(Y,B)} \\ 0 & 0 \arrow[from=1-2, to=2-2] \arrow[from=2-2, to=3-2] \arrow[from=3-2, to=4-2] \arrow[from=4-2, to=5-2] \arrow[from=1-1, to=2-1] \arrow[from=2-1, to=3-1] \arrow[from=3-1, to=4-1] \arrow[from=4-1, to=5-1] \arrow["EZ", from=3-1, to=3-2] \arrow["{EZ''}", from=4-1, to=4-2] \arrow["{EZ'}", from=2-1, to=2-2] \end{tikzcd}
\end{document}
```
$\ul{dim}:$ Per naturalità $EZ$ e $Q$ si restringono bene quindi il diagramma commuta.
Sempre per naturalità commuta il diagramma
```tikz 
\usepackage{tikz-cd} 
\begin{document}
\begin{tikzcd} 0 & 0 \\ {C_\bullet(A\times B)} & {C_\bullet(A)\otimes C_\bullet(B)} \\ {C_\bullet(X\times B)\oplus C_\bullet(A\times Y)} & {C_\bullet(X)\otimes C_\bullet(B)\oplus C_\bullet(A)\otimes C_\bullet(Y)} \\ {C_\bullet(X\times B)+C_\bullet(A\times Y)} & {C_\bullet(X)\otimes C_\bullet(B)+ C_\bullet(A)\otimes C_\bullet(Y)} \\ 0 & 0 \arrow[from=1-2, to=2-2] \arrow[from=2-2, to=3-2] \arrow[from=3-2, to=4-2] \arrow[from=4-2, to=5-2] \arrow[from=1-1, to=2-1] \arrow[from=2-1, to=3-1] \arrow[from=3-1, to=4-1] \arrow[from=4-1, to=5-1] \arrow["{EZ'}", from=2-1, to=2-2] \arrow["{EZ'}", from=3-1, to=3-2] \arrow["{EZ'}", from=4-1, to=4-2] \end{tikzcd}
\end{document}
```
Passando ora alle [[1-Omomorfismo di connessione|successioni esatte lunghe]] in omologia e ricordando la ==naturalità dell'omomorfismo di connessione== troviamo che $EZ'_\ast$ è un isomorfismo due volte ogni tre termini, quindi per il [[0-Lemma dei 5|lemma dei 5]] troviamo l'isomorfismo
$$EZ'_\ast:H_\bullet(C_\bullet(A\times Y)+C_\bullet(X\times B))\to H_\bullet(C_\bullet(A)\otimes C_\bullet(Y)+C_\bullet(X)\otimes C_\bullet(B)).$$Per concludere basta fare lo stesso ragionamento sul digramma del testo per mostrare che $EZ''$ induce iso.