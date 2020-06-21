# Analysis 
## Analysis 1
### Funktionen
### Zahlen
[Beispiel (Ringendomorphismus): Konjugation](Beispiel_Ringendomorphismus-Konjugation)
### Folgen
### Reihen
### Stetigkeit ### [Exponentiation](Exponentiation) ### Differentiation
### Integration
### Potenzreihen
### Konvexität
### Unendliche Mengen


## Analysis 2
### Normierte Räume
### Kurven
### Partielle Ableitungen
### Differentiation 2
### Taylorentwicklung im Mehrdimensionalen
### Fixpunktsatz von Banach
### Inverse Funktionen im Mehrdimensionalen
### Implizite Funktionen
### Parameterabhängige Integrale
### Integration 2
### Gewöhnliche Differentialgleichungen
### Fourierreihen
### Matrixfunktionen
### Kompaktheit

## Analysis 3
### Mengensysteme
### Inhalte und Maße
### Messbare Abbildungen, Bildmaße
### Maß-Integral
### Nullmengen, Konvergenzsätze
### $L^p$-Räume
### Maße mit Dichten
### Produktmaße, Satz von Fubini
### Kurvenintegrale und Potentiale
### Mannigfaltigkeiten
### Volumenintegrale
### Oberflächenintegrale
### Satz von Gauß
### Satz von Stokes
### Harmonische Funktionen


## Analysis 4
### Topologie
###### Definition: Metrischer Raum
Ein metrischer Raum $(X,d)$ ist eine Menge $X$ mit einer Abbildung $d : X\times X \to \mathbb R$, genannt Metrik auf $X$, sodass gelten:
1. $$d(x,y) = d(y,x) \qquad \forall_{x,y \in X}$$
1. $$d(x,y) \ge 0,  \qquad d(x,y) = 0 \iff x=y\qquad \forall_ {x,y \in X}$$
1. $$d(x,z) \le d(x,y) + d(y,z) \qquad \forall _{x,y,z \in X}$$
Eine Metrik ist also eine symmetrische, positiv definite und subadditive Abbildung.

###### Definition: Topologischer Raum
Ein topologischer Raum $(X, \mathcal T)$  ist eine Menge $X$ mit einem Mengensystem $\mathcal T \subseteq \mathcal P(X)$ auf $X$, genannt Topologie auf $X$, sodass gelten:  1. $$\emptyset, X \in \mathcal T$$
1. $$\forall _{\mathcal F \subseteq \mathcal T}: \bigcup \mathcal F \in \mathcal T$$

1. $$\forall _{\substack{\mathcal F \subseteq \mathcal T \\ \left| \mathcal F \right| \lt \infty}}: \bigcap_{  }\mathcal F \in \mathcal T$$

Eine Topologie ist also ein beliebig vereinigungsstabiles, endlich durchschnittsstabiles Mengensystem, welches die Grundmenge und die leere Menge enthält.

###### Definition: Halbnormierter Raum
Ein halbnormierter Raum $(X, p)$ ist ein $\mathbb K$-Vektorraum $X$ mit einer Abbildung $p : X \to \mathbb K$, genannt Halbnorm auf $X$, sodass gelten:
1. $$p(x) \ge 0 \qquad \mathop{\forall}\limits_{\substack{x \in X}}$$
2. $$p(x + y) \le p(x) + p(y) \qquad  \mathop{\forall }\limits _ {\substack{x, y \in X}}$$
Eine Halbnorm ist also eine nichtnegative und subadditive Abbildung.

###### Definition: Normierter Raum
Ein normierter Raum $(X,\left\lVert \cdot  \right\rVert)$ ist ein $\mathbb K$-Vektorraum $X$ mit einer Abbildung $\left\lVert \cdot  \right\rVert  : X \to \mathbb K$, genannt Norm auf $X$, sodass gelten:
1. $$\left\lVert x \right\rVert \ge 0, \qquad \left\lVert x \right\rVert = 0 \iff x =0 \qquad \forall _{x\in X}$$
1. $$\left\lVert \lambda x \right\rVert = \left| \lambda  \right| \left\lVert x \right\rVert \qquad \mathop{\forall}\limits _{\substack{\lambda \in \mathbb{K} \\ x \in X}} $$
2. $$\left\lVert x + y \right\rVert \le  \left\lVert x \right\rVert  +  \left\lVert  y  \right\rVert   \qquad   \mathop{\forall }\limits_{x, y \in X}$$
Eine Norm ist also eine positiv-definite, absolut homogene und subadditive Abbildung.

