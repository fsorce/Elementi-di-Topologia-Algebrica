Osserviamo che per il [[4-Inclusioni e cofibrazioni|criterio sulle inclusioni]], l'inclusione chiusa $S^{n-1}\subseteq D^{n}$ è una cofibrazione, infatti $D^n\times I$ si può retrarre su $D^n\times\cpa{0}\cup S^{n-1}\times I$ proiettando da $(\ul0,2)$.

Sia ora $X$ un [[2-Complessi CW|complesso CW]] con $n$-scheletro $X^n$. Affermiamo che anche l'inclusione $X^n\subseteq X$ è una cofibrazione.
$\ul{dim}:$ Per quanto detto $S^{n}_\la\to D^{n+1}_\la$ sono cofibrazioni, quindi anche $\bigsqcup S^n_\la\to \bigsqcup_\la D^{n+1}_\la$ lo è. Dalla commutatività del seguente diagramma segue per [[4-Pushout di cofibrazione|il criterio sul pushout di cofibrazioni]] che anche $X^n\to X^{n+1}$ è una cofibrazione ($X^{n+1}$ è ottenuto da $X^n$ [[2-Incollamento di n-celle|incollando]] i $D^{n+1}_\la$)
```tikz 
\usepackage{tikz-cd} 
\begin{document} 
\begin{tikzcd} {\bigsqcup_\lambda S^n_{\lambda}} & {\bigsqcup_\lambda D^{n+1}_\lambda} \\ {X^n} & {X^{n+1}} \arrow["\subseteq"', from=2-1, to=2-2] \arrow["{(f_\lambda)_\lambda}"', from=1-1, to=2-1] \arrow["{\subseteq }", from=1-1, to=1-2] \arrow["{(f_\lambda)_\lambda}", from=1-2, to=2-2] \end{tikzcd}
\end{document}
```
Poiché la composizione di cofibrazioni è cofibrazione, tutte le inclusioni $X^n\subseteq X^{n+m}$ sono cofibrazioni. Allora anche $X^n\subseteq X$ lo è, basta estendere l'omotopia uno scheletro alla volta sempre più rapidamente.
