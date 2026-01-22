# GRUPPI UTENTI SITO



La sezione **"Gruppi Utenti Sito"**, accessibile dalla voce di menu
principale "**Utenti**", consente di visualizzare e gestire i gruppi e
le gerarchie in cui possono essere suddivisi gli utenti del sito

**NOTA BENE:** con il termine "Gerarchia Utenti" si intende un insieme
di gruppi organizzati secondo una struttura gerarchica ad albero

All'interno di questa sezione dell'applicazione comparirà quindi la
maschera **"Gruppi Utenti"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gruppi_utenti_passcom.bmp](./assets/media/image254.png){width="5.604166666666667in"
height="3.5in"}

in cui verranno visualizzati:

- **in azzurro** i gruppi utente che rappresentano il gruppo radice di
  una certa gerarchia.

> Tali gruppi avranno quindi anche dei gruppi figli visualizzabili e
> gestibili cliccando sul pulsante **"Modifica"** presente nella
> contestuale barra degli strumenti

- **in bianco** i gruppi utente che non appartengono a nessuna gerarchia
  e che non hanno quindi nessun gruppo figlio.

- **in verde** i gruppi **Standard** ("Utente Autenticato" e "Utenti Non
  Autenticati").

> **Utente Autenticato:** apparterranno a questo gruppo tutti gli utenti
> che hanno effettuato il login al sito. Nel momento in cui, dunque, un
> qualsiasi utente effettui l'accesso al sito verrà automaticamente
> inserito all'interno di questo gruppo.
>
> **Utenti Non Autenticati:** apparterranno a questo gruppo tutti gli
> utenti che visitano il sito senza effettuare l'autenticazione.
>
> **NOTA BENE:** i gruppi Standard sopra indicati sono creati in
> automatico dall'applicazione e la loro gestione è demandata
> interamente a Passweb. Tali gruppi non potranno quindi essere
> eliminati, non sarà possibile creare su di essi nessun tipo di
> gerarchia, così come non sarà possibile associare loro degli utenti in
> maniera manuale né tantomeno gestirne i parametri di "Comunicazione
> Interna" o di "Gestione SMS".

Sulla base di quanto detto appare evidente che all'interno della
maschera "Gruppi Utenti" verranno, in ogni caso, visualizzati i soli
gruppi di utenti che non hanno un gruppo padre.

I pulsanti presenti nella contestuale barra degli strumenti
consentiranno rispettivamente di:

**Lista Utenti Gruppo**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_lista_utenti_gruppo.bmp](./assets/media/image110.png){width="0.7076388888888889in"
height="0.175in"}): consente di visualizzare l'elenco degli utenti
appartenenti al gruppo attualmente selezionato.

Cliccando su questo pulsante verrà infatti visualizzata la maschera
"**Lista Utenti -- Nome Gruppo**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\passcom_lista_utenti_nome_gruppo.bmp](./assets/media/image255.png){width="5.825in"
height="3.545138888888889in"}

contenente l'elenco degli utenti appartenenti al gruppo in esame. I
pulsanti presenti nella barra degli strumenti consentono di:

- **Esportazione Utenti**
  (![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_esporta_utenti.bmp](./assets/media/image112.png){width="0.6951388888888889in"
  height="0.175in"} ): consente di esportare **in formato .csv**
  l'elenco degli utenti del gruppo

> Per maggiori informazioni relativamente alla procedura di esportazione
> utenti si veda anche la sezione *"Utenti -- Utenti Sito -- Utenti"* di
> questo manuale

- **Aggiungi al Gruppo** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_aggiungi_al_gruppo.bmp](./assets/media/image113.png){width="0.7208333333333333in"
  height="0.2076388888888889in"} ): consente di associare al gruppo in
  esame, un qualsiasi utente del sito. Cliccando su questo pulsante
  verrà quindi visualizzata la maschera, **a selezione multipla**, dei
  possibili utenti da aggiungere al gruppo

