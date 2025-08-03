Sia $X$ uno spazio topologico. La sua sospensione è $$\Sigma X=\frac{X\times I}{X\times\cpa{0,1}},$$mentre la sua sospensione ridotta (da applicare nel contesto di spazi puntati) è $$SX=\frac{X\times I}{X\times \cpa{0,1}\cup \cpa{x_0}\times I}.$$Sotto lievi ipotesi si ha che $\Sigma X\simeq SX$.

Osserviamo che $SX=S^1\wedge X$, dove l'operazione è il [[4-Prodotto Smash|prodotto smash]]. 

Consideriamo ora uno spazio $X$ e definiamo la seguente mappa tra [[4-Gruppi di omotopia|gruppi di omotopia]]$$\Sigma:\pi_i(X,x_0)=[S^i,X]^0\to [S^1\wedge S^i,S^1\wedge X]^0=\pi_{i+1}(SX,x_0).$$La mappa è in realtà un omomorfismo per $i\geq 1$.
$\ul{dim}:$ Consideriamo il diagramma commutativo
```tikz 
\usepackage{tikz-cd} 
\begin{document} 
\begin{tikzcd} 0 & {\pi_{i+1}(CX,X)} & {\pi_i(X)} & 0 \\ & {\pi_{i+1}(CX/X)} & {\pi_{i+1}(SX)} \arrow["\partial", from=1-2, to=1-3] \arrow[from=1-1, to=1-2] \arrow[from=1-3, to=1-4] \arrow["\Sigma", from=1-3, to=2-3] \arrow["q"', from=1-2, to=2-2] \arrow["\cong"{marking, allow upside down}, draw=none, from=2-2, to=2-3] \end{tikzcd}
\end{document}
```
le altre tre mappe sono omomorfismi perché indotti da mappe continue o appartenenti alla [[4-Successione lunga in omotopia|successione della coppia]] $(CX,X)$.