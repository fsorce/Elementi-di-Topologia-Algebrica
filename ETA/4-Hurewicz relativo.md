Sia $(X,A)$ una coppia di [[2-Complessi CW|complessi CW]] semplicemente connessi e tale che $H_i(X,A)=0$ per $i<n$ per un $n\geq 2$ fissato. Allora $\pi_i(X,A)=0$ per $i<n$ e $h_n:\pi_n(X,A)\to H_n(X,A)$ è un isomorfismo.

$\ul{dim}:$ 
Osserviamo che, poiché $X$ e $A$ sono semplicemente connessi vale anche $\pi_1(X,A)=0$:
Sviluppando la [[4-Successione lunga in omotopia|successione della coppia]], ricaviamo $0\to \pi_1(X,A)\to0$, quindi $\pi_1(X)=0$ si surgetta in $\pi_1(X,A)$, quindi in particolare $\pi_1(X,A)=0$.

Osserviamo che $(X,A)$ è una buona coppia, quindi per [[1&3 -Teorema di Escissione|escissione]] $H_\bullet(X,A)=\wt H_\bullet(X/A)$. 

Consideriamo il seguente lemma:
Se $(X,A)$ è [[4-Spazi n-connessi|(n-1)-connessa]] e $A$ è semplicemente connesso (e quindi $(CA,A)$ è $2$-connessa) si ha per [[4-Escissione in omotopia|escissione in omotopia]] che la mappa $$\pi_i(X,A)\overset{esc}\to \pi_i(X\cup CA,CA)\overset{\text{eq.\ omot.}}\cong \pi_i((X\cup CA)/CA,\ast)=\pi_i(X/A)$$è un isomorfismo per $i< (n-1)+2=n+1$.

Teniamo a mente il diagramma
```tikz 
\usepackage{tikz-cd} 
\begin{document}
\begin{tikzcd} {\pi_i(X,A)} & {\pi_i(X/A)} \\ {H_i(X,A)} & {\widetilde H_i(X/A)} \arrow["{h_i}", from=1-1, to=2-1] \arrow["{h_i}", from=1-2, to=2-2] \arrow["esc", from=2-1, to=2-2] \arrow["{p_\ast}", from=1-1, to=1-2] \end{tikzcd}
\end{document}
```
Procediamo per induzione:
$n=2$) Abbiamo già mostrato che $\pi_1(X,A)=0$. Invocando il [[4-Teorema di Hurewicz|teorema di Hurewicz]] per $X/A$ abbiamo la tesi per commutatività del diagramma.

$n>2)$ Applicando induzione forte supponiamo che $(X,A)$ sia $(n-1)$-connesso (infatti per $i<n$ si ha $\pi_i(X,A)\cong H_i(X,A)=0$). Invocando il [[4-Teorema di Hurewicz|teorema di Hurewicz]] per $X/A$ la tesi segue per commutatività del diagramma.