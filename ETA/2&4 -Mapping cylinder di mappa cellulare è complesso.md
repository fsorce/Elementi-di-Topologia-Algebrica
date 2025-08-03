Sia $f:X\to Y$ una [[2&4 -Teorema di approssimazione cellulare|mappa cellulare]] tra [[2-Complessi CW|complessi CW]], allora il suo [[4-Mapping Cylinder|mapping cylinder]] $M_f$ è un complesso CW e possiamo interpretare $X$ come un suo sottocomplesso.

$\ul{dim}:$ $X\times I$ e $Y$ hanno una immediata struttura di complessi CW (le $n$-celle di $X\times I$ sono della forma $e^n\times \cpa{0}$, $e^n\times \cpa1$ o $e^{n-1}\times (0,1)$).

Definiamo la struttura in ogni dimensione:
$n=0$) Prendiamo le $0$-celle di $X$ e di $Y$, dove $X$ è visto come $X\times \cpa1$. (Poiché $f$ è cellulare non serve aggiungere le $0$-celle di $X\times \cpa0$ in quanto sono identificate con celle di $Y$).
$n>0$) Costruiamo $M_f^n$ [[2-Incollamento di n-celle|incollando]] le seguenti celle a $M^{n-1}_f$:
- le $n$-celle di $Y$
- le $n$-celle di $X\times \cpa1$
- i prodotti tra le $(n-1)$-celle di $X$ e $(0,1)$
Le immagini dei dischi aperti vengono mappati omeomorficamente perché sono interamente contenute in $X\times I$ o in $Y$, che sono già complessi. I bordi delle celle in $Y$ e di quelle in $X\times\cpa 1$ continuano a vivere in $Y$ e $X\times\cpa 1$ (nei rispettivi $(n-1)$-scheletri per l'esattezza, quindi appartengono già a $M^{n-1}_f$), le celle della forma $e^{n-1}\times (0,1)$ hanno come bordo $e^{n-1}\times \cpa{1}\cup e^{n-1}\times \cpa{0}\cup \del e^{n-1}\times (0,1)$, il primo pezzo appartiene all'$(n-1)$-scheletro di $X\times \cpa1$, il secondo a quello di $Y$ (perché $f$ è cellulare) e il terzo a $X^{n-2}\times (0,1)\subseteq M^{n-1}_f$.