# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_iu_rubrica_configurazione_res.bmp](./assets/media/image32.png){width="4.590972222222222in"
height="1.8958333333333333in"}

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

**Nome:** permette di inserire un nome per il campo che si sta editando

**Pubblico (selezionato a default):** consente di impostare la
visibilità del componente lato sito web. Se selezionato il
corrispondente componente verrà correttamente pubblicato e visualizzato
all'interno del sito. Nel caso in cui invece tale parametro non sia
selezionato, il corrispondente componente passerà in modalità "Offline",
sarà quindi visibile all'interno del Wizard, dove potrà essere
normalmente gestito, ma non verrà pubblicato e visualizzato all'interno
del sito.

**Periodo di Pubblicazione:** consente di associare al Componente in
oggetto uno specifico periodo di pubblicazione, definendone l'effettiva
data di pubblicazione e la corrispondente data di oscuramento.

Nel primo dei due campi disponibili occorrerà quindi indicare,
utilizzando l'apposito calendario, la data di inizio pubblicazione. Nel
secondo campo andrà invece specificata la data di fine pubblicazione.

> **ATTENZIONE!** Le date indicate all'interno di questi campi verranno
> considerate solo ed esclusivamente nel caso in cui il precedente
> parametro "Pubblico" sia stato selezionato

**Abilita Validazione località Google**: consente, se selezionato, di
attivare la validazione di quanto inserito all'interno del campo
"**Città**" mediante i servizi offerti da Google Maps.

**ATTENZIONE! per ovvie ragioni, questo tipo di validazione potrà
avvenire in maniera corretta solo nel caso in cui il sito possa
utilizzare effettivamente i servizi della Google Maps**.

Nello specifico, considerando che la funzione di validazione offerta da
Google Maps accetta API Key con restrizione a livello di indirizzo IP
(ma non a livello di Referrer), affinché la validazione del dato
inserito all'interno del campo Città possa avvenire in maniera corretta
è necessario verificare di aver inserito all'interno del campo "**Chiave
Google Maps Distance API**" (pagina "**Preferenze Sito**", tab
"**Integrazioni**" del Wizard) una API key valida e funzionante.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\validazione_citta.bmp](./assets/media/image33.png){width="5.759722222222222in"
height="3.3444444444444446in"}

Per maggiori informazioni in merito all'utilizzo della Google Maps e dei
relativi servizi si consiglia di fare riferimento anche a quanto
indicato all'interno del capitolo "*Sito -- Preferenze -- Integrazioni
-- Google Maps API*" di questo manuale

Supponendo dunque di aver configurato ed impostato tutto in maniera
corretta, andando poi ad inserire sul front end del sito un nuovo
indirizzo di spedizione, alla conferma dei dati verrà effettuata una
chiamata ad un'apposita API di Google cui verrà passato l'indirizzo
(completo di Via, Città, Provincia, CAP e Nazione) inserito dall'utente.
L'API oltre a restituire le coordinate geografiche relative a latitudine
e longitudine, restituirà anche i valori esatti dell'indirizzo
corrispondente.

Nel momento in cui il valore ritornato da Google **relativamente al
campo "Città"** dovesse coincidere esattamente con quello inserito
dall'utente in fase di compilazione del form, la validazione avverrà con
successo, e l'indirizzo verrà effettivamente salvato.

In caso contrario invece, i dati inseriti dall'utente non verranno
salvati, verrà mostrato, in corrispondenza del campo "Città", un
apposito messaggio di errore (modificabile alla sezione "Testi/Messaggi
del Sito" agendo per il componente "Rubrica Utente" sul campo "**Errore
Validazione Google**") e all'interno di questo stesso campo verrà
inserito automaticamente il valore della Città ritornato da Google.

**ATTENZIONE!** L'unico campo ad essere validato ed eventualmente
valorizzato con quanto ritornato da Google è il campo "Città". **Non
verranno quindi corretti in automatico dati quali la Via, il CAP, la
Nazione o la Provincia**

Oltre all'eventuale validazione via Google della città, nel form di
creazione dell'indirizzo di spedizione sono sempre attivi anche i
seguenti controlli:

- **Mail:** all'interno di questo campo dovrà essere inserito
  necessariamente un indirizzo di posta elettronica valido. Un apposito
  controllo verificherà la corretta sintassi dell'indirizzo mail
  inserito che dovrà quindi rispettare il formato
  "*nomecasella@indirizzo.it*".

- **Telefono:** all'interno di questo campo potranno essere inseriti
  soltanto numeri di telefono nel formato E.164 (lo standard
  internazionale per la telefonia). Un apposito controllo verificherà la
  correttezza del numero inserito che dovrà quindi rispettare le
  seguenti regole:

  - il primo carattere deve essere un + seguito dal country code (es.
    +39 per l'Italia) e dal numero di telefono

  - il primo numero dopo il + non può essere uno 0

  - il numero di telefono, comprensivo di country code, non può avere
    meno di 5 cifre né più di 15

  - non sono consentiti caratteri speciali (trattini spazi o punti)

> **ATTENZIONE!** nel caso in cui il browser in uso non dovesse
> supportare l'attributo type="tel" (che attiva i controlli sopra
> indicati) il campo verrà gestito come un semplice campo di testo

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo "Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali" di questo
manuale.

