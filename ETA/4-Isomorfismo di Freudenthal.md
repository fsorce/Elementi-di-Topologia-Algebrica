La [[4-Sospensione|mappa di sospensione]] $\Sigma:\pi_{i-1}(S^n)\to \pi_{i}(S^{n+1})$ è un isomorfismo per $0<i<2n$ e suriettiva per $i=2n$.
$\ul{dim}:$ Notiamo che $S S^n=S^{n+1}$ e $CS^n\cong E^{n+1}_+\cong E^{n+1}_-$. 
Consideriamo allora il diagramma commutativo
```tikz 
\usepackage{tikz-cd} 
\begin{document} 
\begin{tikzcd} 0 & {\pi_{i}(E^{n+1}_-,S^n)} & {\pi_{i-1}(S^n)} & 0 \\ & {\pi_{i}(E^{n+1}_-/S^n)} & {\pi_{i}(S^{n+1})} \arrow["\partial", from=1-2, to=1-3] \arrow[from=1-1, to=1-2] \arrow[from=1-3, to=1-4] \arrow["\Sigma", from=1-3, to=2-3] \arrow["q"', from=1-2, to=2-2] \arrow["\cong"{marking, allow upside down}, draw=none, from=2-2, to=2-3] \end{tikzcd}
\end{document}
```
La tesi segue se $q$ è un isomorfismo per $0<i<2n$ e surgettiva per $i=2n$.
Consideriamo ora il seguente diagramma
```tikz 
\usepackage{tikz-cd} 
\begin{document} 
\begin{tikzcd} {\pi_{i}(E^{n+1}_-,S^n)} & {\pi_{i-1}(E^{n+1}_-/S^n)} \\ {\pi_{i}(S^{n+1},E^{n+1}_+)} & {\pi_{i}(S^{n+1}/E^{n+1}_+)} \arrow["q", from=1-1, to=1-2] \arrow["\cong"{marking, allow upside down}, draw=none, from=1-2, to=2-2] \arrow["{\subseteq_\ast}"', from=1-1, to=2-1] \arrow["\cong"{marking, allow upside down}, draw=none, from=2-1, to=2-2] \end{tikzcd}
\end{document}
```
La mappa di destra è un isomorfismo perché deriva da un omeomorfismo, quella in basso è un isomorfismo perché le coppie $(S^{n+1},E^{n+1}_+)$ e $(S^{n+1}/E^{n+1}_+,\ast)$ sono omotopicamente equivalenti.

Ricordando che $\pi_{i}(E^{n+1}_-,S^n)\cong \pi_{i}(E^{n+1}_+,S^n)\cong \pi_{i-1}(S^n)=0$ per $0< i< n+1$ troviamo per [[4-Escissione in omotopia|escissione]] che $\subseteq_\ast$ è un isomorfismo per $0<i<2n$ e surgettiva per $i=2n$, come voluto.