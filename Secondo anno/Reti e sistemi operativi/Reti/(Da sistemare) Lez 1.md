>[!Cos'è internet?]-
	 >Internet è un agglomerato di dispositivi interconnessi connessi , esso è formato da :
	>- Host : I dispositivi "finali" che ricevono / inviano ed elaborano  #pacchetti 
	>-  Packet switches : Hanno il compito di far circolare i #pacchetti (router , swtich ...)
	>- Collegamenti di comunicazione : Sono il tramite attraverso cui colleghiamo le #interfacce di dispositivi differenti (satellite , fibra ottica ...)
	>- Rete : una collezione di dispositivi / router / switch e collegamenti gestiti da una organizzazione
	>![[Pasted image 20251003115644.png]]
	>Internet è **governata da standard e #protocolli** , gli standard sono tali cosi' da permettere la possibilità di comunicazione tra dispositivi e device diversi
	>>[!Reti di core]-
	>>Sono un insieme di router interconessi che hanno 2 compiti fondamentali.
	>>- Inoltro/Switching : Ogni router è connesso ad n interfacce , nel momento che ricevo un pacchetto su una interfaccia controllo l'indirizzo di destinazione del pacchetto ricevuto attraverso la tabella di inoltro che mi permette di capire a chi devo mandare il pacchetto ricevuto
	>> - Instradamento / Routing : E' un azione globale, questo significa che tutti i router all'interno di una rete al fine di poter instaurare dei percorsi ottimali per la trasportazione dei pacchetti
	>> ![[Pasted image 20251003122607.png]]
	>> Queste 2 funzioni permetto di creare la mia tabella di inoltro cosi' che possa far circolare correttamente i pacchetti ricevuti
	>>>[!Esempio grafico USA]-
	
>[!Cos'è un protocollo?]-
>Un protocollo definisce il formato , l'ordine di invio e ricezione tra le entità di rete e le azione che devono essere effettuate alla trasmissione e ricezione di un messaggio(pacchetto)
>>[!Esempio grafico]-
>>![[Pasted image 20251003121018.png]]
>

>[!Come è strutturata una rete?]-
>Usualmente abbiamo client e server ai bordi della rete collegati attraverso i mezzi di connessione , mentre al centro della rete abbiamo un interconnessione di router e delle reti annidate
>![[Pasted image 20251003121511.png]]![[Pasted image 20251003121530.png]]
>>[!Cosa devono fare gli host?]-
>>>[!Mandare pacchetti]-
>>>- Ricevono i pacchetti per poi dividerli in pacchetti più piccoli di una lunghezza di L (bit)
>>>- Trasmettono i pachetti all'interno della rete un rateo di trasmissione R (bit/secondo)

>[!Pachet Switching]
>>[!Store & forward / Immagazzina ed inoltra]-
>>Prima di inoltrare un pacchetto il router deve obbligatoriamente ricevere completamente il pacchetto 
>>![[Pasted image 20251003123301.png]]
>>(Approfondisci questo esempio e cerca di capire perchè la velocità di trasmissione di 3 pacchetti è 4L/R)
>>Esempio di Diana![[Pasted image 20251003125048.png]]
>
>>[!Queueing / Incodamento]-
>>![[Pasted image 20251003124450.png]]
>>Viene utilizzato quando i pacchetti arrivano con una velocità superiore rispetto alla loro distribuzione, questo porta 2 conseguenze negative:>>
>>- Perdita di pacchetti per colpa dell'overflow dei buffer
>>- Ritardo aumentato

>[!Commutazione di circuito e Commutazione di pacchetto]-
>**Guarda bene sulle slide / chatgpt / libro** / riguarda videolezione
>>[!Circuit switch / Commutazione di cirucito]-
>>![[Pasted image 20251003124608.png]]
>>Ogni collegamento tra sorgente e destinazione ha un n numero di circuiti 
>>Immagina la commutazione di circuito come il sistema dei treni , ogni treno ha un binario designato su cui solo esso può circolare
>
>>[!Commutazione di pacchetto]-
>>![[Pasted image 20251003125422.png]]
>>
>>[!Commutazione di circuito vs Commutazione di pacchetto]-

>[!Struttura d'internet]-
>Abbiamo un numero indefinito di host che accedono ad internet attraverso degli ISP che  sono interconnessi tra di loro creando cosi' un enorme rete globale, ma la struttura della singola rete è abbastanza complessa