> **NOTA BENE:** dall'elenco dei possibili utenti da aggiungere al
> gruppo verranno ovviamente esclusi quelli che dello specifico gruppo
> fanno già parte.
>
> Per associare uno più utenti al gruppo in esame sarà quindi
> sufficiente selezionarli all'interno della tabella sopra evidenziata
> (filtrabile attraverso l'apposito pannello di ricerca), e cliccare poi
> sul pulsante "**Aggiungi**" visualizzato nella contestuale barra degli

- **Modifica Utente**
  (![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_modifica_utente.bmp](./assets/media/image10.png){width="0.5847222222222223in"
  height="0.18819444444444444in"}): consente di accedere ai dati
  anagrafici dell'utente attualmente selezionato in elenco. Cliccando su
  questo pulsante verrà infatti aperta la maschera **"Dati Utente"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\passcom_dati_utente2.bmp](./assets/media/image256.png){width="5.895833333333333in"
height="3.4805555555555556in"}

> attraverso cui poter gestire, eventualmente, anche l'associazione
> "Utente -- Gruppo".

- **Rimuovi dal gruppo** ( ): consente di eliminare l'associazione tra
  il gruppo in esame e l'utente attualmente selezionato in elenco.

> **ATTENZIONE!** La rimozione di un utente da uno specifico gruppo,
> **non elimina l'utente dal sito**. L'utente rimosso continuerà quindi
> ad essere presente tra gli "Utenti Sito".

- **Elimina Utente:**
  (![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_elimina_utente.bmp](./assets/media/image68.png){width="0.5652777777777778in"
  height="0.2013888888888889in"} ) consente di eliminare l'utente
  attualmente selezionato dal database di Passweb

> **ATTENZIONE!: per Utenti di tipo Passcom la corretta procedura di
> eliminazione è quella che prevede di agire direttamente all'interno
> del gestionale, ad esempio, mediante l'apposito parametro presente in
> "*Dati Aziendali (F4 da "Anagrafica Azienda") -- Configurazione Moduli
> -- Collegamento sito commercialista*"**
>
> ![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\gestione_sito_19.comm.bmp](./assets/media/image235.png){width="2.571527777777778in"
> height="0.9743055555555555in"}
>
> Nel caso in cui si dovesse comunque decidere di procedere
> all'eliminazione di un utente Passcom tramite questo pulsante, sarà
> poi necessario intervenire anche lato gestionale; in caso contrario lo
> specifico utente potrebbe comunque essere riesportato a seguito di una
> futura sincronizzazione.
>
> Eliminando un utente dal sito, indipendentemente dal fatto che questo
> sia un Utente Passcom o un Utente NON Passcom, verranno
> automaticamente eliminate anche tutte le cartelle "Standard" presenti
> in Area Riservata (sezione Documenti) create da quello stesso utente,
> **che non risultano essere legate ad altri gruppi e che non hanno file
> al loro interno**.
>
> **NOTA BENE:** eliminando un utente, sia esso Passcom o NON Passcom,
> verranno automaticamente eliminati anche i messaggi e le attività in
> agenda ad esso collegate.
>
> Per maggiori informazioni relativamente alle diverse sezioni e
> funzionalità dell'Area Riservata si veda anche la sezione *"Business
> to Business Area Riservata"* di questo manuale.

- **Crea Nuovo** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_crea_nuovo.bmp](./assets/media/image257.png){width="0.3638888888888889in"
  height="0.15555555555555556in"} ): consente di creare un nuovo utente
  **NON Passcom.** Per maggiori informazioni relativamente alla
  procedura di creazione di un nuovo utente NON Passcom si veda anche la
  sezione *"Utenti -- Utenti Sito -- Utenti"* di questo manuale

**Modifica** (
![Videate\\pulsante_modifica.bmp](./assets/media/image258.png){width="0.31805555555555554in"
height="0.14930555555555555in"} ): consente di gestire le proprietà del
gruppo attualmente selezionato oltre, eventualmente, alla gerarchia cui
esso da origine.

Cliccando su questo pulsante verrà infatti visualizzata la maschera
**"Gerarchia Utenti -- Nome gruppo radice"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gruppi_utentiNOBP1_passcom.bmp](./assets/media/image259.png){width="5.610416666666667in"
height="3.629861111111111in"}

all'interno della quale sarà possibile gestire, attraverso l'apposito
albero presente nella parte sinistra l'eventuale gerarchia.

