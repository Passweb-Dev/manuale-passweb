# CATEGORIE



Il tab "**Categorie**" visibile solo dopo aver configurato e salvato i
parametri presenti all'interno del tab "Configurazione", consente di
configurare e gestire la generazione del feed utilizzato per condividere
con Clerk informazioni relative alle Categorie Merceologiche gestite
all'interno del proprio sito Ecommerce.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\clerk_feed_categorie.bmp](./assets/media/image17.png)

In questo senso dunque il parametro:

**Genera Feed alla Sincronizzazione**: consente, se selezionato, di
generare automaticamente il feed ad ogni sincronizzazione sito --
gestionale (Standard o Totale).

**URL Feed**: consente di visualizzare l'url di pubblicazione del feed,
quello che dovrà poi essere inserito all'interno del campo "JSON
Categories URL" alla pagina "**Data -- Configuration**" dello store
Clerk con cui si desidera effettuare l'integrazione (per maggiori
informazioni in merito si veda anche quanto indicato all'interno del
precedente capitolo "*Sincronizzazione Dati*")

Il pulsante "**Genera Feed**" presente nella parte bassa della maschera
consente invece di avviare manualmente la generazione del relativo feed.

Per ciascuna categoria presente all'interno del feed verranno gestite le
seguenti informazioni:

- id Categoria Passweb

- nome Categoria

- descrizione Categoria

- url della pagina di Categoria

- sotto categorie (array contenente i codici delle sotto categorie
  merceologiche)

- url immagine della Categoria

**ATTENZIONE!** **il feed delle categorie conterrà sempre e comunque
tutte le categorie merceologiche attualmente gestite all'interno del
sito**

Nel caso dei siti multilingua i campi presenti all'interno del feed (es.
"nome categoria") verranno valorizzati nella lingua impostata in fase di
configurazione del relativo account Clerk

