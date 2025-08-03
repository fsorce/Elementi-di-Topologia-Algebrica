Fissiamo una mappa $f:S^{2n-1}\to S^n$ con $n>1$. Fissiamo anche $x\in H^{2n-1}(S^{2n-1})$ e $y\in H^n(S^n)$ generatori.
Sviluppando la [[4-Successione in coomologia del cono|successione del cono di ]]$f$ troviamo$$\under{=0}{H^{n-1}(S^{2n-1})}\to H^n(C_f)\to H^n(S^n)\to \under{=0}{H^n(S^{2n-1})}$$da cui $H^n(C_f)\cong \Z$. Analogamente in gradi alti $\Z=H^{2n-1}(S^{2n-1})\cong H^{2n}(C_f)$.

Siano $\al=(j^\ast)\ii(y)\in H^n(C_f)$ e $\beta=\del^\ast(x)\in H^{2n}(C_f)$. 
Poiché sia $j^\ast$ che $\del^\ast$ sono isomorfismi nei gradi considerati, $\al$ e $\beta$ generano i rispettivi gruppi.

Osserviamo che $\al\cup \al\in H^{2n}(C_f)$, quindi è multiplo di $\beta$, cioè$$\al^2=\Hc(f)\beta.$$Il numero $\Hc(f)$ è l'invariante di Hopf.

Osserviamo che se $g:S^n\to S^n$ ha [[2-Gradi di mappe tra sfere|grado]] $m$ e $k:S^{2n-1}\to S^{2n-1}$ ha grado $r$ allora$$\Hc(g\circ f\circ k)=m^2k\cdot \Hc(f).$$Se $n$ è dispari allora per l'[[3-Prodotto cup|anticommutatività del prodotto cup]] $\al^2=(-1)^{n}\al^2=-\al^2$, quindi $\Hc(f)=0$.

È un fatto che se $n$ è pari allora esiste $f:S^{2n-1}\to S^n$ tale che $\Hc(f)=\pm 2$, quindi componendo con mappe di vario grado costruiamo nuove mappe $g:S^{2n-1}\to S^n$ con invariante di Hopf pari arbitrario, in particolare $\pi_{2n-1}(S^n)$ è infinito, mostrando perché nel [[4-Teorema di Serre|teorema di Serre]] dobbiamo avere un gruppo infinito in quel grado.