Definition: Konvexer Kegel
Eine nichtleere Teilmenge $C\subseteq X$ eines rellen Vektorraums $X$ heißt konvexer Kegel, falls für alle $\alpha \ge 0, \ c\in C$ gilt: $$\alpha c\in C.$$
#### Definition: Dualkegel
Sei $C\subseteq X$ ein konvexer Kegel in einem rellen Vektorraum $X$.  
Dann heißt die Menge $$C^* := \left\{ f \in X^* \mid f|_C \ge 0 \right\} \subseteq X^*$$ Dualkegel von $C$.

#### Kommentar
Ist $C$ ein konvexer Kegel in $X$, so ist der Dualkegel $C^*$ ein konvexer Kegel in $X^*$.  


#### Definition: Bidualkegel
Sei $C\subseteq X$ ein konvexer Kegel in einem rellen Vektorraum $X$.  
Dann heißt $$C^{**}$$ der Dualkegel von $C.$

#### Definition: Kanonischer Bidualraummonomorphismus
Sei $X$ ein $K$-Vektorraum.  
Dann heißt die Abbildung $$J:\begin{cases}X &\to &X'' \\ x &\mapsto &J(x):\begin{cases}X' &\to &K \\ f &\mapsto &f(x) \end{cases} \end{cases}$$ kanonischer Bidualraummonomorphismus.

#### Satz: Kanonischer Bidualraummonomorphismus
Sei $X$ ein $K$-Vektorraum. Dann ist der Bidualraummonomorphismus $$J:\begin{cases}X &\to &X'' \\ x &\mapsto &J(x):\begin{cases}X' &\to &K \\ f &\mapsto &f(x) \end{cases} \end{cases}$$ ein injektiver Vektorraumhomomorphismus.  
Ist $X$ endlichdimensional, so ist $J$ ein Isomorphismus.  

#### Definition: Reflexiver Raum
Ein normierter Raum $X$ heißt reflexiv, falls der kanonische Bidualraummonomorphismus surjektiv ist.
#### Satz: Konvexer Kegel unter kanonischer Bidualraummonomorphismustransformation
Sei $C\subseteq X$ ein konvexer Kegel in einem rellen, reflexiven Banachraum $(X,\left\lVert \cdot  \right\rVert )$ und $J : X \to X^{**}$ der kanonische Bidualraummonomorphismus.  
Dann ist $$J(C) = C^{**}.$$
**Beweis.** Der Beweis gliedert sich in drei Schritten:  
1. $J(C) \subseteq C^{**}$
2. $c\not \in C\implies \exists f \in C^*: f(c) \lt 0$$h
3. $C^{**}\subseteq J(C)$


Lösung:  

(a) Let $\varphi \in J(C)$, $f \in C^*$ and $\varphi =J(x)$ for some $x\in C$. By definition, $F|_C \ge  0$. Therefore $\varphi (f) = J(x)(f)=f(x) \ge 0$ and $J(C)\subseteq C^{**}$.  

(b) Let $A,B \subseteq X$ be disjoint convex sets, $A$ closed and $B$ compact.  
Then $\exists F\in X^{*}, \ c \in \mathbb R$ such that $\forall a\in A, \ b \in B$ $$F(a)\lt c \lt F(b).$$  
Suppose $c\not \in C.$  
Then by Geometric Hahn-Banach, there exist $r\in \mathbb R, \ f \in X^*$ such that for all $d\in C,$ $$f(c)\lt r \lt f(d).$$  
Especially, since $0\in C$ and $f(0) =0$, we jave $f(c)\lt 0.$
Claim: $f|_C \ge  0$  
Suppose $f(d_0)\lt 0$ for some $d_0 \lt 0$. Then $f(\alpha d_0)\lt r$ for some $\alpha \gt 0$, but $\alpha d_0\in C$, a contradiction.  

(c) Let $\varphi \in C^{**}$. Since $X$ is reflexive, $x:=J^{-1}(\varphi )\in X$ exists. Suppose $x \not \in C$. Then by (b), $\exists f\in C^*$ such that $$\underbrace{f(x)}_{=\varphi (f)} \lt 0,$$ a contradiction.  

(d) Let $\varphi \in X^{**}\setminus J(X)$. Define $$\begin{align*} C^{(1)} :=& \left\{ f\in X^* \mid \varphi (f)\ge 0 \right\}\\ C^{(2)}:=& \left\{ \lambda \varphi \mid \lambda \ge 0 \right\}\\ C :=& \left\{ c\in C \mid f(c) \ge 0 \ \forall f\in C^{(1)} \right\} \\ =& \bigcap_{f\in C^{(1)}}f^{-1}\left( [0,\infty) \right).     \end{align*}$$  
We note that $C$ is closed. If $c\in C, \ \alpha \ge 0$ then for all $f\in C$, $$f(\alpha c) = \alpha f(c) \ge 0,$$ which implies that $C$ is a convex cone. Its dual cone is $$C^* = \left\{ f\in X^* \mid f(c) \ge  0 \ \forall c\in C \right\}. $$ Since $f\in C^{(1)}$, it follows that $f|C \ge 0$, which in turn is equivalent to $f \in C^*$. Therefore $C^{(1)}\subseteq C^*$.  
Let $\lambda \varphi  \in C^{(2)}$, i.e. $(\lambda \varphi )(f)\ge 0 \ \forall f\in C^{(1)}$, which is equivalent to $\lambda \varphi \in {C^{(1)}}^*\subseteq C^{**}$. Therefore $\varphi \in C^{**}$ but $\varphi \not \in J(C).$  

(e) Let $C ={0}$. Then $C^* = X^*$ and $C^{**}=J(C)$, because if $\varphi \in C^{**}$ then for all $f\in X^*$, $\varphi (f) \ge  0$ and herewith $\varphi (f) = 0$.

# [Endomorphismenalgebra](Endomorphismenalgebra)

