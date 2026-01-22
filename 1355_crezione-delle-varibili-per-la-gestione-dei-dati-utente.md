# CREZIONE DELLE VARIBILI PER LA GESTIONE DEI DATI UTENTE



Come già indicato nel precedente capitolo di questo manuale
l'inserimento nel dataLayer della sezione user_data con i dati di prima
parte degli utenti che hanno prestato tutti i consensi del caso, di per
sé non comporta assolutamente il trasferimento di queste informazioni a
Google Analytics o a Google Ads.

Come per i dati ecommerce infatti, anche in questo caso dovremo prima di
tutto creare in GTM le variabili di livello dati necessarie per
prelevare dal dataLayer di Passweb i relativi dati utente in maniera
tale da averi a disposizione anche all'interno di Tag Manager.

Fatto questo dovremo poi creare anche un'ulteriore variabile, questa
volta di tipo "User-Provided Data", che di fatto sarà quella che
conterrà tutti i dati utente prelevati dal dataLayer e quella che
dovremo effettivamente utilizzare in fase di configurazione dei vari Tag
di tracciamento verso Google Analytics e/o Google Ads per fare in modo
di inviare a queste piattaforme, oltre ai dati ecommerce con i relativi
parametri, anche i dati utente necessari per la gestione delle
conversioni avanzate.

Vediamo quindi nel dettaglio quali variabili dovremo creare e come fare
per crearle.

