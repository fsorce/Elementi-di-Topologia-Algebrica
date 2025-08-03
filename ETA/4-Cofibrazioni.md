Una mappa $i:A\to X$ ha la HEP per $Y$ se per ogni omotopia $h:A\times I\to Y$ e per ogni mappa $f:X\to Y$ tale che $f\circ i=h_0$ esiste $H:X\times I\to Y$ che fa commutare il diagramma
```tikz 
\usepackage{tikz-cd} 
\begin{document}
\begin{tikzcd} A && X \\ & {X\times I} \\ {A\times I} && Y \arrow["i", from=1-1, to=1-3] \arrow["f", from=1-3, to=3-3] \arrow["h"', from=3-1, to=3-3] \arrow["{i\times id}", from=3-1, to=2-2] \arrow["H", dashed, from=2-2, to=3-3] \arrow["{i^A_0}"', from=1-1, to=3-1] \arrow["{i^X_0}"', from=1-3, to=2-2] \end{tikzcd}
\end{document}
```
Una mappa è una cofibrazione se ha la HEP per ogni spazio $Y$.

Fatto: le cofibrazioni sono embedding e hanno immagine chiusa se il codominio è Hausdorff.

Se $\cpa{x_0}\inj X$ è una cofibrazione chiusa allora $(X,x_0)$ è uno spazio ben puntato e $x_0$ è un punto base non degenere.

Vale la seguente caratterizzazione delle cofibrazioni: TFAE
1. $i:A\to X$ ha la HEP per $M_i$
2. $i$ è una cofibrazione
3. $\sigma_{X\times I}$ indotta dalla [[4-Mapping Cylinder|proprietà universale]] di $M_i$ ammette una retrazione.
$\ul{dim}:$
$2\implies 1$) Ovvio
$1\implies 2)$ $H=\sigma_Y\circ K$, dove $K$ è l'estensione $K:X\times I\to M_i$ che esiste perché $i$ ha la HEP per $M_i$ e $\sigma_Y$ deriva dalla proprietà universale di $M_i$.
$2\implies 3)$ La retrazione è $H$ estensione di $k:A\times I\to M_i$. La composizione $H\circ \sigma_{X\times I}$ è uguale all'identità perché rispetta la proprietà universale di $M_i$ ponendo come ulteriore spazio $M_i$ stesso.
$3\implies 2)$ Se $H'$ è una retrazione di $\sigma_{X\times I}$ allora l'estensione voluta è $\sigma_Y\circ H':X\times I\to M_i\to Y$.
