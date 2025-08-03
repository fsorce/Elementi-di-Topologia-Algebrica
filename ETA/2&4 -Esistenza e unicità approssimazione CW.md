Una mappa $f:X\to Y$ è detta equivalenza omotopica debole se induce isomorfismi tra i [[4-Gruppi di omotopia|gruppi di omotopia]] in ogni grado.

Per il [[2&4 -Teorema di Approssimazione CW|teorema di approssimazione CW]] applicato scegliendo $A=\cpa{\ast}$, $k=-1$ e $n=\infty$ ricaviamo che esiste un [[2-Complessi CW|complesso CW]] $X$ e una mappa $F:X\to Y$ equivalenza omotopica debole. Una tale mappa è detta approssimazione CW.

Le approssimazioni CW di un dato spazio connesso per archi sono uniche a meno di equivalenza omotopica.
$\ul{dim}:$ Siano $F_1:X_1\to Y$ e $F_2:X_2\to Y$ due approssimazioni CW dello stesso spazio. 
Vogliamo costruire $f:X_1\to X_2$ tale che $F_1=F_2\circ f$, così facendo passando alle indotte sui gruppi di omotopia troveremo che anche $f$ è una equivalenza debole, ma per il [[2&4 -Teorema di Whitehead|teorema di Whitehead]] le equivalenze omotopiche deboli tra [[2-Complessi CW|complessi CW]] connessi per archi sono equivalenze omotopiche.

A meno di passare per il [[2&4 -Mapping cylinder di mappa cellulare è complesso|mapping cylinder]] $M_{F_2}$ supponiamo che $F_2$ sia una inclusione ($F_1$ viene composta con l'inclusione di $Y$ in $M_{F_2}$ e resta una approssimazione CW).
In quanto l'inclusione $F_2$ è un'equivalenza omotopica debole, notiamo che $(Y,X_2)$ è $i$-connesso per ogni $i$, cioè $\pi_i(Y,X_2)=0$ in ogni grado.
Per il [[2&4 -Costruzione di omotopie relative da CW|criterio sulla costruzione di omotopie relative da complessi CW]] si ha che la mappa $F_1:X_1\to Y$ è omotopa ad una mappa $f:X_1\to X_2$.