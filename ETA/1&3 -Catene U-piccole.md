Considera $\Uc$ ricoprimento tale che $X=\bigcup_{U\in \Uc}\rg U$. Ha senso definire le catene $\Uc$-piccole come il generato dai simplessi con immagine contenuta in un elemento di $\Uc$.

Nota che per ogni simplesso $\sigma$ esiste $k$ tale che la [[1-Suddivisione baricentrica]] $B^k(\sigma)$ è tale che ogni simplesso che lo costituisce è contenuto in un elemento di $\Uc$, cioè $B^k(\sigma)\in C^\Uc(X)$ definitivamente.
(_basta suddividere finché il diametro dei singoli simplessi non supera il numero di Lebesgue di $\Uc\cap \imm\sigma$_)

Il risultato principale sulle catene $\Uc$-piccole è che $H^\Uc_\bullet(X)= H_\bullet(X)$ tramite la mappa indotta dall'inclusione dei complessi.
$\ul{dim}:$ Ricordando che la [[1-Suddivisione baricentrica|suddivisione baricentrica è omotopa all'identità]], sia $T_k$ l'omotopia tra $id$ e $B^k$.
Iniettiva: sia $a\in Z^\Uc(X)$ tale che $a=\del b$ in $C(X)$. Notiamo che $$b-B^k(b)=\del T_kb-T_ka\implies a-\del B^k(b)=-\del T_ka$$$$\implies a=\del(B^k(b)-T_ka).$$Per ipotesi $B^k(b)\in C^\Uc(X)$ e, poiché $a\in C^\Uc(X)$, anche $T_ka\in C^\Uc(X)$ per naturalità dell'omotopia derivante dal [[1-Teorema dei funtori liberi-aciclici]].
Surgettiva: Sia $a\in Z(X)$ e notiamo che $B^k(a)\in Z^\Uc(X)$.$$a-B^ka=\del T_k a-T_k\under{=0}{\del a}\implies [a]=[B^ka].$$

Notiamo che la successione esatta]$$0\to C^\Uc(X)\to C(X)\to \frac{C(X)}{C^\Uc(X)}\to 0$$spezza (possiamo costruire una sezione prendendo rappresentanti), quindi resta esatta applicando $\cdot\otimes G$ e $Hom(\cdot,G)$. Passando in omologia $i_\ast$ è un isomorfismo per quanto detto, quindi $H\pa{\frac{C(X)}{C^\Uc(X)}}=0$, quindi per i [[3-Teorema dei coefficienti universali omologia|teoremi dei coefficienti universali]] troviamo che sono banali anche $$H^\bullet\pa{\frac{C(X)}{C^\Uc(X)};G}\quad\text e\quad H_\bullet\pa{\frac{C(X)}{C^\Uc(X)};G},$$ovvero anche $i\otimes id_G$ e $i^\ast$ inducono isomorfismi.