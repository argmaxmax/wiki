## Topologische Strukturen

###### [Definition: Topologischer Raum](def-topologischer-raum)

###### [Definition: Metrischer Raum](def- metrischer-raum)
###### [Definition: Normierter Raum](def-normierter-raum)

###### [Definition: Halbnormierter Raum](def-halbnormierter-raum)
###### Beispiel Metrischer Raum: Normierter Raum
Sei $(X, \left\lVert \cdot  \right\rVert )$ ein normierter Raum. Dann ist $d(x,y) = \left\lVert x -y \right\rVert$ eine Metrik auf $X.$

###### Beispiel Metrischer Raum: Diskreter Raum
Die Abbildung $d(x,y) = 1 - \delta_{xy}$ ist eine Metrik auf einer beliebigen Menge $X.$

###### [Definition: Stetigkeit in topologischen Räumen](def-stetigkeit-topologische-räume)
###### [Definition: Stetigkeit in metrischen Räumen](def-stetigkeit-metrische-räume)
###### [Definition: Stetigkeit in normierten Räumen](def-stetigkeit-normierte-räume)

###### Satz: Stetigkeitskriterien in metrischen Räumen

Eine Abbildung $f \colon X \longrightarrow Y$ auf metrischen Räumen $(X,d_X), \ (Y, d_Y)$ ist genau dann stetig, wenn:
$$\mathop{\forall}\limits_{\varepsilon \gt 0} \mathop{\exists}\limits_{ \delta \gt 0} : d_X(x, y) \lt \delta \implies d_Y(f(x), f(y)) \lt \varepsilon $$

###### Beispiel

Die Identität $\operatorname{id}: X\to X$ auf einem topologischen Raum $X$ ist wegen $\operatorname{id}^{-1}(U) = U$ immer eine stetige Selbstabbildung auf einem topologischen Raum.

- Für jedes $c \in Y$ ist die konstante Funktion $f:\begin{cases}X &\to & Y \\ x &\mapsto &c \end{cases}$ zwischen topologischen Räumen $X,Y$ stetig, denn $f^{-1}(U) = \begin{cases}X, & c \in U\\ \emptyset, & c \not \in U\end{cases}$ ist offen für alle (offenen) $U\subseteq Y$.

- Jede Polynomfunktion $f:\begin{cases}X &\to &X \\ x &\mapsto &\displaystyle\sum_{k=0}^{n}x^k  \end{cases}$ auf einem bewerteten Körper $(X, \left| \cdot  \right| )$ ist eine stetige Selbstabbildung, denn dieser ist ein metrischer Raum mit der Metrik $d(x,y) = |x-y|$, und in einem metrischen Raum ist eine folgenstetige Abbildung stetig. Da Produkte und Summen konvergenter Folgen in bewerteten Körpern wiederum konvergent sind mit dem entsprechendem Grenzwert, gilt abschließend für jede konvergente Folge $(x_n) \subseteq X, \ x_n \to \overline{x}$ dass $f(x_n) \to f(\overline{x})$.
  Als Fortsetzung dieser Betrachtung sind allgemeiner rationale Funktionen auf bewerteten Körpern stetig.

- Das Signum ist auf den reellen Zahlen unstetig genau in der Null.
- Die charakteristische Funktion $\chi  _ \mathbb Q \colon \mathbb R\longrightarrow \{0,1\}$, $x \longmapsto \begin{cases} 1 &;& \text{if } x \in \mathbb Q \\\ 0 &:& \text{sonst.}\end{cases}$ ist auf den reellen Zahlen überall unstetig.


------
------


