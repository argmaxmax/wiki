# Beispiel (Banachraum): Raum der beschränkten Operatoren
Seien $X,Y$ normierte Räume, $Y$ vollständig. Dann ist der Raum der beschränkten Operatoren $B(X,Y)$ mit der Operatornorm ein Banachraum.
## Beweis.
Sei $(T_n)$ eine Cauchyfolge in $B(X,Y)$ und $x\in X$ beliebig. Dann ist $(T_nx)$ eine Cauchyfolge in $Y$, da $$\left\lVert T_nx -T_mx \right\rVert \le \left\lVert T_n - T_m \right\rVert \cdot \left\lVert x \right\rVert.$$  
Wegen der Vollständigkeit von $Y$ existiert $y\in Y$ sodass $T_nx \to y$ für $n\to \infty$.  
Definiere eine Abbildung $$T:\begin{cases}X &\to &Y \\ x &\mapsto &Tx=\lim_{n \to \infty} T_nx \end{cases}.$$  
Durch die Linearität von $T_n$ für $n\in \mathbb N$ und der Stetigkeit der Vektorraumoperationen gilt für alle $x\in X$: $$\left\lVert Tx-T_nx \right\rVert = \lim_{m \to \infty} \left\lVert T_mx-T_nx \right\rVert \le \lim_{m \to \infty}  \left\lVert T_m-T_n \right\rVert \cdot \left\lVert x \right\rVert .$$  
Weil $(T_n)$ eine Cauchyfolge ist und $$\forall \varepsilon \gt 0\ \exists N \forall  n,m \ge N: \left\lVert T_m-T_n \right\rVert \le \varepsilon$$gilt für alle $x\in X:$ $$\left\lVert Tx - T_Nx \right\rVert \le \varepsilon \left\lVert x \right\rVert $$  
und insgesamt für alle $x\in X:$ $$\left\lVert Tx-T_nx \right\rVert \le \varepsilon \left\lVert x \right\rVert$$  
Weshalb $T-T_N \in B(X,Y)$ ein beschränkter Operator ist.  
Aus der Subadditivität folgt $T\in B(X,Y)$ aus $$\left\lVert T \right\rVert \le \left\lVert T-T_N \right\rVert +\left\lVert T_N \right\rVert \lt \infty.$$  
Und abschließend folgt die Konvergenz durch $$\forall \varepsilon \gt 0 \exists N \ \forall n \ge N \ \forall x\in X: \left\lVert Tx - T_nx \right\rVert \le \varepsilon \left\lVert x \right\rVert $$ zu $\left\lVert T-T_n \right\rVert \to 0.\quad\blacksquare$
