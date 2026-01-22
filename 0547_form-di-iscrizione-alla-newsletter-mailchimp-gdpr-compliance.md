# FORM DI ISCRIZIONE ALLA NEWSLETTER MAILCHIMP GDPR COMPLIANCE



Nel caso in cui l'esigenza dovesse essere quella di cerare un form di
iscrizione alla Newsletter che soddisfi appieno la vigente normativa in
materia di Privacy e Trattamento dei dati, sarà necessario verificare,
per prima cosa, di aver creato, lato MailChimp, la lista utilizzata per
gestire gli iscritti alla Newsletter, con il campo "**Enable GDPR
fields**" opportunamente selezionato.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\mailchimp_gdpr_1.bmp](./assets/media/image38.png){width="4.584722222222222in"
height="2.5in"}

In queste condizioni il form di iscrizione associato in automatico da
MailChimp alla lista in esame, conterrà già alcuni campi necessari per
poter gestire e memorizzare i vari consensi che l'utente dovrà poi dare
per potersi effettivamente iscrivere alla Newsletter, campi questi che
potranno tranquillamente essere integrati, eliminati e personalizzati
secondo le normali modalità di editing proprie di MailChimp.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\mailchimp_gdpr_2.bmp](./assets/media/image39.png){width="4.584722222222222in"
height="3.1104166666666666in"}

**ATTENZIONE!** Non è possibile, per ovvie ragioni, eliminare
completamente tutti i check presenti all'interno della sezione
"Marketing Permission"

Lato Passweb, nel momento in cui la lista MailChimp utilizzata, dovesse
essere stata creata con il check "**Enable GDPR fields**" selezionato,
all'interno del form di iscrizione alla Newsletter, oltre ai normali
campi di iscrizione (es. Nome, Email ecc...) verrà visualizzato anche un
ulteriore elemento denominato "**Marketing Permission**" necessario per
poter gestire la corrispondente sezione presente all'interno del form di
iscrizione configurato su MailChimp.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\mailchimp_gdpr_3.bmp](./assets/media/image40.png){width="5.1625in"
height="3.4868055555555557in"}

**ATTENZIONE!** Il componente "Marketing Permission" non può essere
eliminato operando direttamente da Passweb.

A differenza di quanto avviene su MailChimp, dove all'interno della
sezione "Marketing Permission" sono presenti inizialmente tre diverse
possibili opzioni di scelta, rispettivamente **Email**, **Direct Email**
e **Customized Online Advertising** (opzioni queste che possono comunque
essere integrate e/o eliminate con il solo vincolo che almeno una deve
sempre essere presente), lato Passweb il componente "**Marketing
Permission**" evidenziato in figura presenta invece, a default, la sola
opzione "**Email**", opzione questa che l'utente dovrà eventualmente
selezionare per iscriversi alla Newsletter acconsentendo in maniera
esplicita a ricevere comunicazioni di carattere commerciale.

Nel momento in cui l'esigenza dovesse essere invece quella di gestire
più di un singolo consenso (es. consenso ad essere contattato via SMS,
consenso ad essere contattato telefonicamente ecc...) sarà necessario
configurare il Componente Passweb "Marketing Permission" andando ad
aggiungere esattamente le stesse opzioni presenti anche all'interno del
form di iscrizione configurato su MailChimp, prestando particolare
attenzione al fatto di utilizzare all'interno di Passweb le stesse
etichette assegnate su MailChimp alle relative opzioni.

In questo senso dunque, aprendo la maschera di gestione e configurazione
del componente "**Marketing Permission**" sarà possibile impostare un
valore per i seguenti parametri:

**Nome:** consente di personalizzare il nome assegnato al Componente in
esame (il nome assegnato a default è "Marketing Permission").

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

**Tab Index:** consente di personalizzare l'ordine di tabulazione del
form assegnando uno specifico numero d'ordine al campo in oggetto. Una
volta assegnato un numero d'ordine ad ogni campo del form sarà poi
possibile spostarsi da un elemento all'altro, utilizzando il tasto "TAB"
e secondo l'ordine di tabulazione impostato.

Nel caso in cui si decida di personalizzare l'ordine di tabulazione
degli elementi del form sarà necessario assegnare uno specifico numero
d'ordine ad ogni singolo campo. In caso contrario il passaggio da un
campo all'altro attraverso il tasto TAB si interromperà in
corrispondenza del campo con l'ultimo numero d'ordine impostato.

> **NOTA BENE:** il campo "Tab Index" non è un campo obbligatorio. Nel
> caso in cui si decida di non personalizzare l'ordine di tabulazione
> del form sarà poi il browser a definire gli spostamenti da un campo
> all'altro attraverso il tasto TAB

**Label (etichetta):** consente di personalizzare, in ciascuna delle
lingue attualmente gestite sul sito, l'etichetta che verrà visualizzata
in corrispondenza di questo particolare componente.

Il valore assegnato a default al campo in esame coincide esattamente con
quanto presente all'interno del campo "**Field label**" del
corrispondente componente "Marketing Permission" presente sul form di
iscrizione MailChimp

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\mailchimp_gdpr_5.bmp](./assets/media/image41.png){width="5.1625in"
height="3.4868055555555557in"}

**Descrizione:** consente di personalizzare, in ciascuna delle lingue
attualmente gestite sul sito, la descrizione visualizzata per questo
particolare componente immediatamente dopo l'etichetta definita
attraverso il precedente parametro.

Il valore assegnato a default al campo in esame coincide esattamente con
quanto presente all'interno del campo "**Description**" del
corrispondente componente "Marketing Permission" presente sul form di
iscrizione MailChimp

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\mailchimp_gdpr_6.bmp](./assets/media/image42.png){width="5.1625in"
height="3.4868055555555557in"}