###### Beispiel Metrischer Raum: Normierter Raum
Sei $(X, \left\lVert \cdot  \right\rVert )$ ein normierter Raum. Dann ist $d(x,y) = \left\lVert x -y \right\rVert$ eine Metrik auf $X.$

###### Beispiel Metrischer Raum: Diskreter Raum
Die Abbildung $d(x,y) = 1 - \delta_{xy}$ ist eine Metrik auf einer beliebigen Menge $X.$
### Normierte Räume
### Operatoren und Funktionale
### Hilberträume
### Spektraltheorie

----------------------------------------------------------------------
----------------------------------------------------------------------

# Algebra
## Diskrete Strukturen
### Logik
### Mengenlehre
### Graphentheorie
### Kombinatorik
## Gruppen
## Ringe
## Körper
## Vektorräume
## Normalformen
## Hilberträume
### Definition: Skalarprodukt, Euklidischer Raum, Unitärer Raum, Bilinearform, Sesquilinearform, symmetrisch, hermitesch
Sei $X$ ein $\mathbb{K}$-Vektorraum. Eine Abbildung 
$$\left\langle \cdot, \cdot  \right\rangle \colon\begin{cases}X\times X &\to & \mathbb{K} \\ (x,y) &\mapsto & \left\langle x,y  \right\rangle \end{cases}$$
heißt Skalarprodukt, wenn sie sesquilinear:
$$\mathop{\forall}\limits _ {\substack{x,y,z \in X\\ \lambda \in \mathbb{K}}} \colon
\begin{aligned}
\left\langle x, y+\lambda z \right\rangle &= \left\langle x,y \right\rangle+ \lambda\left\langle y,z \right\rangle \\
\left\langle x+\lambda y, z \right\rangle &=\left\langle x,z \right\rangle + \overline{\lambda} \left\langle y,z \right\rangle
,\end{aligned}$$
hermitesch:
$$\mathop{\forall}\limits _ {\substack{x,y \in X}}\colon \left\langle x,y \right\rangle = \overline{\left\langle y,x \right\rangle},$$
und  positiv definit:
$$\mathop{\forall}\limits _ {\substack{x \in X \\ x\neq 0}} \colon \left\langle x,x \right\rangle \gt 0$$
ist.
Die Sesquilinearität bildet im Reellen eine Bilinearität. Ein Skalarpodukt ist biadditiv.

### Beispiel: Kanonisches Skalarprodukt
### Beispiel: Integralskalarprodukt auf den stetigen Funktionen:
Für $a \lt b$ bezeichne $\mathscr{C}\left( [a,b];\ \mathbb{K} \right)$ wie gewohnt die stetigen Funktionen auf dem kompakten Intervall $[a,b] \subseteq \mathbb{R}$. Es ist durch 
$$\left\langle \cdot, \cdot  \right\rangle \colon\begin{cases} \mathscr{C}\left( [a,b];\ \mathbb{K} \right)\times\mathscr{C}\left( [a,b];\ \mathbb{K} \right)&\to &\mathbb{K} \\  (f,g) &\mapsto & \left\langle f,g \right\rangle : = \displaystyle\int_{a}^{b} \overline{f(x)}g(x) \ \mathrm{d} x \end{cases}$$
ein Skalarprodukt gegeben, $\left(\mathscr{C}\left( [a,b] ; \ \mathbb{K} \right), \ \left\langle \cdot, \cdot  \right\rangle \right)$ ist ein Skalarproduktraum.

###### Definition: Standardskalarprodukt
Für $x=\begin{pmatrix} x_1\\ \vdots\\ x_n \end{pmatrix},\ y= \begin{pmatrix} y_1\\ \vdots\\ y_n \end{pmatrix}\in \mathbb{K}^n$ ist durch $\left\langle x,y \right\rangle := \overline{x}^\bot y = \sum\limits_{k=1}^{n}\overline{x}_ky_k$ ein Skalarprodukt definiert.

