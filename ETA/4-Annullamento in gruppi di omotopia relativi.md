Sia $f:(D^i,S^{i-1},\ast)\to (X,A,x_0)$. $f$ è banale in $\pi_i(X,A,x_0)$ se e solo se è omotopa ad una mappa $f':D^i\to A$. Inoltre l'omotopia che costruiamo supponendo $f$ banale è costante su $S^{i-1}$.
$\ul{dim}:$
$\impliedby$) Costruiamo l'omotopia$$H(x,t)=\begin{cases}
h(x,2t) & t\in [0,0.5]\\
f'((2t-1)\ast+(2-2t) x) & t\in [0.5,1]
\end{cases}$$e funziona perché $S^{i-1}\subseteq D^i$ continua ad essere mappato in $A$.
$\implies$) Sia $G$ una omotopia da $f$ alla mappa costante. Per avere la tesi dovremo trovare una omotopia che garantisca che $H(S^{i-1},t)\subseteq A$ per ogni $t$. Costruiamo$$H(x,t)=\begin{cases}
G(\frac2{2-t}x,t) & 0\leq \norm x\leq \frac{2-t}2\\
G(\frac x{\norm x},2-2\norm x) & \frac{2-t}2\leq \norm x\leq 1
\end{cases}$$Notiamo che $H$ è continua perché per $\norm x=1-t/2$ entrambe le espressioni sono $G(\frac x{\norm x},t)$. 
Osserviamo che $H(\cdot,0)=G(\cdot,0)=f$, $H(\cdot,1)\subseteq G(S^{i-1},\cdots)\cup\cpa{x_0}\subseteq A$ e se $x\in S^{i-1}$ allora $H(x,t)=G(x,0)=H(x,0)$, cioè $H(\cdot ,t)|_{S^{i-1}}$ è costante.