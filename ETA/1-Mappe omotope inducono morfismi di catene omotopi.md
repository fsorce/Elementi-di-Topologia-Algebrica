Una contrazione per deformazione $h:X\times I\to X$ induce un morfismo omotopo a $\e_\bullet$ dato da $$\e_n=\begin{cases}0 &\text{se }n>0\\ \sum n_\sigma\sigma\mapsto\pa{\sum n_\sigma}\sigma_0 &\text{se }n=0\end{cases}$$dove $\sigma_0:\Delta^0\to\cpa{x_0}$ per $x_0$ retratto di deformazione di $X$. Segue che $H_\bullet(X)=\Z[0]$.

---
Se $\eta_0,\eta_1:X\to X\times I$ sono le immersioni per $t=0$ e $t=1$ esiste una omotopia di catene naturale tra $(\eta_0)_\#$ e $(\eta_1)_\#$ (usa il [[1-Teorema dei funtori liberi-aciclici]]).

Grazie a questo lemma possiamo mostrare che mappe omotope inducono morfismi di catene omotopi, infatti$$f_i=H\circ \eta_i\implies (f_1)_\#-(f_0)_\#=H_\#\circ ((\eta_1)_\#-(\eta_0)_\#).$$