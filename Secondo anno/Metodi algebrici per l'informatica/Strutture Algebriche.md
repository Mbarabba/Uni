>[!Operazione Binaria]-
>$\text{Sia M un insieme } f:M\times M \rightarrow M$
>Un'**operazione binaria** su un insieme M è una regola che prende **due elementi** qualsiasi di M e li combina per produrre un **unico risultato** che appartiene ancora allo stesso insieme M.

>[!INFO]- Proprietà #associativa 
>La **proprietà #associativa ** garantisce che, in un'operazione ripetuta, l'ordine in cui si eseguono i calcoli non influisce sul risultato finale. 
>
>>[!EXAMPLE]+
>>- Moltiplicazione: $(a \cdot b)\cdot c = a\cdot(b\cdot c)$
>>- Addizione : $(5+2)+1 = 5 + (2+1)$

>[!INFO]- Elemento Inverso
>L'**elemento inverso**  di un elemento _a_ e donominato come -a , è un altro elemento che, combinato con _a_, produce l'elemento neutro. È l'elemento che "annulla" o "fa tornare indietro" l'operazione. L'esistenza di un inverso dipende dall'esistenza di un elemento neutro.
>
>>[!EXAMPLE]+ Esempi
>>- Addizione : $x + (-x) = 0$
>>- Moltiplicazione $x\cdot \frac{1}{x}=1$

>[!INFO]- Elemento Neutro
>L'**elemento neutro** denotatato come $0_{M}$ è un elemento speciale di un insieme che, quando combinato con qualsiasi altro elemento tramite un'operazione binaria, lascia quell'elemento **invariato**. È l'elemento "non fare nulla" dell'operazione.
>
>>[!EXAMPLE]+ Esempi
>>- Addizione : $x+0=0+x=x$
>>- Moltiplicazione : $x*1=1*x=x$

>[!INFO]+ #Semigruppo 
>M viene detto **Semigruppo** se $f$ è #associativa
>$$\begin{gather} \forall a,b,c \in M \quad f(a,b)=a\cdot b,ab \\
(a\cdot b) \cdot c = a \cdot (b \cdot c) \end{gather}$$

>[!INFO]+ #Monoide
>M viene detto **Monoide** se M è un #Semigruppo ed ha un elemento neutro: 
>$$\begin{gather}\exists1_{M} \text{ (elemento neutro)}:\forall a\in M \quad 1_{M}\cdot a=a\cdot1_{M}=a\end{gather}$$
>
>>[!INFO]+ Monoide #Abeliano
>Un monoide M si dice **abeliano se il prodotto è commutativo** , ossia se :
>$$\begin{gather} a \cdot b=b \cdot a \quad \forall a,b \in M   \end{gather}$$
>
>>[!EXAMPLE]- Esempio
>>$(N,+,0_{N})$ è un monoide abeliano , questo perchè la somma è commutativa e 0 è il suo elemento neutro
>>
>>- $\mathbb{N}$ è l'inseme della struttura (In questo caso è l'insieme dei numeri naturali)
>>- \+ è la sua operazione , inoltre $a+b\in N \quad \forall a,b\in N$
>>  (La somma di 2 naturali appartiene ancora all'insieme dei numeri naturali)
>>- $0_{N}$ è il suo elemento neutro

>[!INFO]+ #Gruppo
>M è un **Gruppo** se :
>1. M è un #Semigruppo 
>2. M è un #Monoide 
>3. Esiste **l'elemento inverso ed è unico**
>   $\qquad \forall a\in M\exists b\in M : a\cdot b=b\cdot a=1_{M}$
>
>>[!INFO]+ #Gruppo_ciclico
>M si dice #Gruppo_ciclico se $\exists a\in G$ tale che $G = \{a^k:k\in Z\}$
>>
>>Per far si che G sia un gruppo ciclico ogni suo elemento può essere espresso come potenza del generatore \<a\>
>>
>>>[!INFO] Osservazione
>>>Se G è ciclico allora è #Abeliano ma se un gruppo è abeliano non per forza è ciclico
>
>>[!EXAMPLE]- Esempio
>>$(\mathbb{Z},+,0)$ è un gruppo abeliano ,
>>$\exists a \in \mathbb{Z} : \mathbb{Z}=<a>=\{ka:k\in \mathbb{z}\}$
>
>>[!EXAMPLE]- Esempio
>>$\mathbb{Z},\mathbb{Q},\mathbb{R},\mathbb{C}$ sono gruppi abeliani rispetto a \+,0

>[!INFO]+ #Anello
>Sia A un gruppo abeliano rispetto alla somma , allora esso viene definito come anello se :
>5. A è un #Monoide rispetto al prodotto , in particolare esiste $1_{A}$ tale che:
>   $\qquad a\cdot1_{A}=1_{A}\cdot a=a$
>6. Valgono le leggi distributive del prodotto rispetto alla somma , ossia:
>   $\qquad a \cdot (b \cdot c) = a \cdot b + a \cdot c \qquad (b+c) \cdot a = b \cdot a + c \cdot a$
>  
>- Se il prodotto è commutativo l'anello si dice che l'anello è commutativo
>- Se $\forall a \not= 0_{M} \text{ esiste } a^{-1}$ A viene definito come #Camp