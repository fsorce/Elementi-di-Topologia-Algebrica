Se $A$ e $G$ sono $R$-moduli con $R$ PID e $0\to K(A)\to F(A)\to A\to 0$ è la [[3-Risoluzione libera|risoluzione libera standard]] di $A$ poniamo$$\begin{align}
Tor(A,G)=& \ker(K(A)\otimes G\to F(A)\otimes G)\\
Ext(A,G)=& \coker(Hom(F(A),G)\to Hom(K(A),G))
\end{align}$$In realtà possiamo mostrare che non importa la risoluzione libera scelta:
- Interpretando $0\to K(A)\otimes G\to F(A)\otimes G$ e $Hom(F(A),G)\to Hom(K(A),G)\to 0$ come complessi notiamo che gli $H_1$ e $H^1$ rispettivamente sono proprio $Tor(A,G)$ e $Ext(A,G)$.
- Per il [[3-Lemma sulle risoluzioni libere|lemma sulle risoluzioni libere]], cambiando risoluzione libera troviamo complessi omotopi (questo viene preservato applicando i funtori), quindi troviamo [[1-Omotopia di catene|la stessa omologia]].

Valgono le seguenti proprietà:
- Se $A$ è libero, $Tor(A,G)=0=Ext(A,G)$
- $Tor(\Z/n\Z,G)=\cpa{g\in G\mid ng=0}$
- $Ext(\Z/n\Z,G)=G/nG$
- $Tor(A_1\oplus A_2,G)=Tor(A_1,G)\oplus Tor(A_2,G)$
- $Ext(A_1\oplus A_2,G)=Ext(A_1,G)\oplus Ext(A_2,G)$

Si ha inoltre che $Tor(A,G)=Tor(G,A)$:
Considero due risoluzioni libere $0\to P_1\to P_0\to A\to0$ e $0\to Q_1\to Q_0\to G\to 0$ e disegniamo il diagramma

```tikz 
\usepackage{tikz-cd} 
\begin{document} 
\begin{tikzcd} & 0 & 0 & {Tor(A,G)} \\ 0 & {P_1\otimes Q_1} & {P_1\otimes Q_0} & {P_1\otimes G} & 0 \\ 0 & {P_0\otimes Q_1} & {P_0\otimes Q_0} & {P_0\otimes G} & 0 \\ {Tor(G,A)} & {A\otimes Q_1} & {A\otimes Q_0} & {A\otimes G} & 0 \\ & 0 & 0 & 0 \arrow[from=2-1, to=2-2] \arrow[from=2-2, to=2-3] \arrow[from=2-3, to=2-4] \arrow[from=2-4, to=2-5] \arrow[from=1-2, to=2-2] \arrow[from=1-3, to=2-3] \arrow[from=3-1, to=3-2] \arrow[from=3-4, to=3-5] \arrow[from=3-3, to=3-4] \arrow[from=3-2, to=3-3] \arrow["\alpha", from=2-2, to=3-2] \arrow["\beta", from=2-3, to=3-3] \arrow["\gamma", from=2-4, to=3-4] \arrow[from=1-4, to=2-4] \arrow["{\gamma'}", from=3-4, to=4-4] \arrow["{\beta'}", from=3-3, to=4-3] \arrow["{\alpha'}", from=3-2, to=4-2] \arrow[from=4-2, to=5-2] \arrow[from=4-3, to=5-3] \arrow[from=4-1, to=4-2] \arrow[from=4-2, to=4-3] \arrow[from=4-3, to=4-4] \arrow[from=4-4, to=5-4] \arrow[from=4-4, to=4-5] \end{tikzcd}
\end{document}
```

Applicando il [[0-Lemma del serpente|lemma del serpente]] alle due righe esatte superiori ricaviamo che è esatta la successione$$0\to 0\to Tor(A,G)\to \frac{P_0\otimes Q_1}{\imm \al}\to \frac{P_0\otimes Q_0}{\imm \beta}\to \frac{P_0\otimes G}{\imm \gamma}$$che per esattezza delle colonne e surgettività delle mappe inferiori restituisce la successione esatta$$0\to Tor(A,G)\to A\otimes Q_1\to A\otimes Q_0$$segue dunque che $Tor(A,G)\cong \ker(A\otimes Q_1\to A\otimes Q_0)=Tor(G,A)$.