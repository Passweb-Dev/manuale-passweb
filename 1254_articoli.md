# ARTICOLI



All'interno di questa sezione è possibile configurare e gestire l'invio
allo Store Mailchimp dei dati relativi agli articoli presenti
all'interno del proprio sito Ecommerce.

![](./assets/media/image125.png)

**ATTENZIONE!** Non è possibile distinguere quali articoli inviare e
quali no per cui, allo stato attuale, tutti gli articoli gestiti
all'interno del sito (compresi eventuali articoli di tipo Spesa)
verranno inviati allo Store Mailchimp

Nello specifico poi è bene sottolineare che:

- **Nel caso di articoli strutturati**, verranno inviati allo Store
  MailChimp solo ed esclusivamente eventuali articoli figli
  correttamente esportati e gestiti all'interno del proprio sito.

> Se l'esigenza dovesse essere, quindi, quella di attivare su MailChimp
> determinate azioni di marketing automation anche in relazione ad
> articoli configurabili sarà necessario assicurarsi, per prima cosa, di
> gestire all'interno del sito non solo il padre di struttura (che come
> detto non verrà mai inviato, per ovvie ragioni, allo Store MailChimp)
> ma anche tutti i possibili articoli figli.

- **Nel caso di articoli a Taglie / Colori (solo Ecommerce Mexal)**,
  verrà inviato allo Store MailChimp l'articolo in se (es. "Scarpe
  Adidas") senza nessuna indicazione relativamente alla specifica Taglia
  / Colore

I parametri di configurazione presenti all'interno di questa sezione
consentono di specificare, selezionandole tra specifici Campi Articolo
e/o tra gli Attributi Passweb attualmente codificati e gestiti, quali
informazioni dovranno essere effettivamente trasmesse a MailChimp per
ogni singolo articolo,.

Nello specifico dunque il campo:

- **Titolo -- campo obbligatorio:** consente di impostare,
  selezionandolo dall'apposito menu a tendina, il campo da cui prelevare
  il Titolo dell'articolo che dovrà poi essere passato allo Store
  MailChimp.

- **Descrizione:** consente di impostare, selezionandolo dall'apposito
  menu a tendina, il campo da cui prelevare la Descrizione dell'articolo
  che dovrà poi essere passata allo Store MailChimp

- **Categoria:** consente di impostare, selezionandolo dall'apposito
  menu a tendina, il campo da cui prelevare la Categoria Merceologia di
  appartenenza degli articoli che verranno poi trasmessi allo Store
  MailChimp

- **Listino -- campo obbligatorio:** consente di indicare,
  selezionandolo dall'apposito menu a tendina, lo specifico listino
  sulla base del quale determinare i prezzi degli articoli che verranno
  poi trasmessi allo Store MailChimp

- **Categoria Sconto cliente:** consente di indicare la specifica
  "Categoria Sconto Cliente" (selezionandola tra quelle definite
  all'interno del gestionale) che dovrà essere presa in considerazione
  nella determinazione del prezzo degli articoli che verranno poi
  trasmessi allo Store MailChimp

Come indicato gli unici campi obbligatori sono quelli relativi al Titolo
dell'articolo e al suo prezzo, campi questi che, di base, dovranno poi
essere inseriti anche in eventuali mail di remarketing gestite
all'interno di MailChimp.

**ATTENZIONE!** L'aggiunta nella trasmissione a MailChimp di
informazioni non obbligatorie sugli articoli (es. Descrizione, Categoria
Merceologica di appartenenza ecc...) potrebbero aumentare i tempi di
sincronizzazione tra Passweb e MailChimp per cui, come consigliato da
MailChimp stesso, tali informazioni andrebbero inserite solo se
strettamente necessarie.

Oltre ai campi appena esaminati, per ogni singolo articolo, verrà
**SEMPRE** trasmessa a MailChimp, se presente, anche la relativa
"**Immagine Prodotto**" (quella visualizzata come immagine iniziale
all'interno della scheda prodotto del relativo articolo), oltre ad una
specifica quantità necessaria a MailChimp per determinare se il relativo
articolo è o meno ancora disponibile.

Tale quantità verrà determinata sulla base della "Disponibilità Passweb"
del relativo articolo, dunque, sulla base delle impostazioni settate per
i parametri presenti all'interno della sezione "Disponibilità" della
maschera "*Configurazione Catalogo*" del Wizard, e sarà aggiornata
ovviamente all'ultima sincronizzazione "Sito -- Gestionale"

Il pulsante "**Sincro Articoli**"
(![](./assets/media/image123.png) ) presente nella barra degli strumenti
di uno Store correttamente connesso, consente di avviare manualmente la
procedura di importazione sul relativo Store MailChimp, dei dati
relativi a tutti gli articoli gestiti all'interno del proprio sito.

**ATTENZIONE!** Una volta lanciata la procedura di importazione articoli
sullo Store Mailchimp l'esito verrà notificato via mail all'indirizzo
indicato all'interno della sezione "Posta/SMS" del Wizard (campo E-mail)

Tale operazione dovrebbe essere effettuata solo la prima volta o,
eventualmente, nel momento in cui si dovesse rendere necessario, per
qualche ragione, allineare la base dati del proprio sito (a livello di
articoli gestiti) con quella presente all'interno dello Store MailChimp.

Una volta effettuata la prima importazione sarà infatti Passweb stesso,
al termine di ogni sincronizzazione Sito -- Gestionale, a preoccuparsi
di trasmettere, in maniera del tutto automatica, allo Store MailChimp
eventuali nuovi articoli importati all'interno del proprio sito
Ecommerce a seguito di quella stessa sincronizzazione e/o ad aggiornare
quelli già presenti all'interno dello Store MailChimp.

Una volta terminata la procedura di importazione, per visualizzare
all'interno di MailChimp gli articoli importati dal proprio sito Passweb
è sufficiente cliccare sulla voce di Menu "**File Manager**" (1)
presente nella barra alta degli strumenti, accedere alla sezione
"**Products**" (2) e selezionare tra tutti i prodotti disponibili quelli
legati allo "**Store Passweb**" (3)

![Videate\\mailchimp-ecommerce_10.bmp](./assets/media/image126.png)

Per maggiori informazioni relativamente alla gestione di questi articoli
lato MailChimp e alle eventuali azioni di marketing automation ad essi
legate si rimanda alla specifica documentazione di prodotto
([www.mailchimp.com](http://www.mailchimp.com))

