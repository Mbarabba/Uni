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