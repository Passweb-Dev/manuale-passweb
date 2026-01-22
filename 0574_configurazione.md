# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_newsletter_configurazione.bmp](./assets/media/image146.png){width="5.084722222222222in"
height="3.0652777777777778in"}

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

**Nome**: consente di definire un nome per il Componente "Iscrizione
Newsletter " che si sta editando

**Pubblico**: consente di impostare la visibilità del componente in
esame. Lasciando il flag deselezionato, il relativo componente verrà
comunque inserito all'interno della pagina, sarà quindi visibile e
personalizzabile graficamente lato Wizard, ma NON risulterà visibile
lato Front End.

**Periodo di Pubblicazione:** consente di associare al Componente in
oggetto uno specifico periodo di pubblicazione, definendone l'effettiva
data di pubblicazione e la corrispondente data di oscuramento.

Nel primo dei due campi disponibili occorrerà quindi indicare,
utilizzando l'apposito calendario, la data di inizio pubblicazione. Nel
secondo campo andrà invece specificata la data di fine pubblicazione.

**ATTENZIONE!** Le date indicate all'interno di questi campi verranno
considerate solo ed esclusivamente nel caso in cui il precedente
parametro "Pubblico" sia stato selezionato

**Tipo di integrazione:** consente di specificare la piattaforma
utilizzata per gestire il sistema di Newsletter. E' possibile
selezionare una delle seguenti opzioni:

- MailChimp

- ActiveCampaign

- Brainlead

**ATTENZIONE!** dipendentemente dalla piattaforma selezionata varieranno
poi anche i parametri di configurazione da dover impostare

**Lista Associata -- disponibile per MailChimp / ActiveCampaign**:

Consente di indicare, selezionandola tra quelle gestite all'interno del
proprio account MailChimp/ActiveCampaign, la lista in cui dovrà essere
inserito l'utente che decide di iscriversi al servizio.

**ATTENZIONE!** impostando il campo in esame sull'opzione "Tutte" (solo
ActiveCampaign) l'utente verrà iscritto a tutte le Liste attualmente
presenti all'interno del proprio account

**ATTENZIONE**! nel caso di MailChimp per poter utilizzare una lista è
necessario che questa abbia associato almeno un gruppo di interesse

Il campo in esame è multilingua**.** E' quindi possibile associare una
diversa lista ad ogni singola lingua gestita all'interno del proprio
sito e utilizzare poi queste stesse liste all'interno di MailChimp per
inviare campagne di Newsletter in lingue diverse

**Invia Indirizzo -- disponibile solo per MailChimp:** se selezionato,
consente di inviare a MailChimp anche i dati relativi all'indirizzo di
fatturazione dell'utente che sta effettuando la registrazione al sito.

Queste informazioni verranno prelevate automaticamente dai relativi
campi Indirizzo, Città, Località, Cap, Nazione posto ovviamente che
questi stessi campi siano effettivamente presenti all'interno del form e
che siano anche stati correttamente valorizzati.

**ATTENZIONE!** affinché i dati relativi all'indirizzo possano essere
correttamente memorizzati e visualizzati nell'anagrafica utente di
MailChimp è necessario verificare di aver inserito all'interno del form
di iscrizione alla Newsletter (creato direttamente su MailChimp) il
campo "**Indirizzo**" e di e di aver impostato, in fase di
configurazione di questo stesso campo, il parametro "**Tag campo**" sul
valore "**ADDRESS**" (come evidenziato nella figura di seguito
riportata)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\mailchimp_campo_address.bmp](./assets/media/image147.png){width="5.701388888888889in"
height="3.3506944444444446in"}

**Tag per Campo Privato -- disponibile solo per MailChimp:** consente di
indicare il tag assegnato, in fase di configurazione del form di
iscrizione su MailChimp, al campo (testuale) utilizzato per memorizzare
l'informazione relativa al fatto che l'utente iscritto al servizio sia o
meno un Privato.

Nel momento in cui l'esigenza dovesse essere dunque quella di segmentare
il pubblico MailChimp distinguendo gli utenti "Privati" dagli utenti di
tipo "Azienda" sarà necessario:

- **lato MailChimp** verificare di aver correttamente inserito
  all'interno del form di iscrizione alla Newsletter un **campo
  testuale** adibito alla memorizzazione dell'informazione "Privato"

> **ATTENZIONE!** il campo utilizzato in MailChimp per memorizzare
> l'informazione "Privato" deve necessariamente essere un **campo di
> tipo Testo**

- **lato Passweb** verificare di aver correttamente inserito in
  corrispondenza del parametro "**Tag Campo per Privato"** lo stesso
  valore assegnato, in fase di configurazione del form di iscrizione su
  MailChimp, al parametro "**Tag Campo**" del campo utilizzato per
  memorizzare l'informazione relativa al fatto che l'utente iscritto al
  servizio sia o meno un Privato.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\mailchimp_campo_privato_azienda.bmp](./assets/media/image148.png){width="6.2659722222222225in"
height="2.33125in"}

In queste condizioni il campo Privato impostato su MailChimp non verrà
visualizzato nel form di iscrizione presente sul proprio sito Passweb ma
verrà comunque valorizzato con:

- **1** nel caso in cui l'utente che ha effettuato l'iscrizione al
  servizio dovesse essere effettivamente un utente di tipo "**Privato**"

- **0** nel caso in cui l'utente che ha effettuato l'iscrizione al
  servizio dovesse essere un utente di tipo "**Azienda**"

**Tag utilizzato se l'utente è un Privato / Azienda -- disponibile solo
per ActiveCampaign**:

Consente di indicare, selezionandolo tra quelli definiti all'interno del
proprio account ActiveCampaign lo specifico Tag da associare all'utente
che decide di iscriversi al servizio nel caso in cui questo stesso
utente dovesse essere un Privato / Azienda

Il campo in esame non è, ovviamente, obbligatorio ma potrebbe rivelarsi
particolarmente utile nel momento in cui l'esigenza dovesse essere
quella di segmentare il pubblico di ActiveCampaign distinguendo gli
utenti "Privati" dagli utenti di tipo "Azienda"

**Custom Field per consenso Marketing -- disponibile solo per
BrainLead**:

Consente di indicare, selezionandolo tra quelli presenti all'interno del
relativo menu a tendina, il campo Custom, di tipo GDPR, appositamente
creato su BrainLead, che dovrà essere utilizzato per gestire il consenso
all'iscrizione al sistema di Newsletter e, conseguentemente, alla
ricezione delle mail di carattere Marketing

**ATTENZIONE!** il parametro "**Custom Field per consenso Marketing**" è
obbligatorio. In conseguenza di ciò per poter gestire correttamente
l'iscrizione alla Newsletter di BrainLead sarà necessario creare sulla
piattaforma terza almeno un campo Custom di tipo GDPR da collegare poi
al parametro in oggetto

Il campo dichiarato in corrispondenza di questo parametro sarà infatti
quello collegato al Radio Button "**Iscrizione alla Newsletter Si /
No**" che comparirà poi all'interno del form di registrazione al sito
e/o all'interno del form di profilo utente.

![Videate\\componente_newsletter_mailchimp_1.bmp](./assets/media/image149.png){width="5.604166666666667in"
height="3.4743055555555555in"}

**Posizionamento dei Campi:** consente di posizionare gli elementi
principali del componente secondo uno schema prestabilito.

Nello specifico, gli elementi soggetti al tipo di posizionamento
impostato mediante questo parametro saranno:

- Il form di iscrizione

- Il pulsante di iscrizione

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

