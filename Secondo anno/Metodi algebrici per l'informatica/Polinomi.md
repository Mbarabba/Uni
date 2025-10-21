>[!definizione] Polinomi
>>[!approfondimento]+ Cos'è un polinimo?
>>Un polinomio $a(x)$ è un elemento dell'insieme $K[x]  \text{ (anello commutativo/campo)}$, dove K è il #Campo dei coefficienti.
>>>[!sub-appro] Come esprimere un polinomio 
>>>Formalmente , un polinomio non nullo è un sommatoria espressa come
>>>$$\begin{gather} a(x)=\sum_{i=0}^na_{i}x^i \\ \\
a_{i} \in K \quad \text{ coefficienti appartenenti a }K \\
x \quad \text{ variabile / indeterminante}
\end{gather}$$
>>>>[!EXAMPLE] Esempio pratico
>>>>$$\begin{gather} a(x) = 2x^3+x^2-3x+5 \\
>>>>a_{0} = 5 \quad a_{1}=-3 \quad a_{2}=1 \quad a_{3}=2 \\ \\
>>>>a(x)=\sum_{i=0}^3 a_{i}x^i \\ \\ 
>>>>a(x) = a_{0}x^+a_{1}x^1+a_{2}x^2+a_{3}x^3 \\
>>>>a(x) = 5x^0 -3x + x^2 + 2x^3 = 2x^3 + x^2 -3x + 5
>>>>\end{gather}$$
>>>^polinomio-rappresentazione-formale
>>
>>>[!sub-appro]+ Uguaglianza tra polinomi
>>>Due polinomi sono considerati uguali se e solo se le loro successioni di coefficienti coincidono
>>>
>>>>[!EXAMPLE] Esempio pratico
>>>>$$\begin{gather} a(x) = 3x^2 + 0x + 5 \qquad a_{0}= 5 , a_{1}= 0 , a_{2} =3 \\b(x) = 5 + 3x^2 \qquad b_{0} = 5 , b_{1} = 0 , b_{2}=3\\ \\a = b \qquad \text{ i loro coefficienti sono uguali} \end{gather}$$
>
>>[!approfondimento]+ Operazione tra polinomi
>>>[!sub-appro]+ Somma
>>>La somma tra 2 polinomi è definita in modo tale che avvenga componente per componente
>>>
>>>Siano $a(x),b(x) \in K[x]$ dove K è il campo dei coefficienti i polinomi sono rappresentati come sommatorie
>>>
>>>$$\begin{gather} a(x) = \sum_{i}a_{i}x^i  \\
>>>b(x) = \sum_{k}b_{k}x^k \\  \\
>>>a(x)+b(x) \text{ è definita come : } \\ \\
>>>a(x) + b(x) = \sum_{i}a_{i}x^i  + \sum_{k}b_{k}x^k = \sum_{j}(a_{j}+b_{j})x^j 
>>>\end{gather}
>>>$$
>>>>[!EXAMPLE]+ Esempio pratico di somma tra polinomi
>>>>$$\begin{gather} a(x) = 2x^3+x^2-3x + 5 \\
>>>>b(x) = 4x^3-x^2+7x-1 \\ 
>>>>a(x) + b(x) = c(x)  \\ \\
>>>>c(x) = (5 + (-1))x^0 + (3 + 7)x^1 + (1 + (-1))x^2 + (2 + 4)x^3 \\
>>>>c(x) = 4x^0 + 10x^1 + 0x^2 + 6x^3 \\ \\
>>>>c(x) = 6x^3 + 10x + 4
\end{gather}$$
>>
>>>[!sub-appro]+ Prodotto
>>>Il prodotto tra polinomi è definito attraverso il prodotto di Cauchy
>>>
>>>Siano $a(x),b(x) \in K[x]$ dove K è il campo dei coefficienti i polinomi sono rappresentati come sommatorie
>>>
>>>$$\begin{gather} a(x) = \sum_{i}a_{i}x^i \quad , \quad b(x) = \sum_{k}b_{k}x^k \\  \\
\text{Il loro prodotto } a(x)\cdot b(x) \text{ è un nuovo polinomio indicato come} \\ \\
c_{j}=\sum_{j}c_{j}x^j=\sum_{j=i+k}a_{i}b_{k}
\end{gather}$$
>>>>[!EXAMPLE]+ Esempio pratico di prodotto tra polinomi
>>>>$$\begin{gather} a(x) = 1 + 2x + 3x^2 \qquad a_{0}=1 \quad ,a_{1}=2\quad,a_{2}=3  \\
b(x) = 5+10x \qquad a_{0}=5\quad,a_{1}=10 \\ \\
c_{0} =a_{0}b_{0} = 1*5=5 \\
c_{1}=a_{0}b_{1}+a_{1}b_{0}=(1*10)+(2*5) = 10 + 10 = 20 \\
c_{2}=a_{0}b_{2}+a_{1}b_{1}+a_{2}b_{0} = (1*0) + (2*10) + (3*5) = 20 + 15 = 35 \\ 
\text{Ricordiamo che }b_{2}=0 \\ \\
c_{3} = a_{1}b_{2} + a_{2}b_{1} + a_{3}b_{0} = (2 * 0) + (3*10) + (0 * 5) = 30  \\
\text{ricordiamo che } a_{3},b_{3},b_{2}=0 \\  \\
c(x) = 5 + 20x + 35x^2 + 30x^3 
\end{gather}$$
>>
>
>>[!approfondimento]+ Funzione polinomiale
>>Ad ogni polinomio è assegnata una funzione polinomiale
>>
>>$F : A \rightarrow A \text{ (Dove A = K)}$ è definita con la mappatura$b \longrightarrow a_{n}b^n+\dots+a_{1}b+a_{0}\in A$ 
>>(questa operazione viene chiamata **valutazione di un polinomio**)
>>
>>- $a_{n}$ è il coefficiente del termine di grado n del polinomio $a(x)$
>>- $b^n$ rappresenta l'elemento b (preso dal #Campo K o #Anello A) moltiplicato per se stesso $n$ volte
>>
>>>[!INFO] Precisazioni
>>>- **Corrispondenza Biunivoca su Campi Infiniti:** 
>>>  Nel caso in cui i polinomi siano definiti su un **campo infinito**  esiste una **corrispondenza biunivoca** tra le funzioni polinomiali e i polinomi. In pratica, nei campi finiti , polinomi diversi = funzioni diverse
>>>- **Mancanza di Corrispondenza Biunivoca su Campi Finiti:** 
>>>  In generale, tuttavia, questa corrispondenza biunivoca **non è vera**.
>>>>[!EXAMPLE]- Spiegazione pratica
>>>>$$\begin{gather} K = \mathbb{F_{2}}=\{0,1\} \\
a(x) = x^2 - x \qquad a(x) \in K[x] \\
a(0) = 0^2 - 0 = 0 \\
a(1) = 1^2 - 1 = 0
\end{gather}$$
>>>>$a(x) = x^2-x$ non è il polinomio nullo, tuttavia , la funzione polinomiale associata è quella nulla essendo che restituisce 0 per ogni possibile input di $K$
>
>>[!approfondimento]+ Grado di un polinomio
>>Data la [[#^polinomio-rappresentazione-formale | rappresentazione formale di un polinomio]].
>>
>>Il **grado di un polinomio non nullo**  è definito come  , il massimo numero intero n tale che $a_{n}\not=0$ 
>>- Indicheremo come **coefficiente direttivo** di $a(x)$ il coefficiente del termine di grado massimo $a_{n}$
>>- Indicheremo con $deg(a(x))$ il **grado di un polinomio non nullo**
>>- Indicheremo i polinomi di <u>grado 0 incluso il polinomio nullo</u> come **polinomi costanti**
>>
>>>[!INFO] Osservazioni
>>>- Il grado della somma di 2 polinomi non può superare il grado massimo di $a(x)$ e $b(x)$ , può però essere minore
>>>  $$\begin{gather} a,b\in K[x] \\
deg(a+b) \leq max(deg(a),deg(b)) \leq deg(a) + deg(b)
\end{gather}$$ 
>>>- Il grado del prodotto di 2 polinomi è uguale alla somma del grado dei 2 polinomi
>>>  $$\begin{gather} a,b \in K[x] \\
deg(a\cdot b)=deg(a)+deg(b)
\end{gather}$$  
>>>- $deg(0) = -\infty$
>>>  
>>
>>
