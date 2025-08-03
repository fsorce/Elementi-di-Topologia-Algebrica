Sia $X=A\cup B$. Sono definite le inclusioni$$\begin{align*}&i:A\cap B\to A &j:A\cap B\to B\\&k:A\to X &\ell:B\to X \end{align*}$$e quindi anche le mappe$$\begin{align}&\vp:\funcDef{H(A\cap B)}{H(A)\oplus H(B)}{x}{(i_\ast(x),j_\ast(x))}\\\\
&\psi:\funcDef{H(A)\oplus H(B)}{H(X)}{(u,v)}{k_\ast(u)-\ell_\ast(v)}\end{align}$$
Se $X=\rg A\cup \rg B$ allora esiste $\Delta:H(X)\to H(A\cap B)$ naturale di grado -1 che rende esatta la successione lunga$$\to H_n(A\cap B)\to H_n(A)\oplus H_n(B)\to H_n(X)\to H_{n-1}(A\cap B)\to$$(possiamo prendere le omologie ridotte se $A\cap B\neq \emptyset$).

$\ul{dim}:$ Sia $\Uc=\cpa{A,B}$ e nota che $C^\Uc(X)=C(A)+C(B)$, più precisamente$$0\to C(A\cap B)\to C(A)\oplus C(B)\to C^\Uc(X),$$da cui con [[1-Omomorfismo di connessione|l'omomorfismo di connessione]] e l'uguaglianza [[1&3 -Catene U-piccole|omologia di catene U-piccole e omologia singolare]] troviamo la tesi.

---
Notiamo che le proprietà usate nella dimostrazione [[1&3 -Catene U-piccole|continuano a valere]] anche considerando omologia e coomologia con coefficienti.