Nella parte destra della maschera verranno invece visualizzate, e
potranno quindi essere gestite, le proprietà del gruppo attualmente
selezionato all'interno dell'albero.

**Elimina** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_elimina.bmp](./assets/media/image95.png){width="0.325in"
height="0.14305555555555555in"} ): consente di eliminare il gruppo
attualmente selezionato.

**NOTA BENE:** nel caso in cui al gruppo sia associata anche una
gerarchia, eliminando il gruppo verrà eliminata anche l'intera struttura
di sottogruppi.

**Nuovo Gruppo Utenti** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_nuovo_gruppo_utenti.bmp](./assets/media/image119.png){width="0.6493055555555556in"
height="0.14930555555555555in"} ): consente di creare un nuovo gruppo ed
eventualmente associargli anche una gerarchia di sotto gruppi.

Cliccando su questo pulsante si verrà infatti ricondotti alla maschera
**"Creazione Gruppo"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\passcom_creazione_gruppo.bmp](./assets/media/image260.png){width="5.610416666666667in"
height="3.629861111111111in"}

attraverso cui poter definire tutte le proprietà del gruppo stesso.

In particolare per ogni nuovo gruppo sarà possibile indicare un valore
per i seguenti parametri:

- **Nome (obbligatorio):** consente di specificare il nome del gruppo
  che si sta creando

- **Gestione SMS:** se attivato, consente di abilitare, in Area
  Riservata, gli utenti del gruppo all'invio di SMS per notificare ai
  rispettivi destinatari l'inserimento di un nuovo messaggio, di una
  nuova attività in agenda, ecc...

> **ATTENZIONE!** per poter attivare effettivamente l'invio delle
> notifiche SMS è necessario aver impostato correttamente i parametri di
> configurazione presenti all'interno della sezione "**Configurazione
> SMS**" alla pagina "Account e-mail e SMS" del Wizard (menu "*Posta/SMS
> -- Impostazioni -- Configurazione*")
>
> Per maggiori informazioni in merito all'attivazione dell'account SMS
> si rimanda a quanto indicato nel relativo capitolo di questo manuale
> ("*Parametri Posta /SMS -- Configurazione*")

- **Gestione Telegram --** visualizzato solo nel caso in cui sia stato
  acquistato e correttamente configurato il modulo per l'integrazione
  Passweb -- Telegram

> Se attivato, consente di abilitare, in Area Riservata, gli utenti del
> gruppo all'invio delle notifiche Telegram relativamente
> all'inserimento di un nuovo messaggio, di una nuova attività in
> agenda, ecc...
>
> Per maggiori informazioni in merito all'integrazione Passweb --
> Telegram si rimanda a quanto indicato nel relativo capitolo di questo
> manuale ("*Passweb e Telegram*")

- **Gestione Whatsapp --** visualizzato solo nel caso in cui sia stato
  acquistato e correttamente configurato il modulo per l'integrazione
  Passweb -- WA Smart Business

> Se attivato, consente di abilitare, in Area Riservata, gli utenti del
> gruppo all'invio delle notifiche Whatsapp (tramite piattaforma WA
> Smart Business) relativamente all'inserimento di un nuovo messaggio,
> di una nuova attività in agenda, ecc...
>
> Per maggiori informazioni in merito all'integrazione Passweb -- WA
> Smart Business si rimanda a quanto indicato nel relativo capitolo di
> questo manuale ("*Passweb e WA Smart Business*")

- **Comunicazione interna**: flaggando questo parametro, verrà abilitata
  in Area Riservata la comunicazione tra gli utenti di pari livello. In
  queste condizioni quindi tutti gli utenti appartenenti al gruppo in
  esame potranno comunicare tra loro

- **Comunicazione Livello Superiore**: flaggando questo parametro, verrà
  abilitata in Area Riservata la possibilità di comunicare con i singoli
  utenti dei gruppi padre (collocati quindi ad un livello gerarchico più
  alto) del gruppo in esame. Nel caso in cui tale parametro non venga
  selezionato, la comunicazione verso l'alto potrà essere effettuata a
  livello di intero gruppo ma non a livello di singoli utenti.

