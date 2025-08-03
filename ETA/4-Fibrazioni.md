Una mappa $p:E\to B$ ha la HLP per $X$ se per ogni omotopia $h:X\times I\to B$ e per ogni mappa $a:X\to B$ tale che $p\circ a=h_0$ esiste $H:X\times I\to E$ che fa commutare il diagramma
```tikz 
\usepackage{tikz-cd} 
\begin{document}
\begin{tikzcd} X & E \\ {X\times I} & B \arrow["{i_0^X}"', from=1-1, to=2-1] \arrow["h"', from=2-1, to=2-2] \arrow["a", from=1-1, to=1-2] \arrow["p", from=1-2, to=2-2] \arrow["H", dashed, from=2-1, to=1-2] \end{tikzcd}
\end{document}
```
Una mappa è fibrazione di Hurewicz se ha la HLP per ogni spazio e fibrazione di Serre se la ha per gli $I^n$. Ricordiamo che i rivestimenti sono fibrazioni di Hurewicz.

