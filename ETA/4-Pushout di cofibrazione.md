Se $i:A\to X$ è una [[4-Cofibrazioni|cofibrazione]], $g:A\to Y$ e $Z=\dfrac{X\sqcup Y}{i(a)\sim g(a)}$ ($Z$ è il coprodotto fibrato di $X$ e $Y$ su $A$) allora la proiezione $\pi_Y:Y\to Z$ è una cofibrazione.
$\ul{dim}:$ Verifichiamo la HEP per $W$, $h:Y\times I\to W$ e $f:Z\to W$. Poiché $i$ è una cofibrazione vale il diagramma
```tikz 
\usepackage{tikz-cd} 
\begin{document}
\begin{tikzcd} A && X \\ & {X\times I} \\ {A\times I} && W \arrow["i", from=1-1, to=1-3] \arrow[from=1-1, to=3-1] \arrow[from=1-3, to=2-2] \arrow[from=3-1, to=2-2] \arrow["H", dashed, from=2-2, to=3-3] \arrow["{h\circ g\times id}"', from=3-1, to=3-3] \arrow["{f\circ \pi_X}", from=1-3, to=3-3] \end{tikzcd}
\end{document}
```
Notando ora che $Z\times I$ è il coprodotto fibrato di $Y\times I$ e $X\times I$ su $A\times I$ possiamo anche costruire
```tikz 
\usepackage{tikz-cd} 
\begin{document}
\begin{tikzcd} {A\times I} && {X\times I} \\ \\ {Y\times I} && {Z\times I} \\ \\ &&&& W \arrow["{i\times id}", from=1-1, to=1-3] \arrow["{g\times id}"', from=1-1, to=3-1] \arrow["{\pi_X\times id}"', from=1-3, to=3-3] \arrow["{\pi_Y\times id}", from=3-1, to=3-3] \arrow["{H'}", dashed, from=3-3, to=5-5] \arrow["h"', from=3-1, to=5-5] \arrow["H", from=1-3, to=5-5] \end{tikzcd}
\end{document}
```

