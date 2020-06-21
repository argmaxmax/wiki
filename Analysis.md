##### Definition: Agebraic Interior Point
Let $X$ be an $\mathbb R$-Vectorspace, and $M\subseteq X$.
Then $x\in M$ is called an algebraic interior point of $M$ if $\forall y \in M$ there is some $\varepsilon  \gt 0$ such that $x+ty \in M$ $\forall  t \in (-\varepsilon , \varepsilon)$.

##### Remark:
If $X$ is a normed space and $x \in \mathring{M}$, then $x$ is an algebraic interior point.
In fact, this the case for any topological vector space.

##### Theorem:
Let $X$ be an $\mathbb R$-Vectorspace, $C\subseteqX$ convex with an algebraic interior point.  
Then there exists some functional $F\in X'$ such that $$ F(x)\ge F(z) \quad \forall z\in C $$ 
and $$ F(x) \gt f(z) \quad \text{$\forall $ algebraic interior points of C}. $$ 

##### Proof. 
Translation of Problem: Wlog $0\in C$ is an algebraic interior point of $C$. (By Convexity stability under affine transformations.)  
Then define $p : X \to \mathbb R$ by $$ p(x) = \inf \left\{ t \gt 0 \mid \frac{x}{t}\in C \right\}  $$  
Then $p$ is a sublinear functional.
###### Proof: 
Homogeneity is obvious. For $x,y \in X$ let $s,t \gt 0$ be such that $\frac{x}{s}\in X,$ $\frac{y}{t} \in c$ and it follows $$ \frac{x+y}{s+t} = \frac{s}{s+t}\frac{x}{s}+ \frac{x}{s+t}\frac{y}{t} $$
which implies $s+t \ge p(x+y)$. Taking the infima over $(s,t)$ satifying $(*)$ yields the subadditivity.  
Set $S := \mathbb  Rx.$ Define $$ f:\begin{cases}S &\to &\mathbb R \\ \lambda x &\mapsto &f(\lambda x):=\lambda p(x)  \end{cases} $$  for $\lambda  \in \mathbb R.$  
By Hahn-Banach $\exists F\in X'$ such that $F|_S =f$ and $F(y) \le  p(y)$ for $\lambda \in X.$  
For $z\in C$ it holds $$ F(z) \le  p(z) \le 1 \le  p(x)=F(x). $$  
For $z \in C$ an algebraic interior point of $C$ it holds $$F(z)\ltF(x)  $$ since $p(z) \lt 1$ for algebraic interior points because $\frac{z}{t}\in C$ for some $t \lt 1$. $\blacksquare$



##### Aufgabe: Man zeige, dass die Beschränktheit eines Operators äquivalent zu $\exists C \gt 0 \ \forall x\in X: \left\lVert Tx \right\rVert \le C \cdot\left\lVert x \right\rVert$ ist.
Details. Aus der Beschränktheit von $T$ folgt das nach Definition anhand von $\sup fg \le \sup f \sup g$. Andersherum kann man die $x=0$ ausschließen und den nichtnegativen Faktor nach links ziehen und die Ungleichung bleibt über das Supremum erhalten. $\blacksquare$


##### Satz: Lipschitz-Stetigkeit beschränkter Operatoren
Sei $T\in B(X,Y)$ ein beschränkter Operator auf normierten $\mathbb K$-Vektorräumen. Dann ist $T$ Lipschitz-stetig.  
Details. Da $\left\lVert Tx \right\rVert \le C\cdot \left\lVert x \right\rVert$ für alle $x\in X$ für ein $C \gt 0$, ist $$ \left\lVert Tx-ty \right\rVert = \left\lVert T(x-y) \right\rVert \le C\cdot\left\lVert x-y \right\rVert  $$ für $x,y\in X. \blacksquare$ 

##### Satz: Vektorräume der Linearformen und Linearen Abbildungen
Seien $X_1,\ldots ,X_p$ $K$-Vektorräume. Dann ist die Menge aller Multilinearformen $\mathcal J^p(X_1,\ldots ,X_p)$ ein Vektorraum. Weiterhin ist $\hom(X_1,X_2)$ ein Vektorraum. Als Spezialfall ist der Dualraum $X^*$ ein Vektorraum. Ist $K=\mathbb K$ so sind die Operatormengen $\mathcal L(X_1,X_2), B(X_1,X_2)$ Vektorräume.

##### Satz:
Seien $X,Y$ normierte Räume und $T\in B(X,Y)$ ein beschränkter Operator. Dann ist die Operatornorm $\left\lVert \cdot  \right\rVert$ eine Norm auf $B(X,Y)$ und es gilt für alle $x\in X:$ $$ \left\lVert Tx \right\rVert \le \left\lVert T \right\rVert\cdot \left\lVert x \right\rVert  $$  
Ist weiterhin $Z$ ein weiterer normierter Raum und $S\in B(Y,Z)$ ein weiterer beschränkter Operator, so gilt für die Komposition: $$ \left\lVert ST \right\rVert \le \left\lVert S \right\rVert \cdot \left\lVert T \right\rVert . $$  
Details. Dadurch dass die Operatornorm $\left\lVert \cdot  \right\rVert$ auf $B(X,Y)$ endlich ist, bildet sie in $\mathbb K$ ab. Die Definitheit folgt daraus, dass die Operatornorm ein Supremum aus nichtnegativen Werten ist, welches also genau dann Null ist wenn jeder dieser Werte null ist, also muss, da der Kern eines Operators immer die Null enthält und der Nenner nichtnegativ ist, $T=0$ sein. Ist $\alpha \in \mathbb K$, so folgt die Absolute Homogenität (für $x\neq 0)$ wegen $$  \frac{\left\lVert \alpha T x \right\rVert }{\left\lVert x \right\rVert } = \left| \alpha  \right| \frac{\left\lVert Tx \right\rVert }{x} $$  aus der positiven Homogenität des Supremums. Weiterhin gilt die Dreiecksgleichung wegen der Additivität des Supremums und $$ \frac{\left\lVert (T+S)x \right\rVert }{\left\lVert x \right\rVert } = \frac{\left\lVert Tx+Sx \right\rVert }{\left\lVert x \right\rVert }\le \frac{\left\lVert Tx \right\rVert }{\left\lVert x \right\rVert }+\frac{\left\lVert Sx \right\rVert }{\left\lVert x \right\rVert } $$   
Die Ungleichung für den Funktionswert folgt direkt aus $$ \frac{\left\lVert Tx \right\rVert}{\left\lVert x \right\rVert }\le \displaystyle \sup_{x\in X\\x\neq  0} \frac{\left\lVert Tx \right\rVert }{\left\lVert x \right\rVert }. $$ 

# Kommentar: 
Ist $p$ positiv homogen, so ist Konvexität äquivalent zur Subadditivität.
## Beweis.
Setze in der Subadditivitätsbedingung für $tx$ und $(1-t)y$ ein.  
Für die Rückrichtung mit $t\neq 0$ ist durch Konvexität die Subadditivität gesichert: $$p\left(t \frac{x}{t} + (1-t) \frac{y}{1-t}\right).\blacksquare$$
