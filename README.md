Gioca numeri 
il progetto GiocaNumeri è un programma Java che simula un gioco semplice in cui due giocatori inseriscono numeri. L’obiettivo principale è educativo: mostrare come si utilizzano i thread, i
costruttori e l’interazione tra oggetti in Java. Ecco come funziona il gioco: quando avvii il programma, viene creato un oggetto della classe GestoreGioco, che contiene il numero vincente e un
metodo per verificarlo. Questo numero vincente è impostato a un valore fisso nel costruttore, mentre un costruttore di copia consente a ciascun giocatore di avere la propria istanza del gestore,
evitando così la condivisione diretta dello stesso oggetto. I giocatori sono rappresentati dalla classe Giocatore, che estende Thread. Ogni giocatore ha un nome e un riferimento a un
GestoreGioco. Quando il thread parte, il giocatore si presenta, aspetta qualche secondo, chiede all’utente di inserire un numero e poi lo invia al gestore, che verifica se corrisponde al numero
vincente. A seconda del risultato, il giocatore riceve un messaggio che dice “ho vinto” o “ho perso”. La classe GiocaNumeri contiene il metodo main e si occupa di avviare il gioco. Viene creato il
gestore, due giocatori vengono istanziati e avviati come thread concorrenti. Il programma utilizza il metodo join per aspettare che entrambi i thread finiscano l’esecuzione prima di terminare,
assicurando che il gioco si concluda solo quando tutti i giocatori hanno partecipato. Questo progetto mette in luce concetti chiave della programmazione concorrente e della programmazione
orientata agli oggetti, come l’uso di costruttori, la copia di oggetti e la gestione dell’input da tastiera. Ci sono alcuni aspetti che potrebbero essere migliorati: ad esempio, l’uso di Scanner in più
thread può creare problemi, e il numero vincente è fisso invece di essere generato casualmente.
