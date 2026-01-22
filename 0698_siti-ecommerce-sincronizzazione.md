# SITI ECOMMERCE -- SINCRONIZZAZIONE



In un sito Ecommerce la procedura di **Sincronizzazione** è quella
particolare operazione che consente a Passweb, tra le altre cose, di:

- Valorizzare, all'interno dell'applicazione web, con i dati presenti
  sul gestionale, solamente quei campi della struttura dati che si è
  effettivamente deciso di utilizzare e che in qualche modo sono stai
  variati rispetto all'ultima sincronizzazione

- Prelevare dal gestionale i pagamenti abituali dei vari clienti

- Prelevare dal gestionale i dati della tabella listini

- Prelevare dal gestionale i dati della tabella valute l

- Prelevare dal gestionale le condizioni commerciali dei singoli clienti

- ...

In poche parole dunque mentre la precedente funzione di Aggiornamento
Attributi si preoccupa di rendere disponibili in Passweb gli stessi
campi e le stesse tabelle disponibili in Mexal, lasciando poi all'utente
la libertà di decidere quali di questi utilizzare realmente, **la
funzione di sincronizzazione si occupa invece, sotto questo punto di
vista, di verificare quelli che sono i campi Mexal effettivamente
utilizzati all'interno del sito e di prelevare il valore che essi hanno
in Mexal.**

Oltre a questo l'operazione di sincronizzazione si preoccuperà anche di:

- Inserire eventuali nuovi ordini o clienti all'interno del gestionale

- Riportare all'interno del sito eventuali variazioni effettuate sul
  gestionale a documenti (ordini) non ancora evasi in maniera completa.

- Aggiornare le categorie merceologiche

- Riportare ed aggiornare all'interno del sito le risorse (immagini e
  schede tecniche) associate mediante Docuvision ai vari articoli
  gestiti

- ....

A differenza della procedura di Aggiornamento Attributi, che come visto
è unica e può essere lanciata solo ed esclusivamente da Passweb,
esistono **tre diversi tipi di sincronizzazione (Sincronizzazione
Totale, Sincronizzazione Variati, Sincronizzazione Parziale)** che, a
seconda dei casi, possono essere lanciate solo da Passweb, solo da Mexal
o da entrambi gli applicativi.

**ATTENZIONE!** Nel caso di siti collegati ad uno dei gestionali
Ho.Re.Ca. la sincronizzazione, indipendentemente dal fatto che sita
Totale, Variati o Parziale, quando non eseguita automaticamente, potrà
essere lanciata solo ed esclusivamente dal Back End del sito.

