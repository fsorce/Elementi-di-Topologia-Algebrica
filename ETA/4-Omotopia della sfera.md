Poiché $\R\to S^1$ è un rivestimento si ha per la [[4-Omotopia di fibre|successione delle fibre]]$$\to\pi_n(\Z)\to\pi_n(\R)\to\pi_{n}(S^1)\to \pi_{n-1}(\Z)\to$$dove i $\pi_n(\Z)$ sono nulli per $n\geq 1$ in quanto $\Z$ è un insieme discreto. Segue che $\pi_n(S^1)=0$ per ogni $n\geq2$.
Sono anche noti per altre vie $\pi_1(S^1)=\Z$ e $\pi_0(S^1)=0$.

Grazie all'[[4-Isomorfismo di Freudenthal|isomorfismo di Freudenthal]] sappiamo che$$\Z=\pi_1(S^1)\to\pi_2(S^2)\cong \pi_3(S^3)\cong\pi_4(S^4)\cong\cdots$$dove la prima mappa è surgettiva. Per concludere che $\pi_n(S^n)=\Z$ basta mostrare che $\pi_2(S^2)$ non è un gruppo finito (la prima surgettività mostra già che è ciclico). Ma questo segue notando che se $f\in [S^2,S^2]^0$ allora è ben definito il suo grado come $f_\ast:H_2(S^2)\to H_2(S^2)$ e ci sono tali mappe per infiniti gradi distinti.

Mostriamo che per $i<n$, $\pi_i(S^n)=0$ (la sfera è [[4-Spazi n-connessi|(n-1)-connessa]])
$\ul{dim}:$ Per $n=1,2$ la tesi è nota.
Siano $E^n_+$ ed $E^n_-$ i due emisferi di $S^n$, che trattiamo come aperti ai fini dell'omologia in quanto retrazioni di un loro intorno.
Sviluppando le [[4-Successione lunga in omotopia|successioni]] delle coppie $(S^n,E^n_-)$ e $(E^{n+1}_+,S^{n})$ ricaviamo che per $i>0$ $\pi_i(S^n)\cong \pi_i(S^n,E^n_-)$ e $\pi_i(E^{n+1}_-,S^n)\cong \pi_i(E^{n+1}_+,S^n)\cong \pi_{i-1}(S^n)$.
Per ipotesi induttiva i gruppi della seconda serie sono nulli per $i\leq n$.
Applicando [[4-Escissione in omotopia|escissione]] si ha che$$\pi_{i-1}(S^n)\cong \pi_{i}(E^{n+1}_+,S^n)\overset{esc}\cong \pi_{i}(S^{n+1},E^{n+1}_-)\cong \pi_{i}(S^{n+1})$$per $0<i<n+1+n+1-2=2n$ ($p=q=n+1$). Poiché $n\geq 2$ si ha che $2n>n$ e quindi per $0<i\leq n$ l'isomorfismo vale. Applicando l'ipotesi induttiva abbiamo trovato la tesi per $S^{n+1}$ eccetto che nel caso $i=0$, ma è evidente che $\pi_0(S^{n+1})=0$.