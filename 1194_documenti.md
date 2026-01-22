# DOCUMENTI



La sezione "**Documenti**" ha un aspetto e funzionalità leggermente
diverse a seconda dell'utente loggato.

In particolare, nel momento in cui ad effettuare l'autenticazione
dovesse essere:

- un utente codificato direttamente dal backend del proprio sito
  Passweb, all'interno di questa sezione sarà possibile scambiare
  solamente documenti generici con utenti appartenenti alla propria
  gerarchia

- un utente Passcom, oltre a poter scambiare generici documenti, come
  nel caso precedente, con utenti appartenenti alla propria gerarchia,
  ci sarà anche la possibilità di prelevare e visualizzare documenti
  memorizzati direttamente all'interno del gestionale.

In quest'ultimo caso poi, utenti Passcom di tipo:

- **Commercialista** avranno la possibilità di prelevare e visualizzare
  i documenti memorizzati all'interno del gestionale per tutte le
  aziende esportate e gestite all'interno del sito

- **Dipendente** avranno la possibilità di prelevare e visualizzare i
  documenti memorizzati all'interno del gestionale per le sole aziende
  che sono abilitati a gestire

- **Azienda** avranno la possibilità di prelevare dal gestionale e
  visualizzare solamente i propri documenti

**ATTENZIONE!** Per poter accedere a questa sezione dell'area riservata
è necessario aver abilitato la relativa App operando per questo
all'interno dell'apposita sezione del Wizard accessibile dal menu "*Sito
-- Preferenze*"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_comm_documenti_attivazione.bmp](./assets/media/image55.png)

La pagina è suddivisa in tre distinte sezioni:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_comm_documenti_struttura.bmp](./assets/media/image56.png)

- Nella parte alta è presente campo di ricerca ad autocompletamento
  utile per indicare l'azienda per cui si vogliono visualizzare o
  ricercare dei documenti.

> Ovviamente le aziende visualizzabili all'interno di questo pannello di
> ricerca dipenderanno dalla tipologia di utente loggato
> (Commercialista, Dipendente, Azienda) e dallo specifico gruppo di
> utenti cui esso appartiene.
>
> Un utente Passcom di tipo Commercialista potrà, ad esempio, ricercare
> una qualsiasi delle aziende esportate e gestite all'interno del sito;
> un utente Passcom di tipo Dipendente potrà invece ricercare e
> visualizzare all'interno di questo pannello le sole aziende che è
> effettivamente in grado di gestire (secondo i permessi che gli sono
> stati associati all'interno del gestionale).
>
> Per un utente Passcom di tipo azienda, infine, il campo in esame sarà
> ovviamente bloccato sul nome dell'azienda stessa
>
> **ATTENZIONE!** prima di poter effettivamente visualizzare o ricercare
> delle cartelle e / o dei documenti è indispensabile aver selezionato,
> innanzitutto, una delle aziende gestite

- Nella sezione di sinistra, una volta selezionata un'azienda, viene
  visualizzato invece l'albero delle cartelle in cui sono organizzati i
  documenti di questa stessa azienda.

- Nella sezione di destra, infine, verranno visualizzati i documenti
  presenti all'interno della cartella attualmente selezionata
  all'interno dell'albero o quelli risultanti da una ricerca effettuata
  mediante il pannello di "**Ricerca Documenti**" presente nella parte
  alta di questa stessa sezione.

Nei dispositivi mobile a default, verrà visualizzato, il pannello di
ricerca per la selezione dell'azienda per cui si intende ricercare e
visualizzare dei documenti e, immediatamente al di sotto di questo
pannello, l'albero delle cartelle in cui sono organizzati i documenti di
quella stessa azienda.

In queste condizioni per visualizzare i file presenti all'interno di una
specifica cartella, così come per poter accedere al pannello di "Ricerca
Documenti" sarà necessario selezionare la cartella desiderata
all'interno dell'albero o, in alternativa la radice "Documenti" e
cliccare poi sul pulsante "**Elenco Documenti**" (
![Videate\\pulsante_elenco_documenti_mobile.bmp](./assets/media/image57.png) )

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_comm_documenti_mobile.bmp](./assets/media/image58.png)

In questo modo infatti verrà visualizzata la griglia dei documenti
attualmente presenti all'interno della cartella selezionata con il
relativo pannello di "Ricerca Documenti"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\documenti_comm_azioni_file_mobile_0.bmp](./assets/media/image59.png)

Una volta selezionato uno dei documenti presenti in elenco il pulsante
raffigurante tre piccoli puntini consentirà di accedere al menu delle
azioni effettuabili sul file selezionato

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\documenti_comm_azioni_file_mobile.bmp](./assets/media/image60.png)