###### Satz: Zwischenwertsatz
Sei $f \colon [a,b] \to \mathbb{R}$ stetig, $f(a) \neq  f(b)$. Dann gibt es zu jedem Wert $c \in  \left( \min \left\{ f(a), f(b) \right\}, \ \ \max\left\{ f(a), f(b) \right\}  \right)$ ein Urbild $x_0 \in f^{-1}(c)$, also mit $f(x_0) =c.$
  Insbesondere gilt $f \left( \sup \left\{ f \lt c \right\}   \right) = c.$
  **Beweis.** Wir wählen eine Folge $(x_n) \subseteq \left\{ f \lt c \right\}, \ x_n \to x_* :=\sup \left\{ f \lt c \right\}$. Das Supremum existiert aufgrund der Beschränktheit und Nichtleerheit von $M$, da $\mathbb{R}$ vollständig ist. Das Supremum einer Menge ist immer ein Grenzwert einer Folge aus der Menge. Aus $f(x_n) \lt c$ und der Folgenstetigkeit von $f$ folgt $f(x_*) \le c \lt f(b).$ Weiterhin ist für ein hinreichend großes $n$, $x_* + \frac{1}{n} \in \operatorname{dom}f$ aber nicht in $\left\{ f \lt c \right\}$ und somit folgt der Satz nach Grenzübergang aus $f(x_* +\frac{1}{n}) \ge c$. $\qquad\blacksquare$


------
------


###### Satz: Umkehrfunktion einer stetigen streng monotonen Funktion

Sei $f: [a,b] \longrightarrow \mathbb  R$ stetig und streng monoton. Dann ist $f$ bijektiv und existiert die Umkehrabbildung $f^{-1}$, welche selbst stetig ist.


###### Definition: Lipschitzstetigkeit
Eine Abbildung $f : X \to Y$ zwischen metrischen Räumen $(X,d_X), (Y,d_Y)$ heißt Lipschitzstetig, falls es $L\in \mathbb R$ gibt (genannt Lipschitzkonstante), sodass für alle $x,y \in X$ gilt:
$$d_Y\left( f(x),f(y) \right) \le L\cdot d_X\left( x,y \right) .$$

$\mathbb K$
j


###### Satz: Kriterium für schwache Konvergenz in normierten Räumen

Sei $x\in X$ ein Element eines normierten Raums und $(x_n)\subseteq X$ eine Folge in $X$. Dann sind äquivalent:
1. $(x_n)$ ist beschränkt (also $\sup_{n\in N}\left\lVert x_n \right\rVert \lt \infty$) und $\exists D\subseteq X^*, \ \overline{D}=X^*$ (Existenz einer dichten Teilmenge)
1. $x_n \rightharpoonup x$





###### Satz: Nichtleere schwach offene Mengen in unendlichdimensionalen normierten Räumen
2. Aufgabe: Sei $X$ ein unendlichdimensionaler normierter Raum.
   (a) Man zeige dass eine nichtleere schwach offene Menge $U\in \sigma (X,X^*)$ einen affinen Unterraum enthält, also $\forall x \in U \ \exists  y\in X\setminus \left\{ \emptyset \right\}\ \forall \lambda \in \mathbb R  : x+\lambda y \in U$

###### Definition: Folgenkompakter topologischer Raum, folgekompakte Teilmenge
Ein topologischer Raum $\left( X, \mathcal{T} \right)$ heißt folgenkompakt, wenn jede Folge $x \in$

###### Definition: Offene Menge in einem topologischen Raum
Eine Teilmenge $U \subseteq X$ eines metrischen Raums $\left( X,d  \right)$ heißt offen, wenn für jeden Punkt $x \in U$ ein Radius $r > 0$ existiert, sodass die offene Kugel $B_r(x)$ in $U$ enthalten ist: $B_r(x) \subseteq U.$

###### Satz: Die Offene Kugel ist offen
Sei $\left( X,d \right)$ ein metrischer Raum, $r > 0, \ x\in X$. Dann ist $B_r(x)$ offen.
Beweis: Für $y\in B_r(x)$ beliebig  gilt $d(x,y) \lt r$ also $\varepsilon := r-d(x,y) > 0$. Damit gilt
$$\mathop{\forall}\limits _ {\substack{z \in X}} d(z,y) \lt \varepsilon \implies d(z,x) \lt r$$
was abschließend $B_\varepsilon(y) \subseteq B_r(x)$ und den Satz impliziert. $\blacksquare$

###### Satz: Offene Mengen sind Vereinigungen
Eine Teilmenge $U \subseteq X$ eines metrischen Raums $\left( X,d \right)$ ist genau dann offen, wenn $U$ Vereinigung offener Bälle $B_r(x)$ mit $x \in X, \ r > 0$ ist.

