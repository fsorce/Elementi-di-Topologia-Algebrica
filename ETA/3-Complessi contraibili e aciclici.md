Un complesso $C_\bullet$ è contraibile se la mappa identità è omotopa alla mappa nulla (in particolare $H_n(C_\bullet)=0$ per ogni $n$).
Un complesso è aciclico se $H_n(C_\bullet)=0$ per ogni $n>0$.

Valgono le seguenti proprietà:
1. Se $C_\bullet$ è contraibile allora $C_\bullet\otimes D_\bullet$ è contraibile
2. Se $X$ è contraibile allora $\wt C_\bullet(X)\otimes\wt C_\bullet(Y)$ è contraibile
3. Se $X$ e $Y$ sono contraibili allora $C_\bullet(X)\otimes C_\bullet(Y)$ è aciclico.
$\ul{dim}:$ Il punto 2 segue immediatamente dal punto 1 notando che se $X$ è contraibile allora $\wt C_\bullet(X)$ è contraibile.

1.) Se $k:C_\bullet\to C_{\bullet+1}$ è l'omotopia tra $id$ e $0$, cioè $id=\del k+k\del$, allora poniamo $$\wt k:\funcDef{(C_\bullet\otimes D_\bullet)_n}{(C_\bullet\otimes D_\bullet)_{n+1}}{\al\otimes \beta}{k(\al)\otimes \beta}$$e notiamo che $$\begin{align}
(\del \wt k+\wt k\del)(\al\otimes \beta)=&\del(k(\al)\otimes \beta)+\wt k(\del \al\otimes \beta+(-1)^{|\al|}\al\otimes \del \beta)=\\
=&\del k\al\otimes\beta+(-1)^{|\al|+1}k\al\otimes \del \beta+\\
&+k\del\al\otimes \beta+(-1)^{|\al|}k\al\otimes\del \beta=\\
=&(\del k+k\del)\al \otimes \beta=\al\otimes \beta.
\end{align}$$3.) Mostriamo che il ==nucleo== della mappa surgettiva$$\wt C_\bullet(X)\otimes\wt C_\bullet(Y)\to C_\bullet(X)\otimes C_\bullet(Y)$$è un complesso ==aciclico shiftato di un grado sotto==. Così facendo passando alla [[1-Omomorfismo di connessione|successione esatta lunga]] ricaveremo che $H_i(C_\bullet(X)\otimes C_\bullet(Y))=H_{\bullet-1}(\ker)$, che è nullo per indici positivi.

Separando i complessi nelle somme dirette $\bigoplus_{i+j=n}\wt C_i(X)\otimes \wt C_j(Y)$ (e similmente per $C_\bullet(X)\otimes C_\bullet(Y)$) notiamo che ==il nucleo è dato da $(\wt{C_\bullet(X)\oplus C_\bullet(Y)})_{\bullet+1}$==

Osserviamo che la seguente successione di complessi$$0\to\Z[-1]\to\wt C_\bullet(X)\oplus\wt C_\bullet(Y)\to\wt{C_\bullet(X)\oplus C_\bullet(Y)}\to 0$$dove la prima mappa in grado $-1$ è $1\mapsto(1,-1)$ e la seconda è la somma è esatta.
Passando all'[[1-Omomorfismo di connessione|esatta lunga]] ricaviamo che $\wt H_\bullet(C_\bullet(X)\oplus C_\bullet(Y))=\Z[0]$, in particolare il terzo complesso è aciclico.
