>[!definizione]- Algoritmo di <u>divisione per numeri interi</u>
>>[!approfondimento] Cosa fa?
>>Stabilisce che dati 2 interi $a(dividendo),b(divisore)$ con $b \not= 0$, è sempre possibile trovare 2 interi unici $q(quoziente),r(resto)$
>
>>[!approfondimento] Come lo fa?
>>Siano $a,b \in \mathbb{Z},\quad b\not=0$
>>
>>Allora esistono e sono unici $q,r \in \mathbb{Z}$ tale che :
>>1. $a = bq+r$
>>   Il numero da dividere ($a$) è uguale al divisore ($b$) moltiplicato per il quoziente ($q$) più il resto ($r$).
>>   
>>2. $0 \leq r < |b|$
>> Il **resto $r$** non deve essere nullo e, allo stesso tempo, deve essere **più piccolo del divisore $b$**.
>>>[!EXAMPLE] Esempio pratico
>>>Determinare il quoziente$(q)$ ed il resto$(r)$ della divisione tra $a=397(dividendo)$ , $b=17(divisore)$
>>>
>>>$$\begin{gather} \\
\text{Passo 1} \qquad \frac{397}{17} \rightarrow q=23 , r=6 \\ \\
\text{Passo 2} \quad a = 397 \quad 17\cdot 23 + 6 = 397 \quad \checkmark \\ \\
\text{Passo 3} \quad r = 6 \quad 0 \leq 6 < 17 \quad \checkmark \end{gather}$$
>
>>[!approfondimento]- Dimostrazione <u>(Da rifare)</u>
>>La dimostrazione deve provare 2 cose:
>>- Che $q\text{(quoziente)}$ e $r\text{(resto)}$ **esistono**
>>- Che $q\text{(quoziente)}$ e $r\text{(resto)}$ **sono unici**
>>  
>>>[!sub-appro] Esistenza
>>>$$\text{Sia } R=\{a-bq:q\in \mathbb{Z}\}\cap \mathbb{N}$$
>>>Questo insieme $\mathbb{R}$è formato da tutti i numeri non negativi ottenibili sottraendo multipli interi di $b(\text{divisore})$ da $a(\text{dividendo})$
>>>
>>>Siccome $a\in R\rightarrow R\not=\emptyset$ ed $R\subseteq \mathbb{N}$ per il principio di **induzione**, <u>che equivale al principio del buon ordinamento in $\mathbb{N}$</u> esiste almeno un elemento $r=min(R)$
>>>
>>>Se fosse $r=a-bq \geq b$, potrei scrivere $0 \leq r-b=a-(q+1)b<r$, contro la minimalità di r. Quindi $0 \leq r<b$.
>>>
>>>Sia $a<0$ allora , per il caso precedento , esistono $q',r'\in \mathbb{Z}$ tali che $-a=bq'+r'$, $0\leq r<b$.
>>>Se $r'=0$, allora $a=bq$ con $q=-q'$.
>>>Altrimenti $r'>0$ e $a=-b(q'+1)+(b-r')$ e l'asserto è verificato con $q=-(q'+1)$ e $r=br'$.
>>>
>>>Sia ora $a=bq + r = bq' + r'$con $r \geq r'$, allora $b|(r-r')$, ma $r-r'<b$ quindi $r=r'$ e , di conseguenza $q'=q$. 

>[!definizione]- Divisione di polinomi
>>[!approfondimento] Cosa fa?
>>La divisione tra polinomi stabilisce l'esistenza e l'unicità di un quoziente e di un resto, in modo analogo all'algoritmo di divisione per gli interi.
>>
>>Per **2 polinomi** $a(x)\text{ (dividendo) e } b(x) \text{ (divisore) in }K[x]$ esistono e sono univocamente determinati
>
>>[!approfondimento] Come lo fa?
>>Dato un polinomio $a(x)=\sum_{i=0}^na_{i}x^i\in K[x] \text{ con }a_{n}\not=0$ chiamo:
>>- $LT(a)=a_{n}x^n$ **termine direttivo**
>>- $LC(a)=a_{n}$ **coefficiente direttivo**
>>
>>Sia $K$ un #Campo e $a,b\in K[x]$ con $b \not=0$, allora **esistono** <u>e sono univocamente determinati</u> $q,r\in A$ tali che: 
>>1. $deg(r)<deg(b) \text{ (include il caso }r=0_{K[x]}\text{)}$
>>2. $a=bq+r$
>>>[!EXAMPLE]- Esempio pratico
>>>$$a(x)= 2x^3+x^2-3x+5\qquad b(x)=3x^2-2$$  
>> 
>
>>[!approfondimento]- Dimostrazione