###### Definition: Darstellungsmatrix eines Skalarprodukts
Ist $\left\langle \cdot, \cdot  \right\rangle$ ein Skalarprodukt auf einem endlichdimensionalen $\mathbb{K}$-Vektorraum $X$ und $B= (b_1, \ldots, b_n)$ eine Basis von $X$, so heißt die Matrix $A = \left( \left\langle b_i, b_j \right\rangle \right)_{i,j} \in \mathbb{K}^{n\times n}$ eine Darstellungsmatrix von $\left\langle \cdot, \cdot \right\rangle.$

###### Definition: Hermitesche, symmetrische Matrix
Eine Matrix $A \in \mathbb{K}^{n\times n}$ heißt hermitesch, wenn $A^{\bot}=\overline{A}.$  
Eine Matrix $A \in \mathbb{R}^{n\times n}$ heißt symmetrisch, wenn $A^{\bot}=A.$

###### Satz: Hermizität von Darstellungsmatrizen von Skalarprodukten
Eine Darstellungsmatrix $A \in \mathbb{K}^{n\times n}$ eines Skalarprodukts eines endlichdimensionalen Skalarproduktraums ist hermitesch.

###### Satz: Darstellungsmatrix eines Skalarprodukts reduziert auf eine Multiplikation
Sei $A$ die Darstellungsmatrix von einem Skalarprodukt $\left\langle \cdot, \cdot \right\rangle$ auf $\mathbb{K}^{n}$ bezüglich der Standardbasis. Dann ist das Skalarprodukt eine Matrixmultiplikation: 
$$\left\langle x,y \right\rangle = \overline{x}^{\bot}Ay.$$

###### Satz: Skalarprodukte induzieren eine Norm
Sei $\left\langle \cdot,\cdot  \right\rangle$ ein Skalarprodukt auf einem $\mathbb{K}$-Vektorraum $X$. Dann ist 
$$\left\lVert x \right\rVert := \sqrt{\left\langle x, x \right\rangle}$$
eine Norm auf $X$ definiert.  
**Beweis.** Die Norm ist nichtnegativ. Ist $x \neq 0$, so ist auch $\left\lVert x \right\rVert \gt 0$.  
Weiterhin ist $\left\lVert \lambda x \right\rVert = \sqrt{\left\langle \lambda x, \lambda x \right\rangle} = \sqrt{\lambda^2\left\langle x,x \right\rangle} = \left\lvert \lambda \right\rvert\sqrt{\left\langle x,x \right\rangle}= \lambda \left\lVert x \right\rVert.$  
Letztlich folgt die Subadditivität anhand der Cauchy-Schwarz-Ungleichung aus: 
$$\begin{aligned} \left\lVert x+y \right\rVert^2
&= \left\lVert x \right\rVert ^2 + \left\langle x, y \right\rangle + \left\langle y, x \right\rangle + \left\lVert y \right\rVert ^2 \\
&= \left\lVert x \right\rVert^2 + 2 \operatorname{Re}\left( \left\langle x,y \right\rangle \right) + \left\lVert y \right\rVert ^2 \\
&\le \left\lVert x \right\rVert^2 + 2 \left\lvert \left\langle x,y \right\rangle \right\rvert+ \left\lVert y \right\rVert^2 \\
&\le \left\lVert x \right\rVert^2 + 2\left\lVert x \right\rVert\left\lVert y \right\rVert +\left\lVert y \right\rVert ^2 \\ 
&= \left( \left\lVert x \right\rVert + \left\lVert y \right\rVert \right)^2 . \qquad \blacksquare
\end{aligned}$$


###### Satz: Normen induzieren Metriken
Sei $\left( X, \left\lVert \cdot \right\rVert \right)$ ein normierter Raum. Dann wird durch 
$$d(x,y) := \left\lVert x-y \right\rVert$$
eine Metrik auf $X$ definiert.  
**Beweis.** Die Symmetrie folgt aus $\left\lVert x-y \right\rVert = \left\lvert -1 \right\rvert \left\lVert y-x \right\rVert.$ Weiterhin ist $d$ nichtnegativ und $d(x,y) = 0 \iff x=y$. Letztlich ist 
$$\left\lVert x - z \right\rVert \le \left\lVert x-y \right\rVert + \left\lVert y-z \right\rVert. \qquad \blacksquare$$

