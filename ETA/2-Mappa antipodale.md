La mappa antipodale $\al:S^n\to S^n$ è la mappa indotta da $-id_{\R^{n+1}}$ ristretta alla sfera.

Ricordando il [[1-Omologia della sfera|complesso cellulare associato alla sfera]], cerchiamo di capire come agisce $\al_\ast$:
Poiché $\al$ è un omeomorfismo, $\al_\ast$ è un isomorfismo e necessariamente manda un generatore $x^i$ di $H_i(D^i_+,S^{i-1})$ in un elemento di $H_i(D^i_-,S^{i-1})$ e viceversa. Segue che $\al_\ast(x^i)$ genera $H_i(D^i_-,S^{i-1})$.

Mostriamo che $d_i(x^i)=\pm(\al_\ast x^{i-1}+(-1)^ix^{i-1})$:
- Mostriamo che generano lo stesso gruppo ciclico. Questo gruppo sarà $\ker d_{i-1}$.
- Ricordo che $d_{i-1}=j_{i-2}\circ \del_\ast$ e che $\al_\ast$ commuta con entrambe queste mappe. Ricordo anche che la mappa antipodale ha [[2-Gradi di mappe tra sfere|grado]] $(-1)^{i-1}$ come mappa da $S^{i-1}$ in sè:$$d_{i-1}\circ \al_\ast=j_{i-2}\circ \al_\ast\circ \del_\ast=j_{i-1}\circ (-1)^{i-1}\circ \del_\ast=(-1)^{i-1}d_{i-1},$$in particolare $\al_\ast x^{i-1}+(-1)^{i}x^{i-1}$ appartiene al gruppo.
- Poiché $H_{i-1}(S^i)=0$ si ha che $\ker d_{i-1}=\imm d_i$, quindi $d_ix^i$ genera $\ker d_i$ (per quanto detto $d_i(\al_\ast x^i)=(-1)^{i}d_ix^i$).
- Sia ora $ax^{i-1}+b\al_\ast x^{i-1}$ un generico ciclo di $H_{i-1}(S^{i-1},S^{i-2})$, cioè$$0=d_{i-1}(ax^{i-1}+b\al_\ast x^{i-1})=ad_{i-1}x^{i-1}+b(-1)^{i-1}d_{i-1}x^{i-1},$$da cio $a(-1)^i=b$, cioè il ciclo di prima si scrive come $a(x^{i-1}+(-1)^i\al_\ast x^{i-1})$.