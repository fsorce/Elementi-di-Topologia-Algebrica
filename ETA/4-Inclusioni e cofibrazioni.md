Sia $i:A\to X$ una inclusione chiusa, allora $i$ è una [[4-Cofibrazioni|cofibrazione]] se e solo se l'inclusione $j:X\times \cpa{0}\cup A\times I\inj X\times I$ ammette retrazione.
$\ul{dim}:$ 
Usiamo il fatto che $i$ è inclusione chiusa implicitamente come condizione necessaria affinché $X\times\cpa0\cup A\times I$ sia ben definito e possa essere immagine di una retrazione.
$\implies$) Usiamo la HEP scegliendo come spazio $X\times\cpa{0}\cup A\times I$ e come mappe quella che manda $X$ nella fetta $X\times \cpa{0}$ (la chiamiamo $f$) e quella che include $A\times I$ in $X\times \cpa{0}\cup A\times I$ (che chiamiamo $h$):
```tikz 
\usepackage{tikz-cd} 
\begin{document}
\begin{tikzcd} A && X \\ & {X\times I} \\ {A\times I} && {X\times\{0\}\cup A\times I} \arrow["i", from=1-1, to=1-3] \arrow["f", from=1-3, to=3-3] \arrow["h"', from=3-1, to=3-3] \arrow["{i\times id}", from=3-1, to=2-2] \arrow["H", dashed, from=2-2, to=3-3] \arrow["{i^A_0}"', from=1-1, to=3-1] \arrow["{i^X_0}"', from=1-3, to=2-2] \end{tikzcd}
\end{document}
```
La $H$ trovata è la retrazione voluta, infatti $H\circ j=id$ per commutatività del diagramma e la scelta di $h$ e $f$.
$\impliedby$) Verifichiamo la HEP per $Y$. Siano dunque $h:A\times I\to Y$ omotopia e $f:X\to Y$ continua che commutano con l'inclusione di $A$ nei due pezzi. Segue che è ben definita una mappa $K:X\times \cpa{0}\cup A\times I\to Y$ che commuta con queste. L'estensione cercata allora è $H=K\circ r$. dove $r$ è la retrazione supposta.