###### Definition: Banachraum
Ein normierter Raum $\left( X, \left\lVert \cdot \right\rVert \right)$ heißt Banachraum, wenn der durch die Norm induzierte Metrische Raum $\left( X, d_{\left\lVert \cdot \right\rVert} \right)$ vollständig ist.

###### Definition: Hilbertraum
Ein Skalarproduktraum $\left( X, \left\langle \cdot, \cdot \right\rangle \right)$ heißt Hilbertraum, wenn er vollständig ist, also wenn der induzierte normierte Raum $\left( X, \left\lVert \cdot \right\rVert \right)$ vollständig, also ein Banachraum ist.

###### Beispiel: Manhattan-Norm
Durch $\left\lVert x \right\rVert := \sum\limits_{i=1}^{n}\left\lvert x_i \right\rvert$ wird eine Norm auf dem $\mathbb{R}^{n}$ definiert, welche nicht durch ein Skalarprodukt induziert ist.  
Es ist dies der Fall der $1$-Norm unter den $p$-Normen:
$$\left\lVert x \right\rVert_p := \left( \sum\limits_{k=1}^{n} x_k^{p} \right)^{1/p}.$$

###### Beispiel: Hamming-Metrik
Auf einem beliebigen Produktraum $X=M^n$ ist eine Metrik, genannt Hamming-Metrik, definiert durch:
$$d(x,y) : = \left\lvert \left\{ i \in \left\{ 1, \ldots, n \right\} \mid x_i \neq y_i \right\} \right\rvert .$$

###### Satz: Endlichdimensional impliziert vollständig
Ein endlichdimensionaler Skalarproduktraum ist ein Hilbertraum.  
Ein endlichdimensionaler Normierter Raum ist ein Banachraum.

###### Satz: Stetige Funktionen auf einem kompakten Intervall bilden mit der Supremumsnorm einen Banachraum
Der Vektorraum $\mathscr{C}\left( [a,b]; \ \mathbb{K} \right)$ bildet mit der Supremumsnorm $\left\lVert f \right\rVert := \sup \operatorname{im}\left\lvert f \right\rvert = \sup \left\lvert f \right\rvert = \max \left\lvert f \right\rvert$ einen vollständigen normierten Raum, also einen Banachraum.

###### Satz: Stetige Funktionen auf einem kompakten Intervall bilden mit der Skalarproduktnorm kein Banachraum
Der Vektorraum $\mathscr{C}\left( [a,];\ \mathbb{R} \right)$ ist mit der vom Skalarprodukt $\left\langle f,g \right\rangle = \int_{a}^{b} f(x)g(x) \ \mathrm{d} x$ induzierten Norm nicht vollständig.

###### Satz: Hilbertscher Folgenraum
Es bezeichne mit $\ell ^{2} : = \left\{ x \in \mathbb{K}^{\mathbb{N}} \mid \sum\limits_{n=1}^{\infty} \left\lvert x_{n} \right\rvert^2 \in \mathrm{c}\right\}$ die Menge aller (betrags-)quadratsummierbaren Folgen. Dies ist ein unendlichdimensionaler Vektorraum. Durch $\left\langle x,y \right\rangle := \sum\limits_{n=1}^{\infty}\overline{x}_ny_n$ ist auf $\ell^2$ ein Skalarprodukt induziert, bezüglich diesem der Raum vollständig ist.

###### Definition: Winkel
Seien $x,y \in X$ normpositive Elemente eines euklidischen Raums $X$.
Dann heißt die eindeutig bestimmte Zahl $\alpha \in [0,\pi]$, sodass 
$$\cos(\alpha) = \frac{\left\langle x,y \right\rangle}{\left\lVert x \right\rVert\left\lVert y \right\rVert}$$
der Winkel zwischen $x, y.$

###### Beispiel: Winkel
Im euklidischen Standardraum ist für $\begin{pmatrix} 1 \\0 \end{pmatrix}, \begin{pmatrix} 1 \\ 1 \end{pmatrix} \in \mathbb{R}^2$: 
$$\frac{\left\langle x,y \right\rangle}{\left\lVert x \right\rVert\left\lVert y \right\rVert} = \frac{1}{\sqrt{2}},$$
also beträgt der Winkel $\frac{\pi}{4}.$

