Sia $f:A\to A'$ un omomorfismo con relative [[3-Risoluzione libera|risoluzioni libere]] date da $F_1,\ F_0$ e $F_1',\ F_0'$. Esistono allora $f_1:F_1\to F_1'$ e $f_0:F_0\to F_0'$ tali che

```tikz 
\usepackage{tikz-cd} 
\begin{document} 
\begin{tikzcd} 0 & {F_1} & {F_0} & A & 0 \\ 0 & {F_1'} & {F_0'} & {A'} & 0 \arrow[from=1-1, to=1-2] \arrow["i", from=1-2, to=1-3] \arrow[from=2-1, to=2-2] \arrow[from=1-4, to=1-5] \arrow[from=2-4, to=2-5] \arrow["f"', from=1-4, to=2-4] \arrow["{f_0}"', from=1-3, to=2-3] \arrow["{i'}", from=2-2, to=2-3] \arrow["{f_1}"', from=1-2, to=2-2] \arrow["p", from=1-3, to=1-4] \arrow["{p'}", from=2-3, to=2-4] \end{tikzcd}
\end{document}
```


Se $f_1'$ e $f_0'$ sono altre mappe che fanno commutare il diagramma allora esiste $s:F_0\to F_1'$ tale che $f_0-f_0=i's$ e $f_1-f_1'=si$

$\ul{dim}:$ 
- Definiamo prima $f_0$ in modo che commuti il quadrato di destra: Se $x$ è un generatore di $F_0$ poniamo che la sua immagine sia un elemento di $p'\ii(f(p(x)))$, che possiamo fare per surgettività di $p'$.
- Fissata $f_0$, $f_1$ è univocamente determinata da $f_1(x)=i'\ii(f_0(i(x)))$ (ben definita per iniettività di $i'$).

- Per commutatività$$p'(f_0-f_0')=pf-pf=0,$$cioè $f_0-f_0'\in \ker p'=\imm i'$, esiste dunque un sollevamento $s:F_0\to F_1'$, cioè $f_0-f_0'=i's$.
- Notiamo ora che$$i'(f_1-f_1')=f_0i-f_0'i=i'si$$e per iniettività di $i'$ segue $f_1-f_1'=si$.