**Ulteriore Testo:** consente di personalizzare, in ciascuna delle
lingue attualmente gestite sul sito, quanto presente all'interno del
campo "**Legal Text**" del corrispondente componente "Marketing
Permission" presente sul form di iscrizione MailChimp

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\mailchimp_gdpr_7.bmp](./assets/media/image43.png){width="5.1625in"
height="3.4868055555555557in"}

**Testo Legale MailChimp:** consente di personalizzare, in ciascuna
delle lingue attualmente gestite sul sito, il "Testo Legale Mailchimp"
ossia quel particolare testo che compare al di sotto dei check di
selezione dei consensi.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\mailchimp_gdpr_8.bmp](./assets/media/image44.png){width="5.1625in"
height="3.4868055555555557in"}

**ATTENZIONE!** Considerando che il "**Testo Legale MailChimp**" è
quello che viene utilizzato per esplicitare il fatto che i dati verranno
poi conservati dalla piattaforma MailChimp, sarebbe opportuno accertarsi
di non eliminare mai questo testo prestando anche particolare attenzione
al fatto di non modificare il link alle condizioni di privacy specifiche
di MailChimp stesso

**Campo Obbligatorio:** se selezionato, l'utente per potersi
effettivamente iscrivere alla Newsletter dovrà necessariamente
selezionare almeno uno dei check presenti all'interno del componente
acconsentendo quindi in maniera esplicita a ricevere determinate
comunicazioni di carattere commerciale.

**ATTENZIONE!** l'obbligatorietà del campo deve essere coerente con
quanto impostato lato MailChimp in corrispondenza del parametro
"**Require at least one option**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\mailchimp_gdpr_9.bmp](./assets/media/image45.png){width="5.1625in"
height="3.4868055555555557in"}

Nel momento in cui, lato MailChimp, dovesse quindi essere stato
selezionato il check evidenziato in figura, sarà poi necessario
accertarsi di aver selezionato sul componente "Marketing Permission" di
Passweb l'analogo check "Campo Obbligatorio"

La sezione "**Gestione valori"** consente di definire e gestire le
diverse possibili opzioni di scelta che verranno visualizzate
all'interno del controllo.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\mailchimp_gdpr_10.bmp](./assets/media/image46.png){width="5.902777777777778in"
height="3.7729166666666667in"}

Per aggiungere una nuova opzione di scelta al controllo è sufficiente
cliccare sul relativo pulsante di aggiunta nuovo elemento (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_aggiungi.bmp](./assets/media/image47.png){width="0.18194444444444444in"
height="0.18194444444444444in"} ) e inserire poi i dati di
configurazione dell'elemento stesso nella parte destra della maschera.

Per ciascuna delle possibili opzioni di scelta sarà necessario indicare:

- **Valore:** consente di specificare il valore che dovrà essere salvato
  nel momento in cui l'utente dovesse selezionare questa opzione.

- **Testo:** consente di indicare la label che dovrà essere
  visualizzata, all'interno del controllo, in corrispondenza
  dell'opzione di scelta che si sta configurando.

> **ATTENZIONE!** Nel caso in cui il campo "Testo" venga lasciato vuoto,
> label e valore dell'opzione di scelta coincideranno entrambi con
> quanto inserito all'interno del campo Valore.
>
> **NOTA BENE:** in ogni caso, alla conferma del form verrà sempre
> salvato solo **il Valore (e NON il Testo)** delle varie opzioni di
> scelta selezionate dall'utente

- **Selezionato:** flaggando questa casella l'opzione di scelta che si
  sta configurando apparirà sul sito già selezionato a default**.**

Una volta inserito un valore, per aggiungerlo all'elenco di valori
selezionabili, è necessario premere **"Aggiungi Elemento"** e
successivamente il tasto "**salva**".

Per **modificare** uno dei valori presenti in elenco è sufficiente
selezionarlo ed agire poi sulle relative proprietà.

Gli altri pulsanti presenti nella parte sinistra della maschera
consentono rispettivamente di:

- **Elimina elemento** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_elimina.bmp](./assets/media/image48.png){width="0.175in"
  height="0.18194444444444444in"} ): consente di eliminare l'elemento
  attualmente selezionata in elenco

- **Sposta su / giù**
  (![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icone_su_giu.bmp](./assets/media/image49.png){width="0.3701388888888889in"
  height="0.21458333333333332in"} ): consente di riordinare tra loro le
  varie opzioni di scelta spostando verso l'alto o il basso l'elemento
  attualmente selezionato in elenco.

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**ATTENZIONE!** Come precedentemente evidenziato, inizialmente,
all'interno del componente in esame sarà presente la sola opzione
"**Email**"

Nel momento in cui l'esigenza dovesse quindi essere quella di gestire
più di un singolo consenso, e quindi più di una singola opzione di
scelta sarà necessario:

- Inserire le opzioni di scelta desiderate direttamente all'interno del
  form di iscrizione configurato su MailChimp assegnando a ciascuna di
  esse uno specifico valore

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\mailchimp_gdpr_11.bmp](./assets/media/image50.png){width="5.1625in"
height="3.4868055555555557in"}

- Inserire all'interno della sezione "Gestione Valori" del Componente
  Passweb "Marketing Permission" esattamente le stesse opzioni di scelta
  configurate su MailChimp al punto precedente, presentando particolare
  attenzione al fatto di inserire per ciascuna di esse all'interno del
  campo Valore esattamente la stesso testo inserito anche su MailChimp

**ATTENZIONE!** Nel caso in cui non dovesse esserci corrispondenza tra
il Valore di un'opzione di scelta configurata su Passweb e le possibili
opzioni di scelta configurate invece su MailChimp il corrispondente dato
non potrà essere salvato