Dopo aver creato il nuovo gruppo questo comparirà nella parte sinistra
della maschera e sarà quindi possibile, a questo punto, associargli
anche dei sottogruppi.

Per maggiori informazioni in merito alla creazione di una gerarchia di
gruppi si veda il successivo capitolo "*Creazione e gestione di una
Gerarchia Personalizzata*" di questo manuale.

**Importa** (
![Videate\\pulsante_importa.bmp](./assets/media/image220.png){width="0.3506944444444444in"
height="0.175in"} ): consente variare in maniera massiva, mediante
l'upload di un apposito file csv i dati di configurazione dei Gruppi
Utente **NON STANDARD**

**ATTENZIONE! la procedura in oggetto non consente di variare in alcun
modo i Gruppi Utente Standard gestiti da Passweb** (per maggiori
informazioni relativamente a questa tipologia di Gruppi Utente si vedano
anche i successivi capitoli di questo manuale)

Cliccando sul pulsante in esame verrà visualizzata la maschera
"**Importazione Dati Gruppi**" mediante la quale poter effettuare
l'upload del file contenente le informazioni desiderate.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\import_file_dati_gruppi_commercialista.bmp](./assets/media/image261.png){width="5.5in"
height="3.441666666666667in"}

Nello specifico all'interno di questa sezione sarà necessario indicare:

- **File (csv-txt):** consente di selezionare il file txt o csv da
  uplodare e contenente i dati dei gruppi utente da modificare

- **Lingua**: consente di indicare la lingua del sito a cui dovranno
  fare riferimento i dati presenti all'interno del file di importazione

- **Separatore**: consente di indicare, selezionandolo, dall'apposito
  menu a tendina, il carattere che è stato utilizzato all'interno del
  file di importazione come separatore per i vari campi

Affinchè la procedura di import possa funzionare in maniera corretta e i
dati contenuti nel file possano essere associati ai relativi gruppi
utente, dovranno essere rispettate delle regole ben precise. Nello
specifico:

- Prima di avviare la procedura di import dovranno già essere stati
  creati all'interno di Passweb, tutti i gruppi utente i cui parametri
  di configurazione dovranno essere valorizzati attraverso questa
  procedura.

> **ATTENZIONE! La procedura di import non crea in alcun modo nuovi
> Gruppi Utente**

- Il file da importare deve avere estensione .csv o .txt

- Il carattere separatore dei vari campi deve essere esattamente quello
  indicato all'interno del campo "**Separatore**" presente nel form di
  importazione.

- L'intestazione, ossia la prima riga del file, deve necessariamente
  contenere l'elenco dei nomi dei campi articolo che dovranno poi essere
  valorizzati con i dati presenti all'interno del file stesso.

<!-- -->

- Il primo campo del file, **obbligatorio e utilizzato come chiave**,
  dovrà essere **l'identificativo Passweb** **del relativo gruppo
  utente**, dato questo reperibile in corrispondenza del relativo campo
  presente nel file che potrà essere generato dalla procedura di
  esportazione dei Gruppi Utente

> ***NOTA BENE:** se all'interno del file da importare non è presente
> l'identificativo del gruppo utente passweb e/o se tale valore non
> corrisponde a quello di un gruppo non standard effettivamente gestito
> all'interno del proprio sito la procedura di import non valorizzerà,
> ovviamente, alcun campo*

- **Il file di importazione deve soddisfare le specifiche del formato
  RFC4180**

<!-- -->

- È necessario creare file distinti per le diverse lingue gestite
  all'interno del sito. In fase di importazione sarà poi possibile, come
  visto, indicare la specifica lingua cui il file fa riferimento

Di seguito viene indicato l'elenco dei campi che potranno essere
inseriti all'interno del file csv e che potranno quindi essere
valorizzati in maniera massiva mediante la procedura in esame:

- **id**: identificativo del gruppo utente reperibile in corrispondenza
  del relativo campo presente nel file che potrà essere generato dalla
  procedura di esportazione dei Gruppi Utente

> **ATTENZIONE! il campo id è obbligatorio e verrà utilizzato come campo
> chiave**

