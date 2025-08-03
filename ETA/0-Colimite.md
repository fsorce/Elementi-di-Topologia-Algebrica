Un poset $(\Lambda, \leq)$ è un insieme diretto se per ogni $\al,\beta\in \Lambda$ esiste $\gamma\in \Lambda$ tale che $\al\leq\gamma$ e $\beta\leq \gamma$.
Un sistema diretto di gruppi abeliani $\cpa{A_\la}_{\la\in \Lambda}$ indicizzato da un insieme diretto $(\Lambda,\leq)$ è tale che 
- per ogni $\al\leq \beta$ esiste un morfismo $\vp_{\al,\beta}:A_\al\to A_\beta$
- se $\al\leq \beta\leq \gamma$ allora $\vp_{\al,\gamma}=\vp_{\al,\beta}\circ \vp_{\beta,\gamma}$
- $\vp_{\al,\al}=id_{A_\al}$.

Il limite diretto di un sistema diretto è dato da$$\varinjlim_{\al\in \Lambda}A_\al=\frac{\bigoplus_{\la\in \Lambda}A_\la}{\ps{a_\al-\vp_{\al,\beta}(a_\al)}_{\al\leq \beta}}$$Osserviamo che dato un elemento generico di $\varinjlim A_\al$ possiamo scegliere un singolo $A_\gamma$ che ne contiene un rappresentante (usiamo la definizione di insieme diretto).


Se $\cpa{A_\al}_{\al\in \Lambda}$, $\cpa{B_\al}_{\al\in \Lambda}$ e $\cpa{C_\al}_{\al\in \Lambda}$ sono sistemi diretti indicizzati sullo stesso insieme diretto, la successione$$0\to A_\al\to B_\al\to C_\al\to 0$$è esatta per ogni $\al\in\Lambda$ e applicare le $\vp_{\al,\beta}$ per ogni gruppo fa commutare le due righe esatte per $\al$ e $\beta$ allora è esatta$$0\to \varinjlim A_\al\to \varinjlim B_\al\to \varinjlim C_\al\to 0$$
Da questo segue un analogo per successioni esatte lunghe che otteniamo spezzando$$\cdots\to A_{n-1,\al}\overset{t_{n-1,\al}}\to A_{n,\al}\overset{t_{n,\al}}\to A_{n+1,\al}\to\cdots$$in$$0\to\under{=\imm t_{n-1,\al}}{\ker t_{n,\al}}\to A_{n,\al}\to \under{=\ker t_{n+1,\al}}{\imm t_{n,\al}}\to 0$$