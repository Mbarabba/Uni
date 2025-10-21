>[!definizione] Cos'è e a che cosa serve un sistema operativo?
>Il sistema operativo ( #SO in breve) **è il primo programma che viene caricato ed eseguito**.
>
>Fondamentalmente , **è un insieme di programmi che ci permette di gestire gli elementi hardware  ed i vari software installati su di esso**.
>
>>[!approfondimento]+ Componenti di un sistema di elaborazione
>>![[Drawing 2025-10-17 09.31.02.excalidraw]]
>>- Utenti : Gli utenti si dividono in 3 sottocategorie
>>	- Umani 
>>	- Altri computer
>>	- Processi Automatizzati 
>>- Programmi Applicativi : Questo strato funge tra intermediario tra l'utente e il #SO , è ciò che l'utente "usa" per essere produttivo
>>- #SO : È il software più importante, che gestisce e coordina tutte le altre componenti
>>- Hardware : È la base fisica e tangibile del computer, l'insieme di tutte le componenti elettroniche e meccaniche

>[!definizione] Politiche e Meccanismi
>>[!approfondimento]+ Meccanismo
>>Un Meccanismo **spiega come una certa operazione è effettuata**
>>
>>I meccanismi sono più stabili delle politiche , esse infatti , cambiano a seconda delle caratteristiche percepite che vogliamo che il sistema di elaborazione abbia 
>
>>[!approfondimento]+ Politica
>>Una Politica **dice cosa deve essere fatto in determinate situazioni**
>>
>>Le politiche impattano profondamente sulle caratteristiche percepite del sistema di elaborazione a differenza dei meccanismi
>>
>>Avere politiche configurabili è utile per combattere la maledizione della generalità

>[!definizione]+ Struttura e servizi dei #SO 
>>[!approfondimento]+ Struttura dei #SO 
>>![[Drawing 2025-10-17 12.48.20.excalidraw]]
>>Non c'è una definizione universalmente accettata di quali programmi fanno parte di un sistema operativo , in generale però un sistema operativo comprende almeno :
>>>[!sub-appro]+ #kernel
>>>Il kernel **è il nucleo centrale del sistema operativo**, è il primo programma che viene caricato all'avvio del computer e rimane sempre in esecuzione.
>>>
>>>>[!INFO] Precisazione
>>>>Con "rimane sempre in esecuzione" intendiamo che rimane in uno stato di "sospensione reattiva", è sempre caricato in memoria , ma non sta costantemente elaborando, "fa qualcosa solo se interpellato"
>>>
>>>**Agisce come ponte tra il software e l'hardware,<u> gestendo in modo sicuro e controllato tutte le risorse del computer </u>** decidendo quale programma può usare la CPU , quanta memoria allocare e come accedere ai dispositivi
>>
>>>[!sub-appro]+ #middleware
>>>Il middleware è lo strato di software che agisce come un ponte o un traduttore universale tra le diverse applicazioni e il sistema operativo .
>>>
>>>>[!INFO] Compito
>>>>Il suo scopo è quello di far comunicare e collaborare programmi e servizi diversi tra di loro che altrimenti non potrebbero comunicare tra di loro date le loro differenza
>>>
>>>>[!EXAMPLE]+ Esempi di programmi middleware
>>>>- API
>>>>- Framework per grafica
>>>>- Framework per suono
>>
>>>[!sub-appro]+ Programmi di sistema
>>>I programmi di sistema sono l'insieme di strumenti e utility che vengono forniti insieme al sistema operativo per aiutare l'utente e gli sviluppatori a gestire ed interagire col computer
>>>
>>>>[!EXAMPLE] Esempi di programmi di sistema
>>>>- GUI - Graphic User Interface 
>>>>- CLI - Command Line Interface
>>>>- Task Manager
>>>>- File Explorer
>>
>>Alcuni SO forniscono anche dei programmi applicativi (editor di codice  / testo , fogli di calcolo ...) ma non li consideriamo parti del sistema operativo
>
>>[!approfondimento] Servizi offerti da un sistema operativo
>>Un sistema operativo offre un certo numero di servizi:
>>- Per i programmi applicativi : Cosi' che possano eseguire sul computer usando le risorse astratte fornite dal sistema operativo
>>- Per gli utenti: Cosi' che possano gestire l'esecuzione dei programmi e stabilire quali risorse hardware i programmi possono usare
>>- Per garantire che il sistema di elaborazione funzioni in maniera efficiente
>>  
>>Gli utenti però interagiscono con il sistema operativo attraverso i programmi di sistema , i quali , utilizzano gli stessi servizi dei programmi applicativi , portando cosi' la necessità da parte del sistema operativo di esporre i suoi servizi esclusivamente ai programmi
>>
>>>[!EXAMPLE]+ Esempi di servizi di sistema
>>>- Controllo processi : Permettono di caricare/esegurile/identifica la terminazione / registrare la condizione di terminazione di un programma
>>>- Gestione file : Permettono di leggere/scrivere/manipolare files e directory
>>>- Gestione dispositivi : Permettono di eseguire operazioni di I/O
>>>- Comunicazione tra processi : Permette la collaborazione e lo scambio di informazioni tra processi
>>>- Protezione e sicurezza
>>>- Allocazione delle risorse
>>>- Rilevamento errori
>>>- Logging : Mantenere traccia di quali programmi utilizzano quali risorse

>[!Definizione]+ Chiamate di sistema ed #API 
>![[Drawing 2025-10-17 14.09.40.excalidraw]]
>>[!approfondimento] Chiamate di sistema
>>Il #kernel offre i propri servizi ai programmi come **chiamate di sistema**
>>
>>Le chiamate di sistema sono delle procedure invocabili da un programma (attraverso un #API) attraverso cui può richiedere un servizio del kernel al sistemo operativo
>
>>[!approfondimento] API - Application Program Interface
>>Un #API (Interfaccia di programmazione delle applicazioni) è una libreria di #middleware utilizzata dai programmi per accedere ai servizi del sistema operativo ed accedere indirettamente alle chiamate di sistema del #kernel 
>
>>[!sub-appro]+ Chiamate di sistema VS #API 
>>- Le API sono esposte dal middleware , chiamate di sistema dal #kernel 
>>- Le API sono implementate in linguaggi di alto livello, le chiamate di sistema attraverso linguaggi di alto livello e assembler
>>- Le API invocano le chiamate di sistema nella loro implementazione
>>- Le API sono standardizzate , le chiamate di sistema cambiano da kernel a kernel
>>- Le API sono stabili, le chiamate di sistema possono cambiare comportamento in base alla versione del SO
>>- Le API hanno funzionalità di alto livello e sono facili da chiamare
>>- Un SO può offrire più API di standard diversi