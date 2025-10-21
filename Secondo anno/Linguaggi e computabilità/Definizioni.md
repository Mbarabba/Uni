> [!Linguaggio]-
 >- #Linguaggio : Un insieme di #parole che può essere **finito o infinito**
 >  >[!INFO]
 >  >**Un linguaggio è regolare se esiste una [[Espressioni Regolari | espressione regolare]] che lo esprime** 
 >	- #Alfabeto($\Sigma$) = Un insieme finito di simboli (o caratteri)
 >		>[!Esempi di alfabeti]-
 >			>- $\Sigma$ = {s1 , s2 , s3}
 >			>- $\Sigma_{c}$(alfabeto delle cifre) = {0 , 1 , 2 , 3 , ...}
 >			>- $\Sigma_{b}$(alfabeto binario) = {0 , 1}
 >			
 >		L'insieme di tutte le parole all'interno di un alfabeto $\Sigma$ è $\Sigma^*$
 >	- >[!Parola]-
 >			>- #parole = **Sequenza finita** di simboli dell'alfabeto $\Sigma$ o la **concatenazione finita** di simboli $\Sigma$
 >			> - Lunghezza di una parola = Prendendo w (word), la sua lunghezza è pari al numero di simboli concatenati
 >			> - Parola Vuota $\varepsilon$ = $\varepsilon$ è una parola con lunghezza pari a 0
 >			
 >	>[!EXAMPLE]- Esempio di problema
 >		>- Tutte le parole che finiscono con 01
 >		>- Tutte le parole che contengono la sottostringa 01
 >		>- Tutte le codifiche binarie di numeri primi
 >		
 
 [[Grammatica]]

 >[!Modello di calcolo]-
 >Un #Modello_di_calcolo è la descrizione formale dell'insieme di operazioni e risorse disponibili
 >>[!Cosa significa calcolare qualcosa?]-
 >>La computazione è una funzione f : Input$\rightarrow$Output
 >
 >- Problema computazionale di **decisione** (Output={si , no})
 >>[!Esempio di problema di problema di decisione]-
 >>**Appartenenza** = Dato $L\subseteq$$\Sigma^*$ , $w\varepsilon$$\Sigma^*$ calcolare se $w\varepsilon L$
 >
 >>[!Esempio di un problema]-
 >>Calcolare la somma di 2 numeri interi a,b
 >>Posso considerare questo problema come un insieme di problemi di decisione
 >>Problema di decisione : Dati $a,b \varepsilon N$, $i \varepsilon N$ il bit i-esimo di a+b è 1? 

[[DFA - Automi deterministici a stati finiti]]
[[NFA - Automi non deterministici a stati finiti]]
[[Ɛ-NFA - Automa a stati finiti non deterministico con le Ɛ mosse]]
[[Espressioni Regolari]]