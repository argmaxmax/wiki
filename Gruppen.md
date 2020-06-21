## Gruppenoperationen
Definition: Gruppenoperation
Eine Gruppenoperation einer Gruppe $G$ auf $M$ ist eine Abbildung 
$$f \colon\begin{cases}G \times M &\longrightarrow &M \\ (g,x) &\longmapsto & g(x) \end{cases},$$
sodass 
$$\mathop{\forall}\limits _ {\substack{g,h \in G \\ x \in M}} (gh)(x) = g(h(x))$$
und 
$$\mathop{\forall}\limits _ {\substack{x \in M}}e(x) =x.$$
Es heißt dann $G$ auf $M$ operierend.

Definition: Fixgruppe einer Gruppenoperation
Es operiere eine Gruppe $G$ auf einer Menge $M$.  
Dann heißt 
$$G_x:= \left\{ g \in G \mid g(x) = x \right\} \subseteq G$$
die Fixgruppe von $x \in M.$


Definition: Bahn einer Gruppenoperation
Es operiere eine Gruppe $G$ auf einer Menge $M$.  
Dann heißt
$$G(x) := \left\{ g(x) \mid g \in G \right\} \subseteq M$$ 
die Bahn von $x \in M.$

Definition: Treue Gruppenoperation
Eine Gruppenoperation einer Gruppe $G$ auf einer Menge $M$ heißt treu, wenn $e$ das einzige Gruppenelement ist, dass alle $x \in M$ fixiert:
$$\bigcap\limits_{x \in M} G_x = \left\{ e \right\}.$$

[Definition: Transitive Gruppenoperation](Definition: Transitive Gruppenoperation)
Eine Gruppenoperation einer Gruppe $G$ auf einer Menge $M$ heißt transitiv, wenn:
$$\mathop{\exists}\limits _ {\substack{x \in M}}G(x) =M.$$

Definition: Symmetrische Gruppe
Die Gruppe $\left( S_M, \circ  \right) := \left( \operatorname{bij}M, \circ  \right)$ aller Bijektionen $\operatorname{bij}M$ auf $M$ mit der Komposition heißt symmetrische Gruppe. 

Satz: Gruppenoperationen und Homomorphismen
Zu einer Gruppenoperation einer Gruppe $G$ auf einer Menge $M$ gibt es einen Homomorphismus
$$\pi \colon\begin{cases}G &\longrightarrow &S_M \\ g &\longmapsto & \varphi_g \colon\begin{cases}M &\longrightarrow &M \\ x &\longmapsto &g(x) \end{cases} \end{cases}.$$  
Die Gruppenoperation ist genau dann treu, wenn dieser Homomorphismus injektiv ist.
Umgekehrt gibt es zu einem Homomorphismus $\pi \colon G \longrightarrow S_M$ eine Gruppenoperation der Gruppe $G$ auf $M$, gegeben durch:
$$\begin{cases} G \times M &\longrightarrow & M \\ (g,x) &\longmapsto & g(x) = (\pi(g))(x) \end{cases}$$