###### Definition: Orthogonale Vektoren
Zwei Vektoren $x,y \in X$ eines Skalarproduktraums $\left( X, \left\langle \cdot, \cdot  \right\rangle \right)$ heißen orthogonal, wenn $\left\langle x,y \right\rangle = 0$, in Zeichen: $x\bot y.$

###### Definition: Orthogonalsystem, Orthonormalsystem, Orthonormalbasis
Eine Teilmenge $S \subseteq X$ eines Skalarproduktraums $X$ heißt Orthogonalsystem, wenn je zwei paarweise verschiedene Vektoren $x,y \in S$ orthogonal sind.

###### Definition: Orthonormalsystem
Eine Teilmenge $S \subseteq X$ eines Skalarproduktraums $X$ heißt Orthonormalsystem, wenn je zwei paarweise verschiedene Vektoren $x,y \in S$ orthogonal sind und alle Elemente $x \in S$ auf der Einheitssphäre liegen, also $\left\lVert x \right\rVert =1$.

###### Definition: Orthonormalbasis
Eine Teilmenge $S \subseteq X$ eines Skalarproduktraums $X$ heißt Orthonormalsystem, wenn je zwei paarweise verschiedene Vektoren $x,y \in S$ orthogonal sind, alle Vektoren $x \in S$ auf der Einheitssphäre $S_1$ liegen, also $\left\lVert x \right\rVert =1$ und $S$ eine Basis von $X$ bildet.

###### Definition: Orthogonales Komplement
Zu einem Unterraum $U \subseteq X$ eines Skalarproduktraums $X$ heißt
$$U^{\bot}:= \left\{ x \in X \mid \mathop{\forall}\limits _ {\substack{u \in U}}\left\langle x,u \right\rangle = 0  \right\}$$
das orthogonale Komplement von $U.$ 

###### Satz: Orthogonalkomplementraum
Das orthogonale Komplement $U^{\bot}$ von $U\subseteq X$ ist ein Unterraum von $X$.

###### Satz: Orthonormalsystem auf dem Raum der stetigen komplexen Funktionen
Auf dem Hilbertraum 
$$\left( \mathscr{C}\left( [a,b];\ \mathbb{C} \right), \ \left\langle f,g \right\rangle:= \int_{a}^{b} \overline{f(x)}g(x) \ \mathrm{d} x \right)$$
ist durch $\left( f_n(x) := \frac{1}{\sqrt{2\pi}}\mathrm{e}^{\mathrm{i}nx} \right)_{ n \in \mathbb{Z} }$ ein Orthonormalsystem gegeben.


###### Satz: Lineare Unabhängigkeit eines Orthogonalsystems
Jedes orthogonalsystem $S \subseteq X$ eines Skalarproduktraums, das nicht den Nullvektor enthält, ist linear unabhängig.  
Ist $X$ endlichdimensional und gilt $\left\lvert S \right\rvert = \dim X$, so ist $S$ eine Basis.  

**Beweis.** Sind $x_1, \ldots, x_n \in S$ paarweise verschieden und $\lambda_1x_1 + \cdots + \lambda_nx_n = 0$ mit $\lambda_i \in \mathbb{K}$.  
Durch Bildung des Skalarprodukts von $x_i$ und $0$ folgt $\mathop{\forall}\limits _ {\substack{i \in [n]}}:$
$$0 = \left\langle x_i, 0 \right\rangle = \left\langle x_i, \sum\limits_{k=1}^{n}\lambda_k x_k \right\rangle = \sum\limits_{k=1}^{n}\lambda_k \left\langle x_i, x_k \right\rangle = \lambda_i \left\langle x_i, x_i \right\rangle ,$$
also ist die Linearkombination trivial und $S$ ist linear unabhängig.  
Weiterhin ist jede maximal linear unabhängige Teilmenge eine Basis. $\blacksquare$

