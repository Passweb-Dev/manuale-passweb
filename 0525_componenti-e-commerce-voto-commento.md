# COMPONENTI E-COMMERCE -- VOTO COMMENTO



Il Componente **"Voto Commento"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_voto_res.bmp](./assets/media/image690.png)

può essere inserito solo ed esclusivamente all'interno di un componente
"**Commenti Associati**" e consente di visualizzare, in corrispondenza
di ogni singolo commento, un controllo del tipo **Si/No** mediante il
quale l' utente potrà esprimere una preferenza sull'utilità dello
specifico commento.

![\\\\192.168.0.84\\d\$\\ManPassweb_Ecommerce\\Videate\\voto_commento_esempio.bmp](./assets/media/image691.png)

**NOTA BENE:** per esprimere una preferenza sull'utilità di un commento,
così come per effettuare un commento o associare un voto ad un prodotto,
è necessario essere autenticati.

Nel caso in cui, dunque si tenti di esprimere una preferenza
sull'utilità dello specifico commento senza prima aver effettuato
l'autenticazione al sito, verrà visualizzato un apposito messaggio di
errore.

Inoltre la valutazione sull'utilità di un commento, proprio perché
effettuabile solo da utenti autenticati rimane legata allo specifico
utente, per cui una volta espresso un giudizio sull'utilità di uno
specifico commento, lo stesso utente potrà solo modificare la sua
preferenza ma non potrà votare una seconda volta lo stesso commento.

A livello di configurazione, una volta inserito il Componente
all'interno della pagina web, verrà aperta in automatico **la sua
maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\voto_commento_configurazione_res.bmp](./assets/media/image692.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

**Nome:** consente di indicare il nome del componente che si sta
realizzando

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

**ATTENZIONE!** Le date indicate all'interno di questi campi verranno
considerate solo ed esclusivamente nel caso in cui il precedente
parametro "Pubblico" sia stato selezionato

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**" e "**Protezione**", presenti nella maschera
di gestione e configurazione di tutti i componenti Passweb, si veda
anche il capitolo " Varianti Responsive -- Configurazione Componenti --
Caratteristiche Generali " di questo manuale.

