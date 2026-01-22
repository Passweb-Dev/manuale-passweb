# UTILIZZO DEL SISTEMA DI NOTIFICHE



Una volta eseguite tutte le operazioni indicate nel precedente capitolo
di questo manuale, nel momento in cui un utente del sito tentasse di
acquistare un articolo (la cui gestione della disponibilità è stata
demandata interamente a Passweb) a disponibilità minore o uguale a zero,
ciò non gli sarebbe ovviamente possibile.

In queste condizioni infatti al posto del pulsante per l'aggiunta
dell'articolo in carrello, verrà visualizzato un apposito messaggio
"**Articolo Esaurito**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\articolo_esaurito.bmp](./assets/media/image104.png)

Entrando però nella pagina prodotto, dipendentemente dal fatto di essere
o meno già autenticato e da come sono stati impostati i vari parametri
di configurazione, l'utente avrà ora la possibilità di richiedere di
essere avvisato nel momento in cui questo stesso articolo dovesse
tornare ad essere disponibile.

Per far questo sarà sufficiente inserire l'indirizzo mail cui dovrà
essere inviata la notifica all'interno dell'apposito campo e/o cliccare
sul relativo pulsante di iscrizione al sistema di notifiche

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\notifica_disponibilita_tutti.bmp](./assets/media/image105.png)

L'utente iscritto al sistema di notifiche verrà così memorizzato nel
database del sito e si suoi dati potranno essere visualizzati
all'interno della sezione *"Catalogo -- Gestione Articoli -- Avvisi
Disponibilità"* del Wizard

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\avvisi_disponibilita.bmp](./assets/media/image106.png)

All'interno di questa sezione, l'amministratore del sito, avrà quindi la
possibilità di visualizzare un elenco di tutti i prodotti per cui sono
state effettuate delle richieste di notifica di disponibilità.

Per ciascuno dei prodotti presenti in elenco sarà possibile visualizzare
la sua descrizione (camp **Articolo**) , il suo codice (campo
**Codice**), il numero di utenti che hanno richiesto di essere avvisati
nel momento in cui quello stesso articolo dovesse tornare ad essere
disponibile (campo **Numero**) e le date in cui sono state effettuate
rispettivamente la prima e l'ultima richiesta di notifica (campi **Prima
Iscrizione** e **Ultima Iscrizione**).

Il pannello di ricerca presente nella parte alta della maschera consente
di filtrare gli articoli in elenco per codice e/o descrizione.

Selezionando infine uno degli articoli presenti in elenco, e cliccando
sul pulsante "**Visualizza Notifiche Disponibilità**" (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_visualizza_notifiche_disponibilita.bmp](./assets/media/image107.png) ) sarà possibile visualizzare un elenco
dettagliato di tutti gli utenti che hanno richiesto di essere avvisati
in merito alla disponibilità di quello specifico articolo.

Per ogni utente è possibile visualizzare l'indirizzo mail cui dovrà
essere inviata la notifica (campo **Email**), la data in cui è stata
effettuata la richiesta di notifica (campo **Data Iscrizione**) e la
data in cui tale notifica è stata effettivamente inviata (campo **Data
Notifica**)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\avvisi_disponibilita_iscritti.bmp](./assets/media/image108.png)

A questo punto, posto di aver eseguito correttamente tutte le operazioni
indicate nel precedente capitolo di questo manuale, l'invio delle
notifiche di disponibilità **sarà completamente automatico e
condizionato soltanto alle sincronizzazioni sito -- gestionale**.

Nel momento in cui, infatti, a seguito di una sincronizzazione, uno o
più articoli di quelli per cui è stata effettuata una richiesta di
notifica dovesse tornare ad avere una disponibilità maggiore di zero,
Passweb verificherà la presenza di una Campagna di tipo "Disponibilità
Articolo" con i relativi invii correttamente configurati e, posto che
tutto sia ok, provvederà a trasferire su MailChimp, all'interno
dell'apposita Lista, tutti gli utenti che avevano richiesto di essere
avvisati relativamente alla disponibilità di quegli specifici articoli.

In particolare all'interno della Lista utilizzata per gestire queste
notifiche verrà creato un gruppo di interesse per ciascuno degli
articoli che è tornato a disponibilità maggiore di zero e a tale gruppo
verranno associati tutti gli utenti che hanno richiesto la notifica per
il corrispondente articolo.

Sempre in maniera automatica, verrà quindi avviata la creazione, in
MailChimp, della relativa Campagna e verranno quindi inviate (dai server
di MailChimp) agli utenti corretti le notifiche di "prodotto nuovamente
disponibile".

Contestualmente verrà anche inviata una mail all'amministratore del sito
per informarlo relativamente alle campagne create in MailChimp e,
conseguentemente, all'invio delle relative notifiche di disponibilità

Terminata la campagna gli utenti ai quali è stata consegnata la notifica
verranno eliminati da MailChimp. Continueranno invece ad essere visibili
all'interno della sezione "*Catalogo -- Gestione Articoli -- Avvisi
Disponibilità"* del Wizard di Passweb dove potrà ora essere visualizzata
anche la data in cui gli è stata inviata la notifica di disponibilità.

