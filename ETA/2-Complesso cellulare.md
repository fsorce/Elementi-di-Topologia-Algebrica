Pongo $C_n(K)=H_n(K^n,K^{n-1})\cong \Z^{\#n\text{-celle}}$ 

SI ha che $\theta_\bullet:H_\bullet(X)\cong H_\bullet(K)$. 
Più precisamente se $k_{n}:H_n(K^n)\to H_n(X)$ e $j_n:H_n(K^n)\to C_n(K)$ allora 
- $j_n$ è iniettiva, 
- $k_n$ è surgettiva, 
- $\imm j_n=Z_n(K)$ 
- $j_n\ii(B_n(K))=\ker k_n$.

$\ul{dim}:$
- Con successione della coppia vedo che $H_i(K^{n})\cong H_i(K^{n-1})$ per $i\neq n,n-1$, quindi $$H_i(K^{i+1})\cong H_i(K^{i+2})\cong\cdots$$Considero le mappe da questi in $H_i(X)$ e vedo che sono anche questi isomorfismi usando il [[1-Lemma sulla compattezza dei supporti delle catene]].
- Costruisci un diagrammone che usa [[2-Omologia di scheletro nulla se supero la dimensione]], [[2-Incollamento di n-celle]] e un po' di giochetti su come composizioni preservano o meno nuclei, immagini e surgettività.

Segue che se $K^{n}=K^{n-1}$ allora $H_n(X)=0$ e che se $X$ ha un numero finito di $n$-celle allora $H_n(X)$ è finitamente generato ($C_n(K)$ libero finitamente generato implica che $Z_n(K)$ è libero finitamente generato).

Nota che se $f:X\to Y$ è cellulare, $f_\ast:H_n(X)\to H_n(Y)$, $\vp_\ast:H_n(K)\to H_n(L)$ allora $\theta_n\circ f_\ast=\theta_n\circ \vp_n$ (_impila i diagrammi che definiscono ciò che induce $\theta$ per i due spazi e vedi che commuta_).