###### Satz: Orthonormalbasen endlichdimensionaler Skalarprodukträume
Sei $B = \left\{ b_1, \ldots, b_n \right\} \subseteq X$ eine Orthonormalbasis eines endlichdimensionalen Skalarproduktraums $X$ und $x  \in X.$ Dann sind die Skalarprodukte $\left\langle b_i,x \right\rangle$ genau die Koordinaten von $x$ bezüglich der Basis $B$.

**Beweis.** Gilt $x = \sum\limits_{k=1}^{n}\lambda_kb_k$ für $\lambda_k \in \mathbb{K}$, so folgt
$$\left\langle b_i, x \right\rangle = \left\langle b_i, \sum\limits_{k=1}^{n}\lambda_k b_k \right\rangle = \sum\limits_{k=1}^{n} \lambda _k \left\langle b_i, b_k \right\rangle = \lambda_i \left\langle b_i, b_i \right\rangle = \lambda_i. \qquad \blacksquare$$
###### Algorithmus: Schmidtsches Orthogonalisierungsverfahren
**Eingabe:** Vektoren $x_1, \ldots , x_n \subseteq X$ eines Skalarproduktraums.  
**Ausgabe:** Orthonormalbasis $\left\{ b_1, \ldots, b_m \right\}$ des induzierten Unterraums $\left\langle x_1, \ldots, x_k \right\rangle\subseteq X$.

1. Setze $m:= 0$.  
2. $\mathbf{for } \quad i = 1,\ldots,n$
	1. $w_i := x_i -\sum\limits_{k=1}^{n} \left\langle b_k, x_i \right\rangle b_k.$
	2. $\mathbf{if }\quad w_i \neq 0$
		1. $m++$ 
		2. $b_m := \frac{1}{\left\lVert w_i \right\rVert }w_i.$

**Beweis.** Wir benutzen Induktion nach der Anzahl $n$ der Erzeuger. Nach Induktion gelten nach Durchlaufen der Schleife für $i=1, \ldots , n-1$:
$$\mathop{\forall}\limits _ {\substack{1 \le i, j \le m}}\left\langle b_i, b_j \right\rangle = \delta_{ ij }$$  
und 
$$\left\langle x_1, \ldots, x_{n-1} \right\rangle = \left\langle  \right\rangle$$


----------------------------------------------------------------------
----------------------------------------------------------------------

# Stochastik
## Stochastik 1
### Diskrete Wahrscheinlichkeitsräume
### Bedingte Wahrscheinlichkeit und Unabhängigkeit
### Zufallsvariablen, Erwartungswerte und Varianzen
### Summen unabhängiger Zufallsvariablen
### Wahrscheinlichkeit mit Dichten
### Grenzwertsätze

## Stochastik 2

## Statistik
### Einführung
### Deskriptive Statistik
### Parameterabschätzung

----------------------------------------------------------------------
----------------------------------------------------------------------

# Informatik

## Datenbanken

## Betriebssysteme

## Theoretische Informatik

## Algorithmik


------

# Rechnung
$|x| < 1 \stackrel{?}{\implies} x^n \to 0$

$\begin{aligned} \liminf\limits_{n \to \infty}A_n &:= \bigcup\limits_{m = 1}^{\infty}\bigcap\limits_{n = m}^{\infty}A_n \\ \limsup\limits_{n \to \infty}A_n &:= \bigcap\limits_{n=1}^{\infty}\bigcup\limits_{n = m}^{\infty}A_n\end{aligned}$ Eine Abbildung/Familie $$x \colon\begin{cases}I &\longrightarrow &X \\ i &\longmapsto &x_i \end{cases} =: (x_i)_{i \in I} \subseteq X$$
heißt Familie 

Für Abbildungen
$$g \colon X \longrightarrow Y\\ f \colon Y \longrightarrow Z,$$
wie ist die Komposition:
$$g \circ f \colon\begin{cases}X &\longrightarrow &Z \\ x &\longmapsto &(g \circ f)(x) := g(f(x)) \end{cases}$$
definiert?

---
[beispiel](beispiel)

## [Topologie](Topologie)
## [Gruppen](Gruppen)
## [Ringe](Ringe)
## [Körper](Körper)
## [Vektorräume](Vektorräume)
## [NormierteRäume](NormierteRäume)
## [Hilberträume](Hilberträume)
## [Exponentiation](Exponentiation)
## [Differentiation](Differentiation)
## [Integration](Integration)

