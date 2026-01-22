# COMPONENTE ORDINI



Il Componente **"Ordini"** permette di creare un modulo utilizzabile
dagli utenti per controllare lo stato dei propri documenti (ordini,
bolle, fatture, resi, matrici ecc...) e visualizzarne il relativo
dettaglio

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_ordini_res.bmp](./assets/media/image397.png){width="2.1166666666666667in"
height="2.5277777777777777in"}

Può essere inserito

- all'interno della pagina "**Ordini**" -- **obbligatorio per poter
  consentire il corretto funzionamento del sito**

- all'interno di pagine generiche (bianche) -- opzionale

Grazie a questo Componente dunque ogni utente potrà sapere in ogni
istante se il suo ordine è stato evaso interamente o parzialmente, se è
stato bloccato o sospeso, quali articoli in particolare non sono
attualmente disponibili ecc.. .

Tale Componente è dunque di fondamentale importanza per quella che è la
tracciabilità del ciclo di vita dell'ordine e, ovviamente, sarà
accessibile ai vari utenti soltanto dopo aver effettuato
l'autenticazione al sito.

L'intero modulo è gestito in maniera completamente automatica da
Passweb. L'utente non dovrà quindi preoccuparsi di inserire o di
mantenere aggiornati, ad esempio, i collegamenti fra i vari documenti
correlati originati da evasioni parziali di uno stesso ordine, cosi come
non dovrà preoccuparsi di inserire pulsanti relativi alla possibilità di
modificare o annullare eventuali ordini in sospeso.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\componente_ecommerce_ordini_esempio.bmp](./assets/media/image398.png){width="5.177777777777778in"
height="3.4972222222222222in"}

All'interno del componente sono presenti diverse sezioni, organizzate
all'interno di appositi tabs, e utilizzate per raggruppare le diverse
tipologie di documenti gestiti.

In particolare la sezione:

- **Attivi:** contiene i documenti ancora attivi e da elaborare quindi
  ordini e/o preventivi per i quali non sono ancora state emesse
  all'interno del gestionale bolle o fatture

> **NOTA BENE:** si ricorda che i preventivi (documenti PR/PX)
> anch\'essi presenti all\'interno della scheda \"Documenti Attivi\",
> non hanno lo stato di riga e in conseguenza di ciò non potranno mai
> essere modificati dall\'utente.
>
> **NOTA BENE:** nel caso in cui un preventivo (documento PR/PX) venga
> trasformato, all\'interno del gestionale, in Ordine (documento OC/OX),
> sul sito web verrà visualizzato sia il preventivo che l\'ordine
> (entrambi all\'interno della sezione \"Documenti Attivi\").

- **Bollati:** contiene tutte le bolle (documenti di trasporto) generate
  a partire da ordini effettuati sul sito o esportate direttamente dal
  gestionale

- **Fatturati:** contiene tutte le fatture e/o i corrispettivi generati
  a partire da ordini effettuati sul sito o esportate direttamente dal
  gestionale

- **Resi:** contiene tutti di documenti di reso (RC) relativi a
  richieste di reso merce approvate e/o elaborate all'interno del
  gestionale

- **Crediti:** contiene tutte le Note d'Accredito (NC) relative a
  richieste di reso merce approvate e/o elaborate all'interno del
  gestionale.

- **Matrici:** contiene tutti i documenti di tipo Matrice (MA, MX)
  creati all'interno del gestionale ed esportati all'interno del sito.

> **ATTENZIONE!** Per poter visualizzare questa sezione è necessario
> aver abilitato la gestione delle matrici impostando per questo il
> parametro "**Abilita Gestione Matrici**" presente all'interno della
> sezione "Configurazione Matrici" del Wizard sul valore Si. Per
> maggiori informazioni in merito si veda anche la sezione "*Ordini --
> Gestione Matrici*" di questo manuale

- **Prenotazioni:** disponibile sono nel caso di siti collegati ai
  gestionali Ho.Re.Ca. Beauty o Menu. Contiene tutti i documenti
  relativi alle varie prenotazioni effettuate dallo specifico utente
  all'interno del sito.

A livello di navigazione del componente è possibile passare da una
sezione all'altra utilizzando anche il tasto "TAB" della tastiera. Il
tasto "Invio" consente invece di aprire e visualizzare il contenuto
corrispondente alla linguetta attualmente selezionata.

Per ogni documento sono riportate le seguenti informazioni

- **Numero:** numero identificativo del documento in esame.

- **Sigla:** sigla e numero assegnati all'interno del gestionale al
  documento in esame. Nel caso in cui l'ordine non sia ancora stato
  inserito sul gestionale questa informazione, ovviamente, non sarà
  presente.

- **Data:** data in cui è stato effettuato l'ordine

**ATTENZIONE!** per poter garantire un corretto e normale funzionamento
del sito è necessario verificare di aver inserito il componente in esame
all'interno della pagina "**Ordini**". In caso contrario infatti
determinati automatismi potrebbero non funzionare in maniera corretta
pregiudicando agli utenti la possibilità di controllare lo stato dei
propri documenti.

