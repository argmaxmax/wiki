# Satz: Fortsetzung beschränkter Operatoren auf den Abschluss
Sei $X$ ein normierter Raum, $S\subseteq X$ ein Untervektorraum und $Y$ ein Banachraum. Sei $T\in B(S,Y)$ ein beschränkter Operator.  
Dann existiert genau ein beschränkter Operator $\widetilde T \in B(\bar{S}, Y)$ sodass gelten: 
1. $\widetilde{T}$ ist eine Fortsetzung von $T:$ $$\widetilde{T}|_S = T$$
2. $$\left\lVert \widetilde{T} \right\rVert = \left\lVert T \right\rVert .$$

## Beweis.
Definiere einen Operator $\widetilde{T} : \bar{S} \to Y$ wie folgt: für $\overline{x} \in \overline{S}$ wähle eine Folge $(x_n) \subseteq S$ mit $\lim_{n \to \infty}x_n = \overline{x}.$  
Dann gilt $$\left\lVert Tx_n-Tx_m \right\rVert \le \left\lVert T \right\rVert \cdot \left\lVert x_n-x_m \right\rVert $$ weshalb $(Tx_n)\subseteq Y$ eine Cauchyfolge ist.  
Da $Y$ vollständig ist existiert $y\in Y$ sodass $Tx_{n} \to y$.  
Wir setzen $\widetilde{T}\bar{x}=y.$ Um zu zeigen, dass diese Definition zulässig ist, reicht es für gegen $\overline{x}$ konvergente Folgen $(x_n), (x'_n)\subseteq S$ zu zeigen, dass $$\left\lVert Tx_n - Tx'_n \right\rVert \le  \left\lVert T \right\rVert \left\lVert x_n-x'_n \right\rVert \le  \left\lVert x_n -\overline{x} \right\rVert + \left\lVert \overline{x}-x'_n \right\rVert \to 0,$$ also ist $\widetilde{T}\overline{x}$ unabhängig von der Wahl der gegen $\overline{x}$ konvergenten Folge. Insgesamt also ist $$\widetilde{T}\overline{x}= \lim_{n \to \infty} Tx_n.$$
(1.) folgt aus der Wahl der konstanten Folge $x_n = \overline{x}$ für $\overline{x}\in{S}$.  
Dass $\widetilde{ T}$ linear ist, folgt aus der Stetigkeit der Addition und Skalarmultiplikation.  
Dass $\widetilde{T}$ beschränkt ist folgt aus $$\left\lVert \widetilde{T}\overline{x} \right\rVert =\lim_{n \to \infty}\left\lVert Tx_n \right\rVert \le \lim_{n \to \infty}\left( \left\lVert T \right\rVert \cdot\left\lVert x_n \right\rVert  \right) =\left\lVert T \right\rVert \cdot\left\lVert \overline{x} \right\rVert .  $$ 
