Il mapping cylinder è dato da$$M_f=\frac{X\times I\sqcup Y}{(x,0)\sim f(x)}.$$Nota che si retrae per deformazione su $Y$.

Possiamo fattorizzare ogni mappa $f:X\to Y$ in una inclusione ed una retrazione passando attraverso $M_f$.

Se $b$ è la mappa $i^Y_0$ fatta passare al quoziente e similmente per $k:X\times I\to M_f$, il mapping cylinder $M_f$ di $f:X\to Y$ ha la seguente proprietà universale:
Per ogni $Z,\ g$ e omotopia $h$ che fanno commutare, esiste un'unica $\sigma_Z$ che fa commutare.
```tikz 
\usepackage{tikz-cd} 
\begin{document}
\begin{tikzcd} X && Y \\ & {M_f} \\ {X\times I} && Z \arrow["f", from=1-1, to=1-3] \arrow["g", from=1-3, to=3-3] \arrow["h"', from=3-1, to=3-3] \arrow["{k}", from=3-1, to=2-2] \arrow["\sigma_Z", dashed, from=2-2, to=3-3] \arrow["{i^X_0}"', from=1-1, to=3-1] \arrow["{b}"', from=1-3, to=2-2] \end{tikzcd}
\end{document}
```
($M_f$ è il coprodotto fibrato di $X\times I$ e $Y$ su $X$ dove $X\to X\times I$ è l'inclusione al livello $0$).