>[!Regole]-
>- # Regola 1
>  $2x = 0 \rightarrow x = -x$
> Imponiamo questa regola attraverso una **relazione di equivalenza**
> Ricordiamo che quindi la "semplificazione" avviene attraverso l'addizione di una stessa variabile (ricordando che $2x = 0 \rightarrow x = -x$)
>>[!EXAMPLE]+ Esempio
>>$$
>>\begin{gather}
>>1 + x + xy = x + xy + y \quad \text{(Sommo } xy \text{ a entrambi i membri)}\\
>>1 + x + 2xy = x + 2xy + y \quad \text{(Per la regola di prima } 2 = o \rightarrow 2xy = 0 \text{)} \\
>>1 + x = x + y \quad \text{(Sommo } x \text{ ad entrambi i membri} \\
>>1 + 2x = 2x + y \quad \text{(}2x = 0 \text{)} \\
>>1 = y \quad \text{(Questo è impossibile perchè y è una "variabile" non una costante)}
>>\end{gather}
>>$$
>
>- # Regola 2
>  $x^n = x \wedge x \wedge \text{... (n-volte) ... } \wedge x= x$
>>[!EXAMPLE]+ Esempio
>>$$
>>\begin{gather}\\
(1+x)^5 \\
(1+x)^2 \cdot (1+x)^2 \cdot (1+x) \qquad \text{[}(1+x)^2 = \lnot p \wedge \lnot p = \lnot p \text{]} \\
(1+x) = \lnot p \\
>>\end{gather}
>>$$
>
>- # Regola Distributiva
>- # Leggi di De Morgan

>[!Traduzione Proposizioni Logiche]-
>Imponiamo che i valori :
>		Vero $\rightarrow$ 1
>		Falso $\rightarrow$ 0
>
>Dobbiamo considerare le proposizioni logiche "come delle funzioni n-"aire che partono da un insieme $P=\{p : proposizioni\}$ , che contiene al suo interno le variabili a cui andremo ad applicare le "funzioni"
>
>>[!Negazione / NOT]-
>>$\lnot : P\rightarrow P$
>>Tabella #Negazione 
>>La "traduzione" di $\lnot x$ in forma algebrica è : **$1+x$**
>
>>[!Congiunzione /AND]-
>>$\land : P \times P \rightarrow P$
>>![[Excalidraw/Drawing 2025-10-04 15.42.11.excalidraw|Drawing 2025-10-04 15.42.11.excalidraw]]
>>Tabella #Congiunzione 
>>La "traduzione" di $p \land q$ in forma algebrica è : **$x*y$**
>
>>[!Disgiunzione Inclusiva \ OR]-
>>$\lor : P \times P \rightarrow P$
>>![[Drawing 2025-10-04 15.55.02.excalidraw]]
>>Tabella #Disgiunzione
>>La "traduzione" di $p \lor q$ in forma algebrica è : **$x+y+xy$**
>
>>[!Disgiunzione Esclusiva \ XOR]-
>>$XOR : P \times P \rightarrow P$
>>![[Drawing 2025-10-04 18.24.22.excalidraw]]
>>Tabella #XOR 
>>La "traduzione di $p \oplus q$ è : $x + y$"
>
>>[!Implicazione Formale]-
>>$\rightarrow : P \times P \rightarrow P$
>>![[Drawing 2025-10-04 18.37.53.excalidraw]]
>>Tabella #Implicazione
>>La "traduzione" di $p \rightarrow q$ è : $1 + x + xy$
>
>>[!INFO]+ Doppia Implicazione
>$x \Leftrightarrow y = 1 + x + y$
>
>>[!EXAMPLE]+ Esempio
>>Formula algebrica : $a + bx + cy + dxy$
>>Formula Logica Proposizionale : 
>>$$
>>\begin{gather}
(a = 0 , b = 0 , c = 0 , d = 0) \quad 0 + 0 + 0 = 0 \lor y \\
(a = 0 , b = 0 , c = 0 , d = 1) \quad 0 + 0 + 0 + xy = x\wedge y \\
(a = 0 , b = 0 , c = 1 , d = 0) \quad 0 + 0 + y + 0 = y\\
(a = 0 , b = 0 , c = 1 , d = 1) \quad  0 + 0 + y + xy =y(1+x) = y \wedge (\lnot x) \\
(a = 0 , b = 1 , c = 0 , d = 0) \quad 0 + x + 0 + 0 = x\\
(a = 0 , b = 1 , c = 0 , d = 1) \quad 0 + x + 0 +xy = x(1+y) = x\wedge(\lnot y) \\ 
(a = 0 , b = 1 , c = 1 , d = 0) \quad 0 + x + y + 0 = x \oplus y \\
(a = 0 , b = 1 , c = 1 , d = 1) \quad 0 + x + y + xy = x \lor y\\
(a = 1 , b = 0 , c = 0 , d = 0) \quad 1 + 0 + 0 + 0 = 1\\
(a = 1 , b = 0 , c = 0 , d = 1) \quad 1 + 0 + 0 + xy = \lnot(x\wedge y) \\
(a = 1 , b = 0 , c = 1 , d = 0) \quad 1 + 0 + y + 0 = \lnot y\\
(a = 1 , b = 0 , c = 1 , d = 1) \quad 1 + 0 + y + xy = 1 + y(1+x) = \lnot (y \wedge(\lnot x))\\
(a = 1 , b = 1 , c = 0 , d = 0) \quad 1 + x + 0 + 0 = \lnot x\\ 
(a = 1 , b = 1 , c = 0 , d = 1) \quad 1 + x + 0 + xy = 1 + x(1 + y) = \lnot(x \wedge \lnot y)\\ 
(a = 1 , b = 1 , c = 1 , d = 0) \quad 1 + x + y = \lnot (x \oplus y)\\
(a = 1 , b = 1 , c = 1 , d = 1) \quad 1 + x + y + xy = \lnot(x \lor y) \\
\end{gather}
>>$$


# [[CNF e DNF]]