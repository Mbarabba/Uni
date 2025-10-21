>[!definizione] Processi
>>[!approfondimento]- Cos'è un processo?
>>Un processo è un entità astratta definita dal sistema operativo al fine di eseguire un programma, questo è necessario visto che il numero di programmi da eseguire è superiore rispetto al numero di CPU del sistema. ^def-processo
>>
>>>[!INFO] &nbsp
>>Possiamo considerare un processo come una versione virtuale di una macchina di Von Neumann
>>- Ha una sua CPU dedicata (virtuale)
>>- Ha un area di memoria dedicata
>>- Ha anche le altre risorse astratte (files, I/O , ...) ma condivise con gli altri processi
>>
>
>
>>[!approfondimento]- **PROGRAMMA VS PROCESSO**
>>- Un **programma** <u>è un entità passiva</u> (insieme d'istruzioni) mentre un **processo** <u>è un entità attiva</u> (esecutore di un programma o un programma in esecuzione)
>>- <u>Un programma può dare origine a più processi</u>
>
>>[!approfondimento]- Struttura di un processo
>>Un processo è composto da diverse parti:
>>- Lo stato dei registri del processore che esegue il programma , incluso il program counter (PC)
>>- Lo stato della **immagine del processo** , ossia adlla regione di memoria centrale usata dal programma
>>	- Processi distinti hanno immagini distinti
>>- Le risorse del sistema operativo in uso al programma
>>	- Le risorse del sistema operativo possono essere condivise tra processi
>>- Varie informazioni sullo stato del processo
>>
>>>[!sub-appro]+ Immagine di un processo
>>> L'intervallo di indirizzi di memoria da cui è costituita l'immagine di un processo è anche detto **spazio di indirizzamento** del processo
>>> 
>>> L'immagine di un processo di norma contiene : 
>>> - Text section (dimensione costante) : Contiene il codice macchina del programma
>>> - Data section (dimensione costante) : Contiene le variabili globali
>>> - Heap (dimensione variabile) : Contiene la memoria allocata dinamicamente durante l'esecuzione
>>> - Stack delle chiamate (dimensione variabile) : contiene parametri, variabili locali e indirizzo di ritorno delle varie procedure che vengono invocate durante l'esecuzione del programma
>>> ![[Drawing 2025-10-17 15.11.11.excalidraw]]
>
>>[!approfondimento]- Operazioni sui processi
>>I sistemi operativi di solito **forniscono delle <u>chiamate di sistema</u> con le quali si possono creare/gestire processi**
>>
>>Dal momento che **solo un processo può creare un altro processo**, <u>all'avvio del sistema operativo vengono creati dei processi "primordiali"</u> dai quali tutti gli altri processi vengono progressivamente creati
>>
>>Le operazioni più importanti per la gestione dei processi sono :
>>- Creazione di processi
>>	- La relazione padre / figlio è di norma importante per le politiche di condivisione e risorse e di coordinazione tra processi
>>- Terminazione di processi
>>	- I processi di regola richiedono esplicitamente la propria terminazione al SO
>>	- Un processo padre può attendere o meno la terminazione di un figlio
>>	- Un processo padre può forzare la terminazione di un figlio
>>
>>>[!EXAMPLE]- Albero di processi in Linux
>>>![[Pasted image 20251019132627.png]]
>>
>>>[!info]- [[API POSIX#^operazioni-processi| API POSIX per le operazioni su processi]]
>>>>[!sub-appro]+ Processi zombie e orfani
>>>>-  Processi #zombie
>>>>	- Se un processo termina ma il padre non lo sta aspettando (non ha invocato #wait ) il processo è detto **zombie** , <u>le sue risorse non possono essere completamente deallocate</u> (il padre  potrebbe prima o poi invocare #wait )
>>>>- Processi #orfani 
>>>>	- Se un processo padre termina prima del figlio , allora il figlio diventa **orfano** <u>non essendoci terminazione a cascata</u> 
>
>>[!approfondimento]-  Comunicazione interprocesso
>>I processi possono essere indipendenti o cooperare, delle possibili motivazione per collaborare sono :
>>- Condivisone di informazioni
>>- Accelerazione computazioni
>>- Modularità ed isolamento
>>	- Modularità : Questo concetto implica la suddivisione di un'applicazione complessa in componenti logici distinti (moduli), ciascuno eseguito come un processo separato
>>	- Isolamento : Utilizzando processi separati per questi moduli, si sfrutta la separazione intrinseca che il sistema operativo garantisce tra i processi
>>
>>Per permettere ai processi di cooperare il sistema operativo deve mettere a [[IPC - Interprocess Communication | disposizione primitive di comunicazione interpocesso (IPC)]]

>[!definizione] Multithreading
>>[!approfondimento]- Cos'è un Thread?
>>Un **thread** è un **percorso di esecuzione concorrente** all'interno di un processo.
>>
>>A livello fondamentale, **ogni singolo thread è un flusso di esecuzione sequenziale** delle istruzioni del programma.
>
>>[!approfondimento]- [[Processi e MultiThreading#^def-processo | Processi]] single e multithreaded
>>I thread di uno stesso processo condividono la memoria globale(data) e le risorse ottenute dal sistema operativo
>>
>>Ogni thread di uno stesso processo però deve avere un proprio stack, altrimenti le chiamate a subroutine di un thread interferirebbero con quelle di un altro thread concorrente
>>
>>![[Pasted image 20251019151236.png]]