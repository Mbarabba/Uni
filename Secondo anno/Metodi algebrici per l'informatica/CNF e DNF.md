# Cosa sono CNF e DNF?

Sono  forme attraverso cui possiamo esprimere una qualsiasi formula booleana ad n-variabili

Prendiamo $B_{1}=\{0,1,x,1+x\}$

 Poniamo come $V = \{(v_{1}\dots v_{_{n}}): v_{i}\in j\{0,1\}\}$  l'insieme costituito da tutte le liste dei valori di verità attribuibili alle proposizioni a cui da cui dipende la fbf
 
 Poniamo come $W \subsetneq V , W = \{v\in V:f(v)=0\}$l'insieme delle liste che **rendono la formula falsa**

>[!CNF : Forma normale congiuntiva]+
>Definizione breve : Congiunzione di disgiunzioni inclusive nelle loro variabili e nelle loro negazioni
>>[!Definzione estesa]-
>>Sia f una fbf allora f può essere espressa come f = $\wedge$ disgiunzioni (la congiunzione di disgiunzioni) dove disgiunzioni =$t_{1}(x_{1})\wedge t_{2}\lor \dots\lor t_{(n)}(x_{n})$ dove n è il numero di proposizioni coinvolte in f , $t_{i}$ posso essere : id (identità) , $\lnot$(negazione)
>
>>[!Formula]+
>>Definiamo come $d=d_{0}=\bigvee_{i=1}^n v_{i}^*(x_{i})$ il polinomio ottenuto disgiungendo le variabili.
>>Preso $v\in V$ poniamo :$$
>>\begin{gather}
d_{v}=\bigvee_{i=1}^n=v_{i}^*(x_{i}) \\
\end{gather} \\ $$
>>dove $v_{i}^* = id \text{ se e solo se } v_{i}=0 \text{ , } \lnot$ altrimenti.
>>Queste sono esattamente le funzioni booleane che compaiono come fattori in CNF.
>>
>>Si definisca per $W\subseteq V$
>>$$\begin{gather}
p_{W} = \prod_{W}dw=\bigwedge_{W}dw
\end{gather}$$
In particolare $p_{{\{v\}}}=d_{v}$ per $v\in V$



>[!DNF : Forma normale disgiuntiva]+
>Definizione breve : Disgiunzioni inclusive di congiunzioni nelle loro variabili e nelle loro negazioni
>>[!Definzione estesa]-
>>Sia f una fbf allora f può essere espressa come f = $\lor$ congiunzioni (la disgiunzione di congiunzioni) dove congiunzioni = $t_{1}(x_{1})\wedge t_{2}\wedge \dots\wedge t_{(n)}(x_{n})$ dove n è il numero di proposizioni coinvolte in f , $t_{i}$ posso essere : id (identità) , $\lnot$(negazione)