###### Definition: Durchmesser eines metrischen Raums/einer Teilmenge eines metrischen Raums
Der Durchmesser eines metrischen Raums $\left( X,d \right)$ ist definiert als das Supremum des Bildes der Metrik:
$$\operatorname{diam}(X) := \sup_{x,y \in X} d(x,y)= \sup\operatorname{im}d$$
Der Durchmesser einer Teilmenge $M \subseteq X$ ist definiert als der Durchmesser des induzierten metrischen Teilraums.


###### Definition: Beschränkter metrischer Raum/beschränkte Teilmenge eines metrischen Raums
Ein metrischer Raum $\left( X,d \right)$ heißt beschränkt, falls $X$ einen endlichen Durchmesser hat:
$$\operatorname{diam}X \lt \infty.$$
Eine Teilmenge $M \subseteq X$ eines metrischen Raums $\left( X,d  \right)$ heißt beschränkt, falls der induzierte metrische Teilraum beschränkt ist.


###### Definition: Beschränkte Abbildung

Eine Abbildung $f : X \to Y$ auf einer beliebigen Menge $X$ in einen metrischen Raum $\left( Y,d \right)$ heißt beschränkt, falls das Bild $\operatorname{ im } f$ ein beschränkter metrischer Teilraum von $Y$ ist, also das Bild endlichen Durchmesser hat:
$$\operatorname{diam}\operatorname{im}f= \sup _{x,y \in \operatorname{im} f} d(x,y) = \sup _{x,y \in X} d\left( f(x), f(y) \right)  \lt \infty $$



###### Definition: Beschränkter normierter Raum/beschränkte Teilmenge eines normierten Raums
Ein normierter Raum $\left( X, \left\lVert \cdot  \right\rVert \right)$ heißt beschränkt, wenn
$$\mathop{\exists}\limits _ {\substack{c \in \mathbb R}} \mathop{\forall}\limits _ {\substack{x \in X}} \left\lVert x \right\rVert \le c$$
Dazu äquivalent ist, dass der induzierte metrische Raum beschränkt ist.
Eine Teilmenge $M \subseteq X$ eines normierten Raums $X$ heißt beschränkt, wenn der Teilraum $M$ des von $X$ induzierten metrischen Raums $\left( X, d_{\left\lVert \cdot  \right\rVert } \right)$ beschränkt ist.


###### Satz: Mengenverhältnisse der offenen, abgeschlossenen Kugeln und dem Abschluss der offenen Kugel in metrischen und normierten Räumen
Sei $\left( X,d \right)$ ein metrischer Raum, $r > 0, \ x \in X$ beliebig.  Dann gelten die folgenden Inklusionen, welche auch echt sein können:
$$B_r(x) \subseteq \overline{B}_r(x)\subseteq \overline{B_r(x)}	.$$
Ist $X$ normierbar, so ist
$$\overline{B}_r(x) = \overline{B_r(x)}.$$
In normierten Räumen koinzidieren also die abgeschlossene Kugel und der Abschluss der offenen Kugel, in metrischen Räumen im Allgemeinen jedoch nicht.

###### Beispiel(Topologie): Coendliche Topologie
Durch $\mathcal T = \left\{ U \subseteq X \mid U =\emptyset \lor \left| U^\complement \right| \lt \infty \right\}$ ist eine Topologie auf jeder beliebigen Menge $X$ definiert, genannt Coendliche Topologie.


###### Beispiel(Topologie): Triviale Topologie
Sei $X$ eine beliebige Menge. Dann ist durch $\left\{ \emptyset, X \right\}$ eine Topologie auf $X$ definiert, genannt triviale oder indiskrete Topologie.


###### Satz: Uneindeutigkeit der metrisierbaren Topologie
Sei $\left( X, \mathcal T \right)$ ein metrisierbarer topologischer Raum. Dann ist im Allgemeinen die induzierende Metrik nicht eindeutig bestimmt.


