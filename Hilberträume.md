Satz: Cauchy-Schwarz-Ungleichung in Prähilberträumen
Sei $(X, \left<\cdot, \cdot  \right>)$ ein Prähilbertraum.
Dann gilt
$$\mathop{\forall}\limits _ {\substack{x,y \in X}} \left| \left\langle x,y \right\rangle  \right| \le \left\lVert x \right\rVert \cdot \left\lVert y \right\rVert$$
beziehungsweise
$$\left\lvert \left\langle x, y \right\rangle  \right\rvert ^2 \le \left\langle x, x \right\rangle \left\langle y,y \right\rangle, $$
mit Gleichheit genau dann, wenn $x,y$ linear abhängig sind.


Definition: Folgenkompakter topologischer Raum, folgekompakte Teilmenge
Ein topologischer Raum $\left( X, \mathcal{T} \right)$ heißt folgenkompakt, wenn jede Folge $x \in$

Definition: Offene Menge in einem topologischen Raum
Eine Teilmenge $U \subseteq X$ eines metrischen Raums $\left( X,d  \right)$ heißt offen, wenn für jeden Punkt $x \in U$ ein Radius $r > 0$ existiert, sodass die offene Kugel $B_r(x)$ in $U$ enthalten ist: $B_r(x) \subseteq U.$

Satz: Die Offene Kugel ist offen
Sei $\left( X,d \right)$ ein metrischer Raum, $r > 0, \ x\in X$. Dann ist $B_r(x)$ offen.
Beweis: Für $y\in B_r(x)$ beliebig  gilt $d(x,y) \lt r$ also $\varepsilon := r-d(x,y) > 0$. Damit gilt
$$\mathop{\forall}\limits _ {\substack{z \in X}} d(z,y) \lt \varepsilon \implies d(z,x) \lt r$$
was abschließend $B_\varepsilon(y) \subseteq B_r(x)$ und den Satz impliziert. $\blacksquare$

Satz: Offene Mengen sind Vereinigungen
Eine Teilmenge $U \subseteq X$ eines metrischen Raums $\left( X,d \right)$ ist genau dann offen, wenn $U$ Vereinigung offener Bälle $B_r(x)$ mit $x \in X, \ r > 0$ ist.

Definition: Durchmesser eines metrischen Raums/einer Teilmenge eines metrischen Raums
Der Durchmesser eines metrischen Raums $\left( X,d \right)$ ist definiert als das Supremum des Bildes der Metrik:
$$\operatorname{diam}(X) := \sup_{x,y \in X} d(x,y)= \sup\operatorname{im}d$$
Der Durchmesser einer Teilmenge $M \subseteq X$ ist definiert als der Durchmesser des induzierten metrischen Teilraums.


Definition: Beschränkter metrischer Raum/beschränkte Teilmenge eines metrischen Raums
Ein metrischer Raum $\left( X,d \right)$ heißt beschränkt, falls $X$ einen endlichen Durchmesser hat:
$$\operatorname{diam}X \lt \infty.$$
Eine Teilmenge $M \subseteq X$ eines metrischen Raums $\left( X,d  \right)$ heißt beschränkt, falls der induzierte metrische Teilraum beschränkt ist.

Definition: Beschränkte Abbildung
Eine Abbildung $f : X \to Y$ auf einer beliebigen Menge $X$ in einen metrischen Raum $\left( Y,d \right)$ heißt beschränkt, falls das Bild $\operatorname{ im } f$ ein beschränkter metrischer Teilraum von $Y$ ist, also das Bild endlichen Durchmesser hat:
$$\operatorname{diam}\operatorname{im}f= \sup _{x,y \in \operatorname{im} f} d(x,y) = \sup _{x,y \in X} d\left( f(x), f(y) \right)  \lt \infty $$

Definition: Beschränkter normierter Raum/beschränkte Teilmenge eines normierten Raums
Ein normierter Raum $\left( X, \left\lVert \cdot  \right\rVert \right)$ heißt beschränkt, wenn
$$\mathop{\exists}\limits _ {\substack{c \in \mathbb R}} \mathop{\forall}\limits _ {\substack{x \in X}} \left\lVert x \right\rVert \le c$$
Dazu äquivalent ist, dass der induzierte metrische Raum beschränkt ist.
Eine Teilmenge $M \subseteq X$ eines normierten Raums $X$ heißt beschränkt, wenn der Teilraum $M$ des von $X$ induzierten metrischen Raums $\left( X, d_{\left\lVert \cdot  \right\rVert } \right)$ beschränkt ist.


Satz: Mengenverhältnisse der offenen, abgeschlossenen Kugeln und dem Abschluss der offenen Kugel in metrischen und normierten Räumen
Sei $\left( X,d \right)$ ein metrischer Raum, $r > 0, \ x \in X$ beliebig.  Dann gelten die folgenden Inklusionen, welche auch echt sein können:
$$B_r(x) \subseteq \overline{B}_r(x)\subseteq \overline{B_r(x)}	.$$
Ist $X$ normierbar, so ist
$$\overline{B}_r(x) = \overline{B_r(x)}.$$
In normierten Räumen koinzidieren also die abgeschlossene Kugel und der Abschluss der offenen Kugel, in metrischen Räumen im Allgemeinen jedoch nicht.

