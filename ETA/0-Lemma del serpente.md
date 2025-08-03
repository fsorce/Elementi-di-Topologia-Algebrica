Consideriamo il diagramma
```tikz 
\usepackage{tikz-cd} 
\begin{document}
\begin{tikzcd} & 0 & 0 & 0 \\ & \ker\alpha & \ker\beta & \ker\gamma \\ 0 & A & B & C & 0 \\ 0 & {A'} & {B'} & {C'} & 0 \\ & {\mathrm{coker}\,\alpha} & {\mathrm{coker}\,\beta} & {\mathrm{coker}\,\gamma} \\ & 0 & 0 & 0 \arrow[from=3-1, to=3-2] \arrow[from=3-2, to=3-3] \arrow[from=3-3, to=3-4] \arrow[from=3-4, to=3-5] \arrow[from=2-2, to=3-2] \arrow[from=2-3, to=3-3] \arrow[from=4-1, to=4-2] \arrow[from=4-4, to=4-5] \arrow[from=4-3, to=4-4] \arrow[from=4-2, to=4-3] \arrow["\alpha", from=3-2, to=4-2] \arrow["\beta", from=3-3, to=4-3] \arrow["\gamma", from=3-4, to=4-4] \arrow[from=2-4, to=3-4] \arrow[from=4-2, to=5-2] \arrow[from=4-3, to=5-3] \arrow[from=4-4, to=5-4] \arrow[from=5-2, to=6-2] \arrow[from=5-3, to=6-3] \arrow[from=5-4, to=6-4] \arrow[from=1-2, to=2-2] \arrow[from=1-3, to=2-3] \arrow[from=1-4, to=2-4] \end{tikzcd}
\end{document}
```
dove ogni riga e colonna è esatta, allora è ben definita ed esatta la successione$$\ker \al\to \ker \beta\to \ker \gamma\to \coker\al\to \coker\beta\to\coker\gamma$$