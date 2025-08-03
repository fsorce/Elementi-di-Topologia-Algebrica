Sia $p:E\to B$ una [[4-Fibrazioni|fibrazione di Serre]], $B_0\subseteq B$, $E_0=p\ii(B_0)$, $b_0\in B_0$ e $e_0\in p\ii(b_0)$, allora $p$ induce una bigezione/isomorfismo$$\pi_n(E,E_0,e_0)\cong \pi_n(B,B_0,b_0).$$In particolare se $B_0=\cpa{b_0}$ e $F=E_0$ allora $\pi_n(E,F,e_0)\cong \pi_n(B,b_0)$, quindi per la [[4-Successione lunga in omotopia|successione lunga in omotopia]] è esatta$$\to \pi_n(F,e_0)\to \pi_n(E,e_0)\to\pi_n(B,b_0)\to\pi_{n-1}(F,e_0)\to$$
$\ul{dim}:$ 
Surgettività) Sia $h:(I^n,\del I^n,J^{n-1})\to (B,B_0,b_0)$ un rappresentante di un elemento del secondo gruppo. A meno di una equivalenza omotopica possiamo interpretare questa mappa come $h:(I^{n-1}\times I,I^{n-1})\to (B,b_0)$. Considerando allora il digramma seguente troviamo $H$ tramite la HLP

```tikz 
\usepackage{tikz-cd} 
\begin{document} 
\begin{tikzcd} {I^{n-1}\simeq J^{n-1}} & E \\ {I^{n-1}\times I} & B \arrow[from=1-1, to=2-1] \arrow["h", from=2-1, to=2-2] \arrow["{cost_{e_0}}", from=1-1, to=1-2] \arrow["p"', from=1-2, to=2-2] \arrow["H", dashed, from=2-1, to=1-2] \end{tikzcd}
\end{document}
```

Grazie a questo diagramma troviamo $H:I^n\to E$ tale che $H(J^{n-1})\subseteq\cpa{e_0}$. Osserviamo inoltre che $$p\circ H(\del I^n)=h(\del I^n)\subseteq B_0\implies H(\del I^n)\subseteq E_0,$$quindi abbiamo trovato $H:(I^n,\del I^n,J^{n-1})\to (E,E_0,e_0)$ tale che $p\circ H=h$.

Iniettività) Siano $f_0,f_1:(I^n,\del I^n,J^{n-1})\to(E,E_0,e_0)$ tali che $p_\ast([f_0])=p_\ast([f_1])$. Per definizione esiste una omotopia $\vp_t:(I^n,\del I^n,J^{n-1})\to (B,B_0,b_0)$ tale che $\vp_0=p\circ f_0$ e $\vp_1=p\circ f_1$. Definiamo ora $$J^n\cong T=I^n\times \cpa{0,1}\cup J^{n-1}\times I\subseteq \del I^{n+1}$$e notiamo che su $T$ possiamo definire una mappa $G$ che sulle facce corrispondenti a $I^n\times \cpa{0,1}$ si comporta come $f_0$ e $f_1$ rispettivamente, mentre sul resto è la mappa costante a $e_0$. Applichiamo ora la HLP al seguente diagramma
```tikz 
\usepackage{tikz-cd} 
\begin{document} 
\begin{tikzcd} {T} & E \\ {I^n\times I} & B \arrow[from=1-1, to=2-1] \arrow["\varphi", from=2-1, to=2-2] \arrow["{G}", from=1-1, to=1-2] \arrow["p"', from=1-2, to=2-2] \arrow["H", dashed, from=2-1, to=1-2] \end{tikzcd}
\end{document}
```

La $H$ trovata è una omotopia tra $f_0$ e $f_1$ che rispetta le inclusioni giuste, quindi $[f_0]=[f_1]$.