Beispiel(Topologie): Coendliche Topologie
Durch $\mathcal T = \left\{ U \subseteq X \mid U =\emptyset \lor \left| U^\complement \right| \lt \infty \right\}$ ist eine Topologie auf jeder beliebigen Menge $X$ definiert, genannt Coendliche Topologie.


Beispiel(Topologie): Triviale Topologie
Sei $X$ eine beliebige Menge. Dann ist durch $\left\{ \emptyset, X \right\}$ eine Topologie auf $X$ definiert, genannt triviale oder indiskrete Topologie.


Satz: Uneindeutigkeit der metrisierbaren Topologie
Sei $\left( X, \mathcal T \right)$ ein metrisierbarer topologischer Raum. Dann ist im Allgemeinen die induzierende Metrik nicht eindeutig bestimmt.


Satz: Nichtmetrisierbarkeit der Trivialtopologie
Sei $X$ eine mindestens zweipunktige Menge versehen mit der Trivialtopologie $\mathcal T$. Dann ist $\mathcal T$ nicht metrisierbar.
Beweis: Angenommen $d$ metrisiere $\left( X, \mathcal{T}  \right)$. Seien $x,y \in X, \ x\neq y, \ r:= d(x,y) > 0$. Im Widerspruch zur Annahme ist die Umgebung $B_{\frac{r}{2}}(x)\not\owns y$ offen. $\blacksquare$

Satz: Eigenschaften  des Systems abgeschlossener Mengen in einem topologischen Raums
Sei $\left( X, \mathcal{ T} \right)$ ein topologischer Raum, $\mathcal{A}$ das System der abgeschlossenen Mengen.
Dann ist $\emptyset, X \in \mathcal{  A  }$ und $\mathcal{A}$ ist endlich vereinigungsstabil und beliebig schnittstabil.

Definition: Basis einer Topologie
Eine Familie offener Mengen $\left( U_i \right)_{i \in I}\subseteq \mathcal{T}$ in einem topologischen Raum $\left( X, \mathcal{T} \right)$ heißt Basis der Topologie $\mathcal{T}$, wenn jede offene Menge $U \subseteq \mathcal{T}$ eine Darstellung als Vereinigung $U = \bigcup_{i \in J \subseteq I} U_i$ aus Basiselementen hat.

Satz: Kanonische Basis der metrisierbaren Topologie
Für einen metrischen Raum $\left( X, d \right)$ ist die Familie der offenen Bälle $\left( B_r(x) \right)_{\substack{r > 0 \\ x \in X}}$ eine Basis der induzierten Topologie.

Definition: Abschluss
Der Abschluss $\overline{M}$ einer Teilmenge $M \subseteq \mathcal T$ eines topologischen Raums $\left( X, \mathcal T \right)$ ist definiert als der Schnitt aller $M$ enthaltenden abgeschlossenen Mengen:
$$\overline{M} := \bigcap_{\substack{A \supseteq M \\ A \text{ closed }}} A.$$

Definition: Topologischer Kern/Inners
Das Innere $M^\circ$ einer Teilmenge $M \subseteq X$ eines topologischen Raums $\left( X, \mathcal{ T} \right)$ ist definiert als die Vereinigung aller in $M$ enthaltenen offenen Mengen:
$$M^\circ := \bigcup_{\substack{U \subseteq M \\ U \in \mathcal{T}}} U.$$

Satz: Abgeschlossenheit der abgeschlossenen Kugel
Die abgeschlossene Kugel $\overline{B}_r(x)$ ist einem metrischen Raum abgeschlossen.

[A2B1](A2B1)


Beispiel (Dualbasis): Dualbasis des Standardraums
Im physikalischen Standardraum $X= \mathbb K^3$ ist $e =(e_1,\ldots , e_3)$ eine geordnete Basis, und es gilt für die Dualbasis: 

$$ e_1^*\left( \begin{pmatrix} 1\\ \vdots\\ 3 \end{pmatrix} \right) = 1 \\ e_2^* \left( \cdot  \right)= 2 \\ e_3^*\left( \cdot  \right) = 3. $$

Im  Reellen Polynomraum $X= \mathbb{R}[X]$ ist $\left( X^0, X^1, \ldots  \right)$ eine geordnete Basis und es gilt für den Vektor $p=2+3X^2$: $$\left( X^0 \right) ^*= 2 \\ \left( X^1 \right) ^* = 0 \\ \left( X^2 \right) ^* = 3 \\ \left( X^3 \right) ^* = 0 \\ \vdots $$

[Satz: Dualbasis und Delta](Satz-Dualbasis_und_Delta)
[Satz: Dualbasis des Dualraums](Satz-Dualbasis_des_Dualraums)

[Definition: Absorbierende Teilmenge eines Vektorraums](def-Absorbierende_Teilmenge_eines_Vektorraums)  
[Beispiel(Algebra): Beschränkte Operatoren](Beispiel_Algebra-Beschränkte_Operatoren)  

[Definition: Isometrie](def-Isometrie)  

[Definition: Resolvente](def-Resolvente)  


[beispiel](beispiel)
