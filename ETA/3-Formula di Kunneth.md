Siano $C$ e $D$ complessi con $C$ libero. Allora è esatta$$0\to\bigoplus_{i+j=n}H_i(C)\otimes H_j(D)\to H_n(C\otimes D)\to \bigoplus_{i+j=n-1}Tor(H_i(C),H_j(D))\to 0$$inoltre se anche $D$ è libero allora spezza.

$\ul{dim}:$ Poiché $C$ è libero, tensorizzando $0\to Z_\bullet(C)\to C_\bullet\to B_{\bullet-1}(C)\to 0$ con $D$ troviamo la successione esatta$$0\to (Z(C)\otimes D)_n\to (C\otimes D)_n\to (B(C)\otimes D)_{n-1}\to 0$$(_se $i+j=n$ allora tensorizziamo la successione nel grado $i$ con $D_j$_).
Passando in [[1-Omomorfismo di connessione|omologia]] troviamo$$H_n(B(C)\otimes D)\overset{\al_n}\to H_n(Z(C)\otimes D)\to H_n(C\otimes D)\to H_{n-1}(B(C)\otimes D)\overset{\al_{n-1}}\to H_{n-1}(Z(C)\otimes D)$$dove $\al_n$ e $\al_{n-1}$ sono indotte dall'inclusione $B_n\subseteq Z_n$ (come nella dimostrazione dei [[3-Teorema dei coefficienti universali omologia|TCU]]).
Estraiamo la successione esatta corta$$0\to \coker\al_n\to H_n(C\otimes D)\to \ker \al_{n-1}\to 0$$e studiamo gli estremi:
- Poiché $Z(C)$ e $B(C)$ sono liberi si ha che $$\begin{align}
	&\ker(id\otimes\del:(Z(C)\otimes D)_n\to(Z(C)\otimes D)_{n-1})=(Z(C)\otimes Z(D))_n\\
	&\imm(id\otimes\del:(Z(C)\otimes D)_{n+1}\to(Z(C)\otimes D)_{n})=(Z(C)\otimes B(D))_{n}\\
	&\ker(id\otimes\del:(B(C)\otimes D)_n\to(B(C)\otimes D)_{n-1})=(B(C)\otimes Z(D))_n\\
	&\imm(id\otimes\del:(B(C)\otimes D)_{n+1}\to(B(C)\otimes D)_{n})=(B(C)\otimes B(D))_{n}
	\end{align}$$dunque $H(Z(C)\otimes D)\cong Z(C)\otimes H(D)$ e $H(B(C)\otimes D)\cong B(C)\otimes H(D)$.
- Sempre per libertà di $C$, la successione $0\to B(C)\to Z(C)\to H(C)\to 0$ è una risoluzione libera, quindi tensorizzando con $H(D)$ troviamo$$0\to Tor(H(C),H(D))\to B(C)\otimes H(D)\to Z(C)\otimes H(D)\to H(C)\otimes H(D)\to 0$$
- Per quanto detto abbiamo trovato $$0\to Tor(H(C),H(D))\to H(B(C)\otimes D)\overset{\al}\to H(Z(C)\otimes D)\to H(C)\otimes H(D)\to 0$$
Supponiamo ora che $D$ sia libero e mostriamo che spezza la successione trovata. Siano $r:C\to Z(C)$ e $s:D\to Z(D)$ retrazioni. Allora la mappa $$\funcDef{(C\otimes D)_n}{H(C)\otimes H(D)}{c\otimes d}{[r(c)]\otimes [s(d)]}$$è ben definita e manda bordi in zero ($[\del r(c)]\otimes [s(b)]+(-1)^{|c|}[r(c)]\otimes[\del s(c)]=0+0$), quindi induce una mappa $\rho:H_n(C\otimes D)\to H(C)\otimes H(D)$ ed è una retrazione per la mappa sopra per costruzione.