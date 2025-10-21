>[!definizione] Cos'è un Linguaggio di programmazione - #LP
>Un linguaggio di programmazione è un insieme che definiscono :
>1. Un insieme di stringhe legali , che vengono definite come programmi
>2. L'attribuzione di un preciso significato a ogni stringa legale
>
>Un linguaggio di programmazione è definito a prescindere dai dettagli dello specifico dispositivo che eseguirà i programmi, sebbene alcune caratteristiche implementative possano condizionare i risultati.

>[!definizione]+ Componenti di un LP
>I linguaggi di programmazione sono definiti da 3 componenti che ne definiscono la forma e il significato
>>[!approfondimento]+ #Sintassi
>>Descrive come le parole possono essere combinate per formare istruzioni legali, definendo la forma delle espressioni e delle istruzioni.
>>
>>La sintassi è specificata da una [[Grammatica#^4dd5ed | grammatica formale]] e definisce il #parser del #compilatore
>
>>[!approfondimento]+ Semantica
>>Descrive il significato di una frase sintatticamente corretta , ovvero cosa succede durante l'esecuzione.

>[!definizione]+ Caratteristiche - **Criteri di qualità**
>>[!approfondimento]- Leggibilità
>>La facilità attraverso cui **riesco a leggere ed interpretare un programma**
>>
>>>[!INFO]- Fattori di leggibilità
>>>>[!sub-appro] Semplicità complessiva
>>>>Un linguaggio dovrebbe avere un insieme gestibile di caratteristiche e costrutti, riducendo al minimo la molteplicità delle funzionalità e l'overloading degli operatori
>>>
>>>>[!sub-appro] Ortogonalità
>>>>Indica se un piccolo insieme di costrutti primitivi può essere combinato in un numero relativamente limitato di modi per definire istruzioni di controllo e strutture dati.
>>>>
>>>>Un linguaggio ortogonale garantisce che ogni combinazione possibile di primitive sia legale, riducendo la necessità di controlli sintattici e la probabilità di eccezioni
>>>
>>>>[!sub-appro] Tipi di dati
>>>
>>>>[!sub-appro] Considerazioni sintattiche
>>>>Riguardano la forma degli identificatori, la composizione flessibile, l'uso di parole speciali o metodi per formare istruzioni composte , e l'impiego di costrutti auto-descrittivi o parole chiave significative
>>
>
>>[!approfondimento]- Facilità di sviluppo
>>La facilità con cui un linguaggio può essere utilizzato per **creare programmi**
>>>[!INFO]- Fattori di facilità di sviluppo
>>>>[!sub-appro] Semplicità e ortogonalità
>>>>Pochi costrutti, un ridotto numero di primitive e un piccolo insieme di regole per combinarle sono fondamentali
>>>
>>>>[!sub-appro] Supporto per l'astrazione
>>>>La capacità di definire e utilizzare strutture complesse o operazioni in modi che permettano di ignorare i dettagli implementativi
>>>
>>>>[!sub-appro] Espressività
>>>>L'uso di operatori potenti per specificare le operazioni in modo compatto e la disponibilità di operatori e funzioni predefinite potenti
>
>>[!approfondimento]- Affidabilità
>>L'affidabilità indica la **conformità alle specifiche del linguaggio**, ovvero la capacità di funzionare secondo quanto specificato
>>>[!INFO]- Fattori di affidabilità
>>>>[!sub-appro] Controllo dei tipi
>>>
>>>>[!sub-appro] Gestione delle eccezioni
>>>
>>>>[!sub-appro] Restrizione dell'Aliasing
>>>>La presenza di due o più metodi distinti per riferirsi alla stessa posizione di memoria, può ridurre l'affidabilità. Restringere l'aliasing aumenta l'affidabilità
>>>
>>>>[!sub-appro] Leggibilità e facilità di sviluppo
>
>>[!approfondimento]- Costo

>[!definizione]+ Classificazione e Categorizzazione
>I linguaggio di programmazione possono essere classificati in base al paradigma supportato o in base alla complessità della [[Grammatica#^gerarchia-chomsky | grammatica che li definisce]]
>>[!approfondimento]+ Classificazione per paradigmi
>>I linguaggi di alto livello sono **raggruppati in base allo stile di programmazione che usano**
>>
>>Un linguaggio di programmazione **può far parte di più paradigmi** di programmazione
>>>[!sub-appro]- Linguaggi Imperativi
>>>Il programma è una sequenza di istruzioni che realizzano trasformazioni di stato.
>>>
>>>Le variabili sono modellate come locazioni di memoria (celle), riflettendo l'architettura di Von Neumman
>>>>[!EXAMPLE] Elenco di linguaggi imperativi
>>>>- C
>>>>- C++
>>>>- Java
>>>>- Perl
>>>>- JavaScript
>>>>- VISUAL BASIC .NET
>>
>>>[!sub-appro]- Linguaggi Funzionali
>>>Un programma è **un espressione che viene valutata**.
>>><u>Il calcolo avviene tramite l'applicazione di funzioni a parametri</u>
>>>>[!EXAMPLE] Elenco di linguaggi funzionali
>>>>- LISP
>>>>- Scheme
>>>>- ML
>>>>- F#
>>>>- Haskell
>>>>- Julia
>>
>>>[!sub-appro]- Linguaggi Logici
>>>Il programma è un insieme di fatti e regole specificate senza un ordine particolare , l'esecuzione è l'equivalente alla realizzazione di una dimostrazione 
>>>>[!EXAMPLE] Lista linguaggi logici
>>>>- Prolog
>>
>>>[!sub-appro]- Linguaggi a Oggetti (Object Oriented)
>>>Un programma è **un insieme di oggetti** che comunicano tra di loro scambiando messaggi 
>>>>[!EXAMPLE] Lista linguaggi a oggetti
>>>>- Java
>>>>- C++
>>>>- Python
>>
>>>[!sub-appro]- Linguaggi di Scripting
>>>Categoria che include linguaggi interpretati, spesso usati per lo sviluppo Web
>>>>[!EXAMPLE] Lista linguaggi di scripting
>>>>- JavaScript
>>>>- PHP
>>>>- Python
>>
>>>[!sub-appro]- Linguaggi ibridi/**Markup**
>>>Linguaggi di markup estesi per supportare funzionalità di programmazione
>>>>[!EXAMPLE]
>>>>- HTML
>>
>>
>>
>>
>>
>
>>[!approfondimento]+ Classificazione per grammatica

>[!definizione] Metodi di Implementazione
>