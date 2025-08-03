Ricordiamo l'[[2-Incollamento di n-celle|isomorfismo]] $\Phi:\bigoplus_\la H_n(D^n,S^{n-1})\to H_n(X,A)$. Notiamo che fissata una cella $e$ possiamo tornare indietro componendo inclusione ed [[1&3 -Teorema di Escissione|escissione]] come segue:$$H_n(X,A)\to H_n(X,X\bs e)\to H_n(D^n,S^{n-1}).$$Grazie a questo isomorfismo possiamo trasformare la mappa di bordo $C_n(K)\to C_{n-1}(K)$ in una matrice $$m(\la,\mu):\bigoplus_\la H_n(D^n_\la,S^{n-1}_\la)\to \bigoplus_\mu H_{n-1}(D^{n-1}_\mu,S^{n-2}_\mu).$$Osserviamo ora che ha senso definire $L^{\la,\mu}$ come la composizione$$S_\la^{n-1}\overset{{f_\la}|_{S^{n-1}_\la}}{\to}K^{n-1}\to K^{n-1}/(K^{n-1}\bs e^{n-1}_\mu)=\ol e^{n-1}_\mu/\del e^{n-1}_\mu\cong S^{n-1}$$chiamiamo il [[2-Gradi di mappe tra sfere|grado]] di questa mappa numero di incidenza.

Le mappe $m(\la,\mu)$ e $L^{\la,\mu}$ sono legate dal seguente diagramma:

```tikz 
\usepackage{tikz-cd} 
\begin{document} 
\begin{tikzcd} {H_n(D^n_\lambda,S^{n-1}_\lambda)} \\ & {H_n(K^n,K^{n-1})} &&& {H_{n-1}(D^{n-1}_\mu,S^{n-2}_\mu)} \\ & {H_{n-1}(K^{n-1})} & {H_{n-1}(K^{n-1},K^{n-2})} & {H_{n-1}(K^{n-1},K^{n-1}\setminus e_\mu^{n-1})} \\ {\widetilde H_{n-1}(S^{n-1}_\lambda)} &&& {\widetilde H_{n-1}(K^{n-1}/(K^{n-1}\setminus e^{n-1}_\mu))} \\ &&&& {\widetilde H_{n-1}(S^{n-1})} \arrow["\partial"', from=1-1, to=4-1] \arrow["\Phi", from=1-1, to=2-2] \arrow["\partial", from=2-2, to=3-2] \arrow["{\subseteq_\ast}", from=4-1, to=3-2] \arrow["{\subseteq_\ast}"', from=3-2, to=3-3] \arrow["{\subseteq_\ast}"', from=3-3, to=3-4] \arrow["{p_\ast}", from=3-4, to=4-4] \arrow["esc"', from=3-4, to=2-5] \arrow["{p_\ast}", from=2-5, to=5-5] \arrow["esc", from=4-4, to=5-5] \arrow["{L^{\lambda,\mu}}", from=4-1, to=5-5] \arrow["{m(\lambda,\mu)}", from=1-1, to=2-5] \arrow["\Phi"', from=2-5, to=3-3] \arrow["{d_n}", from=2-2, to=3-3] \end{tikzcd}
\end{document}
```

---
***Nota bene:*** I numeri di incidenza sono definiti a meno del segno in quanto abbiamo fatto delle scelte con le specifiche $f_\la$ e l'omeomorfismo tra $D^n/S^{n-1}$ e $S^n$.