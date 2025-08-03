Sia $f:X\to Y$ continua e $j:Y\to C_f$ l'inclusione di $Y$ nel [[4-Coni|mapping cone]]. Allora la seguente successione in coomologia è esatta:$$H^0(Y)\to H^0(X)\to H^1(C_f)\to H^1(Y)\to H^1(X)\to H^2(C_f)\to\cdots$$Inoltre mappe $f$ omotope restituiscono successioni isomorfe.

$\ul{dim}:$ Sia $M_f$ il [[4-Mapping Cylinder|mapping cylinder]] di $f$. Notiamo che $X\subseteq M_f$ e $Y\subseteq M_f$, dove questa inclusione è una equivalenza omotopica. Sviluppando la successione della coppia $(M_f,X)$ in coomologia troviamo $$\to H^{i-1}(X)\to H^i(M_f,X)\to {H^i(M_f)}\to H^i(X)\to$$Poiché $M_f$ si retrae su $Y$ si ha che $H^i(M_f)=H^i(Y)$. 

Osserviamo che $(M_f,X)$ è una buona coppia (un valido intorno di $X\times \cpa1$ è $X\times (0.5,1]$), quindi [[1&3 -Teorema di Escissione|ripercorrendo quanto fatto in omologia]] si ha che $H^i(M_f,X)\cong H^i(M_f/X,\ast)\cong \wt H^i(C_f)$.

Sostituendo quanto trovato nella successione originale troviamo quanto voluto.

Siano ora $f_0,f_1:X\to Y$ omotope tramite $H$. Poiché $i^X_0:X\to X\times I$ e $i^X_1:X\to X\times I$ sono equivalenze omotopiche si ha che entrambe le successioni sono isomorfe a quella data da $H:X\times I\to Y$.