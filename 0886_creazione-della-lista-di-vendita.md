# CREAZIONE DELLA LISTA DI VENDITA



Il processo di creazione di una lista di vendita per la pubblicazione di
articoli a taglie / colori o comunque con un massimo di due elementi
varianti, è sostanzialmente analogo a quello utilizzato per la creazione
di una normale lista di vendita utilizzata per la pubblicazione di
semplici articoli di magazzino.

L'unica differenza in tal senso è dettata dal fatto che, come
evidenziato nei precedenti capitoli di questo manuale, **le inserzioni
configurate per gestire articoli con varianti potranno essere utilizzate
solo ed esclusivamente per pubblicare questa particolare tipologia di
articoli**.

Dipendentemente da come è stata configurata la specifica inserzione,
all'interno della Lista di Vendita ad essa collegata potranno quindi
essere inseriti:

- **Articoli a Taglie / Colori**

- **Articoli padri di struttura**

- **Articoli figli di apposite strutture correttamente esportati e
  gestiti anche all'interno del sito Passweb**

In particolare:

- Nel caso in cui l'Inserzione collegata alla lista in esame sia stata
  configurata **con un solo elemento di variazione che corrisponde alla
  tabella Taglie Colori di Mexal**, **in lista andranno inseriti
  solamente articoli a taglie gestiti con la stessa tabella**. In queste
  condizioni Passweb esploderà la Tabella Taglie di Mexal inserendo in
  lista un articolo per ogni taglia presente nella corrispondente
  tabella gestionale

- Nel caso in cui l'Inserzione collegata alla lista in esame sia stata
  configurata **con un solo elemento di variazione che corrisponde
  all'ultimo campo di una struttura, in lista andranno inseriti
  direttamente tutti i figli già codificati e correttamente esportati**
  e gestiti all'interno del sito Passweb

- Nel caso in cui l'Inserzione collegata alla lista in esame sia stata
  configurat**a con due elementi di variazione che corrispondono alla
  Tabella Taglie di Mexal e all'ultimo campo di una struttura** (il
  classico esempio è quello di articoli a taglie e colori con il colore
  gestito come ultimo campo della struttura e le taglie gestite con
  l'apposita tabella Mexal) **in lista andranno inserti i relativi padri
  Mexal**. In queste condizioni Passweb prenderà comunque in
  considerazione solo ed esclusivamente **articoli figli effettivamente
  esportati e gestiti all'interno del sito** e, in relazione ad ognuno
  di essi, verrà inserito in lista un elemento per ogni taglia indicata
  nella corrispondente tabella Mexal

- Nel caso in cui l'Inserzione collegata alla lista in esame sia stata
  configurata **con due elementi di variazione che corrispondono
  all'ultimo e al penultimo campo di una struttura** (un esempio
  potrebbe essere quello di articoli a taglie e colori con entrambi
  questi elementi gestiti in struttura) **in lista andranno inseriti
  direttamente tutti i figli già codificati e correttamente esportati**
  e gestiti all'interno del sito Passweb

**ATTENZIONE!** Per maggiori informazioni relativamente a come gli
articoli inseriti in lista verranno poi raggruppati all'interno della
piattaforma terza si veda quanto indicato nel capitolo relativo alla
pubblicazione di articoli a taglie e colori della specifica piattaforma