###### Satz: Nichtmetrisierbarkeit der Trivialtopologie
Sei $X$ eine mindestens zweipunktige Menge versehen mit der Trivialtopologie $\mathcal T$. Dann ist $\mathcal T$ nicht metrisierbar.
Beweis: Angenommen $d$ metrisiere $\left( X, \mathcal{T}  \right)$. Seien $x,y \in X, \ x\neq y, \ r:= d(x,y) > 0$. Im Widerspruch zur Annahme ist die Umgebung $B_{\frac{r}{2}}(x)\not\owns y$ offen. $\blacksquare$

###### Satz: Eigenschaften  des Systems abgeschlossener Mengen in einem topologischen Raums
Sei $\left( X, \mathcal{ T} \right)$ ein topologischer Raum, $\mathcal{A}$ das System der abgeschlossenen Mengen.
Dann ist $\emptyset, X \in \mathcal{  A  }$ und $\mathcal{A}$ ist endlich vereinigungsstabil und beliebig schnittstabil.

###### Definition: Basis einer Topologie
Eine Familie offener Mengen $\left( U_i \right)_{i \in I}\subseteq \mathcal{T}$ in einem topologischen Raum $\left( X, \mathcal{T} \right)$ heißt Basis der Topologie $\mathcal{T}$, wenn jede offene Menge $U \subseteq \mathcal{T}$ eine Darstellung als Vereinigung $U = \bigcup_{i \in J \subseteq I} U_i$ aus Basiselementen hat.

###### Satz: Kanonische Basis der metrisierbaren Topologie
Für einen metrischen Raum $\left( X, d \right)$ ist die Familie der offenen Bälle $\left( B_r(x) \right)_{\substack{r > 0 \\ x \in X}}$ eine Basis der induzierten Topologie.

###### Definition: Topologische Hülle/Abschluss
Der Abschluss $\overline{M}$ einer Teilmenge $M \subseteq \mathcal T$ eines topologischen Raums $\left( X, \mathcal T \right)$ ist definiert als der Schnitt aller $M$ enthaltenden abgeschlossenen Mengen:
$$\overline{M} := \bigcap_{\substack{A \supseteq M \\ A \text{ closed }}} A.$$

###### Definition: Topologischer Kern/Inners
Das Innere $M^\circ$ einer Teilmenge $M \subseteq X$ eines topologischen Raums $\left( X, \mathcal{ T} \right)$ ist definiert als die Vereinigung aller in $M$ enthaltenen offenen Mengen:
$$M^\circ := \bigcup_{\substack{U \subseteq M \\ U \in \mathcal{T}}} U.$$

###### Satz: Abgeschlossenheit der abgeschlossenen Kugel
Die abgeschlossene Kugel $\overline{B}_r(x)$ ist einem metrischen Raum abgeschlossen.

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
[Definition: Operator](defOperator)
Eine lineare Abbildung $T: X \to Y$ auf $\mathbb K$-Vektorräumen $X,Y$ heißt Operator.

##### Definition: Operatornorm
Seien $X,Y$ normierte Räume. Die Abbildung $$ \left\lVert \cdot \right\rVert :\begin{cases} \mathcal L(X,Y) &\to &[0,\infty] \\ T &\mapsto & \left\lVert T \right\rVert :=\displaystyle \sup _{x\in X\\x\neq 0}\frac{\left\lVert Tx \right\rVert }{\left\lVert x \right\rVert }\end{cases} $$ heißt Operatornorm auf $\mathcal L(X,Y)$.

##### Definition: Beschränkter Operator
Ein Operator $T\in\mathcal L (X,Y)$ heißt beschränkt, wenn die Operatornorm $\left\lVert T \right\rVert$ endlich ist.
Es bezeichne $B(X,Y)$ die Menge aller beschränkten Operatoren, und im Fall $X=Y$ sei es $B(X).$

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

[Vorlesung 19](vo19.md)
[Funktionale und Operatoren](Funktionale und Operatoren)


# Intitialtopologie

- Definition:  Sei $\left\{ f_i :X\to X_i \right\}_{i\in I}$ eine Familie von Abbildungen, wobei $X$ eine beliebige Menge ist und $\left( X_i, \mathcal T \right) _{i\in I}$ eine Familie von topologischen Räumen ist. 
