# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_iu_barra_utente_configurazione_res.bmp](./assets/media/image17.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

**Nome** (obbligatorio), consente di inserire un nome per il Componente
Paragrafo che si sta realizzando

**Pubblico (selezionato a default):** consente di impostare la
visibilità del componente lato sito web.

**Periodo di Pubblicazione:** consente di associare al Componente in
oggetto uno specifico periodo di pubblicazione, definendone l'effettiva
data di pubblicazione e la corrispondente data di oscuramento.

**ATTENZIONE!** Per maggiori informazioni relativamente ai parametri
**Nome, Pubblico, Periodo di Pubblicazione** si veda anche quanto
indicato all'interno del capitolo "*Configurazione Componenti --
Caratteristiche generali* -- *Dati Componente* " di questo manuale

**Caricamento Javascript**: se selezionato, consente di caricare il
relativo componente in maniera asincrona al termine del caricamento
della pagina web.

**ATTENZIONE!** Per maggiori informazioni relativamente ai parametri
**Caricamento Javascript** e **Statico** si veda anche quanto indicato
all'interno del capitolo "*Configurazione Componenti -- Caratteristiche
generali* -- *Staticizzazione e caricamento asincrono*" di questo
manuale

**Disabilita Cache:** consente di disabilitare la possibilità di
inserire in cache il componente in esame.

Per maggiori informazioni relativamente alla gestione della cache in
Passweb si veda anche il relativo capitolo di questo manuale
("*Configurazione -- Cache*")

**Testo**: consente di inserire, in tutte le lingue attualmente gestite
all'interno del sito, il testo che dovrà essere visualizzato all'interno
del componente.

Il pulsante "**Aggiungi Segnaposto**" consente di inserire appositi
placeholder che verranno poi sostituiti a runtime con informazioni
relative all'utente attualmente loggato

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\segnaposto_barra_utente.bmp](./assets/media/image18.png)

Nello specifico è possibile utilizzare i seguenti segnaposto:

- **Nome e Cognome/Ragione Sociale**: in questo caso all'interno del
  Componente verrà visualizzato il Nome e Cognome o in alternativa la
  ragione sociale dell'utente attualmente loggato sul sito

- **Indirizzo E-mail**: in questo caso all'interno del Componente verrà
  visualizzato l'indirizzo mail dell'utente attualmente loggato sul sito

- **Username**: in questo caso all'interno del Componente verrà
  visualizzato lo Username dell'utente attualmente loggato sul sito

- **Codice Conto gestionale**: in questo caso all'interno del Componente
  verrà visualizzato il codice conto associato, sul gestionale,
  all'utente attualmente loggato sul sito.

**ATTENZIONE!** Nel caso in cui l'utente attualmente loggato sia un
utente di tipo **Contatto** (e quindi non ancora inserito all'interno
del gestionale) verrà visualizzato il codice ad esso associato in
Passweb (diverso da quello che gli sarà poi associato nel momento in cui
verrà inserito sul gestionale)

**Visualizza Logout:** se selezionato consentirà di visualizzare
all'interno del Componente il pulsante di Logout necessario per
effettuare la disconnessione dal sito.

**Pagina di destinazione al Logout:** consente di specificare la pagina
del sito cui l'utente verrà automaticamente ridiretto una volta
effettuato il Logout dal sito. Il pulsante "**Deseleziona**"
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_deseleziona_res.bmp](./assets/media/image4.png) ), presente nella contestuale barra degli
strumenti, consente di eliminare l'associazione ad una specifica pagina
cui effettuare il redirect automatico.

> **NOTA BENE:** nel caso in cui non venga indicata una specifica
> "Pagina di destinazione al Logout", una volta effettuata il logout
> l'utente rimarrà esattamente nella pagina di partenza.

**Pagina Logout Cliente Agente:** consente di indicare, selezionandola
dall'apposito menu a tendina, la specifica sezione dell'Area Riservata
cui dovrà essere automaticamente ricondotto un Agente nel momento in cui
dovesse effettuare il logout per il cliente attualmente impersonificato.

**Posizionamento dei Campi:** consente di posizionare gli elementi
principali del componente secondo uno schema prestabilito.

Nello specifico, gli elementi soggetti al tipo di posizionamento
impostato mediante questo parametro saranno:

- La label

- Il pulsante di logout

E' possibile selezionare uno dei seguenti valori:

- Affiancati a destra

- Affiancati a sinistra

- Affiancati e giustificati

- Affiancati e opposti

- Centrati e affiancati

- Centrati e Incolonnati

- Incolonnati a destra

- Incolonnati a sinistra

- Custom

**ATTENZIONE!** Nel caso in cui si decidesse di utilizzare uno dei
preset presenti in elenco poi il posizionamento degli elementi sarà
esattamente quello indicato e non potrà essere modificato in alcun modo.

**L'opzione Custom consente invece di non applicare nessun preset
particolare.** **In queste condizioni dunque il posizionamento dei vari
elementi potrà essere variato liberamente agendo sulle corrette
proprietà CSS mediante lo style editor di Passweb e/o mediante i
relativi strumenti di editing avanzato.**

**Ordinamento di visualizzazione dei campi:** visualizzato solo nel caso
in cui il precedente parametro non sia stato impostato sul valore
Custom.

Consente di definire l'ordine di visualizzazione degli elementi
principali del componente in esame, permettendo dunque, già in fase di
configurazione del componente stesso di decidere quale elemento dovrà
essere visualizzato prima e quale dopo.

**ATTENZIONE**! Anche in questo caso l'opzione Custom, non attiva nessun
tipo di preset per cui l'ordine di visualizzazione dei rispettivi
elementi potrà essere variato liberamente agendo sulle corrette
proprietà CSS mediante lo style editor di Passweb e/o mediante i
relativi strumenti di editing avanzato.

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

