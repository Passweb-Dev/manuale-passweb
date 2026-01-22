# CONFIGURAZONE



Indipendentemente dal fatto di utilizzare direttamente le Cartelle
Docuvision o il pannello Ricerca Documenti evidenziato nel precedente
capitolo di questo manuale, per poter attivare all'interno del proprio
sito la possibilità di ricercare in tempo reale documenti memorizzati
sul gestionale è necessario effettuare determinate configurazioni sia
lato gestionale che lato Passweb.

Nello specifico, lato gestionale, sarà necessario:

- attivare il parametro **"Gestione completa"** (menu *"Anagrafica
  Azienda -- Dati Aziendali (F4) --Moduli Aggiuntivi Configurazione
  Azienda -- Docuvision")*

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pagina_pannello_22.comm.bmp](./assets/media/image116.png){width="5.363888888888889in"
height="3.292361111111111in"}

**NOTA BENE:** il parametro **"Gestione Completa"** è unico per tutte le
sotto aziende eventualmente gestite. Ciò significa dunque che variando
il valore del parametro per una sotto azienda la modifica verrà
automaticamente propagata anche a tutte le altre sotto aziende.

- Definire le classi documento Docuvision abilitate per essere gestite
  anche all'interno del sito.

> **ATTENZIONE!** **nella sezione Documenti dell'area riservata verranno
> visualizzate, all'interno della cartella Docuvision, solamente le
> cartelle corrispondenti a classi documento effettivamente abilitate
> per poter essere pubblicate anche all'interno del sito.**
>
> In questo senso dunque per fare in modo che una determinata classe
> documento di Docuvision possa essere pubblicata anche sul sito web,
> con la relativa cartella, è necessario agire dalle maschere "**Classi
> Documento Personalizzate**" e/o "**Classi Documento Predefinite**"
> accessibili dal menu *"Azienda -- Docuvision -- Impostazioni
> Docuvision -- Classi Documento".*

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\docuvision_5_passcom.bmp](./assets/media/image117.png){width="4.052083333333333in"
height="2.6555555555555554in"}

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\docuvision_6_passcom.bmp](./assets/media/image118.png){width="4.123611111111111in"
height="2.720833333333333in"}

> In entrambi i casi, selezionando una delle classi presenti in elenco e
> cliccando sul pulsante "**Pubblicazione Documenti**" (**F7**) verrà
> visualizzata la maschera "**Configurazione pubblicazione documenti
> docuvision**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\docuvision_7_passcom.bmp](./assets/media/image119.png){width="4.1819444444444445in"
height="3.441666666666667in"}

> attraverso la quale poter decidere se la relativa classe documento
> dovrà o meno essere pubblicata anche all'interno del sito
>
> In particolare dunque il campo

- **Pubblica documenti classe (numero della classe)**: consente, se
  selezionato, di pubblicare la classe in esame anche all'interno del
  sito, creando di fatto la relativa sotto cartella all'interno della
  cartella Docuvision dell'azienda in esame

- **Considera documenti**: consente di decidere, selezionando l'opzione
  dal corrispondente menu a tendina, se sul sito per la classe in esame
  dovranno essere pubblicati i documenti dell'ultimo anno gestito,
  dell'ultimo anno gestito e del precedente oppure di tutti gli anni
  gestiti

> **ATTENZIONE!** sul sito verrà poi creata una specifica cartella per
> ogni anno effettivamente gestito e, ovviamente, potranno essere
> ricercati dei documenti solo per quegli stessi anni

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\comm_cartelle_anni.bmp](./assets/media/image120.png){width="5.519444444444445in"
height="3.4805555555555556in"}

- **Dettaglio Tipo Documento** -- attivo solo per alcune delle classi
  Docuvision predefinite.

> Consente di raffinare ulteriormente la ricerca dei documenti, offrendo
> la possibilità di aggiungere, nell'albero di ricerca, un ulteriore
> livello rappresentato appunto dalle diverse tipologie di documenti
> presenti per una stessa classe Docuvision.
>
> Una volta selezionato questo parametro sarà poi necessario andare a
> selezionare anche le singole tipologie di documento che si vogliono
> effettivamente gestire all'interno del sito.
>
> **ATTENZIONE!** anche in questo caso per ogni tipologia di documento
> selezionata verrà poi creata all'interno del sito una corrispondente
> cartella

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\comm_cartelle_tipo_documento.bmp](./assets/media/image121.png){width="5.519444444444445in"
height="3.4805555555555556in"}

**NOTA BENE:** la ricerca per tipologia di documento può essere attivata
unicamente per alcune delle classi Docuvision predefinite. Nel caso
delle classi personalizzate è quindi possibile effettuare ricerche
unicamente per tipologia di classe e per anni di gestione.

Le "**Cartelle Docuvision**", come precedentemente evidenziato, non sono
però l'unica possibilità di accedere ai documenti memorizzati
all'interno del gestionale.

Volendo è infatti possibile utilizzare anche il pannello "**Ricerca
Documenti**". Questo tipo di ricerca utilizza però le Web Api Passcom
per cui, oltre all'attivazione delle Classi Docuvision, secondo quanto
precedentemente indicato, sarà necessario configurare in maniera
corretta anche l'utente Web Api (sia lato gestionale che lato Passweb)
indicando, tra le altre cose, le aziende per cui tale utente potrà
effettivamente utilizzare le Web Api (tipicamente dovranno essere le
stesse aziende effettivamente esportate e gestite anche all'interno del
sito).

