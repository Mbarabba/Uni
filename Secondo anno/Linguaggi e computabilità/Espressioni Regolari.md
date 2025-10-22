>[!definizione]+ Cosa sono?
>Un espressione regolare è una "espressione algebrica" finalizzata alla rappresentazione del #Linguaggio 
>

>[!definizione] Come le uso?
>- L'algebra che utilizzeremo sarà applicata su $\Sigma$.
>- $a \in \Sigma$ , per ogni carattere $a$, l'espressione regolare $a$ è lecita/regolare , $L(a)=\{a\}$ Il linguaggio che associo all'espressione $a$ è l'insieme $\{a\}$  
>- Date $E_{1},E_{2}$ è valida la costruzione $E_{1}|E_{2}$  
>  $L(E_{1}|E_{2})=L(E_{1})\cup L(E_{2})$
>- Date $E_{1},E_{2}$ , $E_{1}E_{2} \implies L(E_{1}E_{2} ) = \{w_{1}w_{2}:w_{1}\in L(E_{1}) \quad w_{2}\in L(E_{2})\}$ 
>- Data $E^*$ ($^* = \text{Chiusura di Kleene}$) , ripeto 0 o più volte l'espressione marcata 
>  
>>>[!definizione]
> 