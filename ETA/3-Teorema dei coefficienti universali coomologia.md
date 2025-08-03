Sia $(C_\bullet,\del)$ un complesso di catene di moduli liberi, allora la successione$$0\to Ext(H_{n-1}(C_\bullet),G)\to H^n(C_\bullet,G)\overset{\al}\to Hom(H_n(C_\bullet),G)\to0$$è naturale e spezza. L'ultima mappa è data da $\al(\vp)([c])=\vp(c)$.
Segue immediatamente dal teorema che $$H^n(C_\bullet, G)\cong Hom(H_n(C_\bullet), G)\oplus Ext(H_{n-1}(C_\bullet),G).$$$\ul{dim}:$ Possiamo dotare i cicli e i bordi della struttura di complesso restringendo la mappa di bordo, la quale diventa sempre il morfismo banale.
Notiamo che $0\to Z_\bullet\to C_\bullet\to B_{\bullet-1}\to 0$ è esatta e ==spezza== in quanto se $C_\bullet$ è libero anche $Z_\bullet$ e $B_\bullet$ lo sono. Possiamo dunque [[3-Coomologia a coefficienti in gruppo|applicare Hom]] e ricavare una seconda successione esatta $$0\to Hom(B_{\bullet-1},G)\to Hom(C_\bullet, G)\to Hom(Z_{\bullet}, G)\to 0.$$Passando in omologia troviamo la [[1-Omomorfismo di connessione|successione esatta lunga]]$$\to Hom(Z_{n-1},G)\overset{\vp^{n-1}}\to Hom(B_{n-1},G)\to  H^n(C_\bullet,G)\to Hom(Z_n,G)\overset{\vp^n}\to Hom(B_n,G)\to$$Notiamo che l'omomorfismo di connessione $\vp^\bullet$ è $Hom(\subseteq,G)$ per l'==inclusione== $B_\bullet\subseteq Z_\bullet$, *(infatti ripercorrendo la [[1-Omomorfismo di connessione|dimostrazione]], sia $\psi\in Hom(Z_n,G)$, che possiamo estendere a $\wt\psi\in Hom(C_n,G)$ per surgettività. Applicando il cobordo $\delta$ troviamo $\delta \wt \psi(c)=\wt \psi(\del c)=\psi(\del c)=\delta \psi(c)$, dove abbiamo usato il fatto che $B_{n}\subseteq Z_{n}$. In definitiva la classe di $\psi\in Hom(B_n,G)$ è l'immagine della classe di $\psi\in Hom(Z_n,G)$ tramite l'omomorfismo di connessione, cioè $\vp^n$ è indotta dall'inclusione)*.

Dalla successione esatta lunga sopra estraiamo l'esatta corta$$0\to \coker\vp^{n-1}\to H^n(C_\bullet,G)\to \ker\vp^{n}\to 0$$Il [[3-Tor e Ext|primo termine]] è $$\coker\vp^{n-1}=\coker(Hom(Z_{n-1}, G)\to Hom(B_{n-1}, G))=Ext(H_{n-1}(C_\bullet),G)$$per il secondo ricordiamo l'esattezza sinistra di $Hom(\cdot, G)$ e la applichiamo come segue:
$$
\begin{gather}
0\to B_n\to Z_n\to H_n(C_\bullet)\to 0\\
0\to Hom(H_n(C_\bullet),G)\to Hom(Z_n,G)\overset{\vp^n}\to Hom(B_n,G)
\end{gather}$$da cui segue che $Hom(H_n(C_\bullet),G)\cong \ker\vp^n$.

Per concludere basta ==mostrare che la successione spezza==:
Sia $r:C_n\to Z_n$ una retrazione e consideriamo il diagramma
```tikz 
\usepackage{tikz-cd} 
\begin{document}
\begin{tikzcd} & \ker\delta \\ 0 & {Z_n(Hom(C_\bullet,G))} & {Hom(C_n,G)} & {Hom(C_{n+1},G)} \\ 0 & {Hom(H_n(C_\bullet),G)} & {Hom(Z_n,G)} & {Hom(B_n,G)} \\ & {\ker\varphi^n} \arrow["{\varphi^n}", from=3-3, to=3-4] \arrow[from=3-2, to=3-3] \arrow[from=3-1, to=3-2] \arrow[from=2-1, to=2-2] \arrow["{=}"{marking, allow upside down}, draw=none, from=4-2, to=3-2] \arrow["{r^\#}", from=3-3, to=2-3] \arrow[from=2-2, to=2-3] \arrow["\delta", from=2-3, to=2-4] \arrow["{Hom(\partial,G)}"', from=3-4, to=2-4] \arrow["{=}"{marking, allow upside down}, draw=none, from=1-2, to=2-2] \end{tikzcd}
\end{document}
```

Notiamo che $r^\#$ ristretta a all'immagine di $Hom(H_n(C_\bullet),G)$ ha immagine in $\ker \delta$ per commutatività del diagramma, quindi per esattezza possiamo costruire un omomorfismo $\rho=[r^\#\circ \pi^\#]$, dove $\pi:Z_n\to H_n(C_\bullet)$ è la proiezione. Osserviamo che la mappa è una retrazione per $\al$ perché se $[\psi]\in H^n(C_\bullet,G)$ allora $$\rho(\al([\psi]))=[r^\#(\pi^\#(\al([\psi])))]=[\al([\psi])[r]]=[\psi|_{Z_n}\circ r]=[\psi].$$