- **nome**: corrispondente al campo **Nome** presente nella sezione
  "**Generale**" della maschera di configurazione del gruppo

> Consente di impostare il nome del relativo Gruppo Utente
>
> Il campo è un booleano e ammette i seguenti valori:

- **SI 🡪** L'utente può effettuare il login al sito

- **NO 🡪** L'utente non può effettuare il login al sito

<!-- -->

- **sms**: corrispondente al campo "**Gestione Sms**" presente nella
  sezione "**Area Riservata**" della maschera di configurazione del
  gruppo

> Consente di indicare se gli utenti del relativo gruppo potranno o meno
> gestire gli sms
>
> Il campo è un booleano e ammette i seguenti valori:

- **SI 🡪** Gli utenti del gruppo potranno gestire gli sms

- **NO 🡪** Gli utenti del gruppo non potranno gestire gli sms

<!-- -->

- **whatsapp**: corrispondente al campo "**Gestione Whatsapp**" presente
  nella sezione "**Area Riservata**" della maschera di configurazione
  del gruppo

> Consente di indicare se gli utenti del relativo gruppo potranno o meno
> gestire le notifiche collegate ai diversi eventi gestiti via Whatsapp
>
> Il campo è un booleano e ammette i seguenti valori:

- **SI 🡪** Gli utenti del gruppo potranno gestire le notifiche Whatsapp

- **NO 🡪** Gli utenti del gruppo non potranno gestire le notifiche
  Whatsapp

> **ATTENZIONE!** il campo in esame dovrà essere gestito solo nel caso
> in cui sia stato attivato il modulo relativo all'integrazione Passweb
> -- WA Smart Business. Per maggiori informazioni si rimanda a quanto
> indicato nel relativo capitolo ("*Passweb e WA Smart Business*") di
> questo manuale

- **telegram**: corrispondente al campo "**Gestione Telegram**" presente
  nella sezione "**Area Riservata**" della maschera di configurazione
  del gruppo

> Consente di indicare se gli utenti del relativo gruppo potranno o meno
> gestire le notifiche collegate ai diversi eventi gestiti via Telegram
>
> Il campo è un booleano e ammette i seguenti valori:

- **SI 🡪** Gli utenti del gruppo potranno gestire le notifiche Telegram

- **NO 🡪** Gli utenti del gruppo non potranno gestire le notifiche
  Telegram

> **ATTENZIONE!** il campo in esame dovrà essere gestito solo nel caso
> in cui sia stato attivato il modulo relativo all'integrazione Passweb
> -- Telegram. Per maggiori informazioni si rimanda a quanto indicato
> nel relativo capitolo ("*Passweb e Telegram*") di questo manuale

- **comunicazioneInterna**: corrispondente al campo "**Comunicazione
  Intera**" presente nella sezione "**Area Riservata**" della maschera
  di configurazione del gruppo

> Consente di indicare se gli utenti del relativo gruppo potranno o meno
> comunicare tra di loro
>
> Il campo è un booleano e ammette i seguenti valori:

- **SI 🡪** Gli utenti del gruppo potranno comunicare tra di loro

- **NO 🡪** Gli utenti del gruppo non potranno comunicare tra di loro

<!-- -->

- **comunicazioneUp**: corrispondente al campo "**Comunicazione Utenti
  Livello superiore**" presente nella sezione "**Area Riservata**" della
  maschera di configurazione del gruppo

> Consente di indicare se gli utenti del relativo gruppo potranno o meno
> comunicare con gli utenti dei gruppi padri
>
> Il campo è un booleano e ammette i seguenti valori:

- **SI 🡪** Gli utenti del gruppo potranno comunicare con gli utenti dei
  gruppi padri

- **NO 🡪** Gli utenti del gruppo non potranno comunicare con gli utenti
  dei gruppi padri

**Esporta** (
![Videate\\pulsante_esporta.bmp](./assets/media/image218.png){width="0.33125in"
height="0.175in"} ): consente di esportare, all'interno di un apposito
file csv, i dati dei gruppi utente, NON STANDARD, attualmente gestiti
all'interno del sito.

**ATTENZIONE!** I campi presenti nel file csv sono gli stessi indicati
per la procedura di importazione dati