**ATTENZIONE!** **nel momento in cui l'utente Web Api non dovesse essere
configurato in maniera corretta, il panello "Ricerca Documenti" avrà al
suo interno il solo campo "Titolo" e consentirà quindi di ricercare
solamente i documenti presenti all'interno di Cartelle Standard e / o di
Cartelle Azienda corrispondenti ad utenti non prelevati dal gestionale**

Nello specifico per poter abilitare il proprio sito commercialista
all'utilizzo delle Web Api, e attivare quindi la corrispondente ricerca
documenti in area riservata, sarà necessario, lato gestionale:

- Verificare di utilizzare una versione Passcom superiore alla 2024D
  (per versioni inferiori alla 2024D l'utilizzo delle Web Api richiede
  necessariamente l'attivazione della suite MDS)

- Creare un utente abilitato all'utilizzo delle API e appartenente
  quindi al gruppo "**Servizi Web API**" (solo utenti di questo gruppo
  potranno infatti utilizzare i relativi servizi)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\passcom_webApi_1.bmp](./assets/media/image122.png){width="4.675in"
height="2.6430555555555557in"}

- Definire le Aziende dell'installazione per cui sarà effettivamente
  possibile utilizzare le Web Api.

> Per fare questo sarà necessario selezionare il Gruppo Utenti
> utilizzato per gestire l'utente Web Api e cliccare poi sul pulsante
> "**Impostazioni**" (F11) in maniera tale da accedere alla maschera
> "**Impostazioni Gruppo ...**" evidenziata in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\passcom_webApi_2.bmp](./assets/media/image123.png){width="5.616666666666666in"
height="3.220833333333333in"}

> Il campo "**Aziende**" consentirà di indicare esattamente le aziende
> per cui sarà possibile utilizzare le Web Api.
>
> **ATTENZIONE!** nel caso in cui il campo "Aziende" dovesse essere
> lasciato vuoto, sarà poi possibile utilizzare le Web Api su tutte le
> aziende dell'installazione
>
> **Il consiglio, ovviamente, è sempre quello di abilitare l'utilizzo
> delle Web Api per tutte le aziende che saranno poi esportate e gestite
> anche all'interno del sito.**
>
> In caso contrario infatti, l'unica possibilità di accedere ai
> documenti Docuvision per aziende per cui non è stato attivato
> l'utilizzo delle Web Api, sarà quella di utilizzare le Cartelle
> Docuvision.
>
> In questo senso poi è bene sottolineare anche che, nel momento in cui
> Passweb andrà a verificare la presenza di eventuali nuovi documenti
> presenti nel gestionale (nelle classi Docuvision opportunamente
> abilitate) per inserire poi i corrispondenti avvisi in bacheca e/o per
> inviare le corrispondenti notifiche mail / sms, potrà prendere in
> considerazione solo le aziende per cui è stato correttamente abilitato
> l'utilizzo delle Web Api.
>
> Per tali aziende verranno quindi inviate eventuali notifiche mentre,
> per il resto, verrà inviata una mail all'amministratore del sito con
> l'indicazione delle aziende per cui le Web Api non state attivate e
> per cui non è quindi stato possibile inviare eventuali notifiche di
> pubblicazione documenti (per maggiori informazioni relativamente alle
> notifiche gestite da Passweb in merito alla pubblicazione di nuovi
> documenti Docuvision si veda anche quanto indicato nei successi
> capitoli di questo manuale).

Lato Passweb sarà invece necessario:

- accedere alla pagina "**Configurazione -- Configurazione Gestionale**"
  del Wizard e impostare i parametri richiesti all'interno della sezione
  Web API, parametri questi che potranno essere diversi a seconda del
  fatto che Passcom sia installato presso la Web Farm Passepartout o in
  locale presso il cliente

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\parametri_conf_Passcom_webAPI_locale.bmp](./assets/media/image124.png){width="5.5777777777777775in"
height="3.5194444444444444in"}

> In ogni caso si tratterà comunque di impostare un valore per i
> seguenti campi:

- **Login API:** username dell'utente Passcom abilitato all'utilizzo
  delle Web Api

- **Password API:** password dell'utente Mexal abilitato all'utilizzo
  delle Web Api

- **Base Address WebApi -- solo per installazioni locali:** indirizzo
  del server Passcom più la porta su cui è in ascolto il servizio Web
  Api

> I valori necessari per costruire il Base Address possono essere
> ricavati all'interno della maschera gestionale "**Configurazione
> webapi**" ("*Servizi -- Configurazioni -- Configurazione moduli -- Web
> Api*")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\passcom_webApi_3.bmp](./assets/media/image125.png){width="3.4868055555555557in"
height="1.7465277777777777in"}

> Supponendo dunque che i valori presenti all'interno dei campi
> evidenziati in figura siano rispettivamente mrossi e 9104 il Base
> Address da inserire nel corrispondente campo Passweb sarà esattamente
> il seguente
>
> *https://mrossi.passepartout.local:9104*
>
> **ATTENZIONE!** per maggiori informazioni relativamente al Base
> Address e, più in generale, all'attivazione e all'utilizzo delle Web
> Api Passcom si consiglia di fare sempre riferimento alla relativa
> documentazione di prodotto

