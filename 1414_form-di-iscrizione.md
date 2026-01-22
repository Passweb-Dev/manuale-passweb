# FORM DI ISCRIZIONE



Oltre al sistema di tracciamento evidenziato in precedenza, cui possono
essere collegate diverse automazioni ecommerce, Brainlead consente di
gestire anche un classico sistema di newsletter cui gli utenti del sito
dovranno iscriversi in maniera volontaria dando tutti i consensi del
caso (coerentemente con quanto previsto dalla vigente normativa in
materia di privacy e trattamento dei dati)

In questo senso diventa di fondamentale importanza il fatto di poter
gestire in maniera corretta il form di iscrizione che l'utente dovrà
compilare per aderire al servizio, form questo che, per prima cosa,
dovrà necessariamente essere creato all'interno di Brainlead.

**ATTENZIONE!** Per maggiori informazioni relativamente a come poter
creare e configurare un form di iscrizione alla Newsletter all'interno
di Brainlead si rimanda alla specifica documentazione di prodotto

(<https://help.brainlead.it/support/solutions/articles/44001966185>)

Una volta creato il form sarà poi necessario inserirlo all'interno del
sito Passweb e per far questo sarà possibile procedere in due modi
diversi, dipendentemente, in sostanza, dal fatto di voler gestire o meno
in un unico processo la registrazione al sito e la registrazione al
sistema di newsletter:

- utilizzando uno dei metodi di integrazione messi a disposizione da
  Brainlead

- utilizzando i componenti nativi di Passweb

Nel primo caso, una volta creato il form sarà sufficiente accedere alla
sezione "**Web Forms**" di Brainlead, aprire il menù a tendina cliccando
sul relativo pulsante posto in corrispondenza del form stesso e
selezionare poi la voce "**Integrazioni con il sito web**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\form_brainlead_1.bmp](./assets/media/image9.png)

In questo modo verrà infatti visualizzata la schermata con i vari metodi
di integrazione (e le relative istruzioni), tra cui poter scegliere (per
maggiori informazioni in merito ai singoli metodi di integrazione si
rimanda alla relativa documentazione di prodotto.)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\form_brainlead_2.bmp](./assets/media/image10.png)

**Ovviamente questo tipo di soluzione non consente di realizzare un
processo di iscrizione alla Newsletter contestuale al processo di
registrazione al sito.**

In queste condizioni andranno per forza di cose gestiti due diversi
form, quello per la registrazione al sito e quello per l'iscrizione al
sistema di Newsletter.

Nel momento in cui l'esigenza dovesse essere invece quella di mettere
l'utente nelle condizioni di iscriversi alla newsletter contestualmente
alla registrazione al sito, sarà necessario ricorrere alla seconda
opzione gestendo quindi il form di iscrizione con i componenti nativi di
Passweb e, nello specifico, con il componente **"Newsletter (MailChimp o
BrainLead)"**, componente questo che dovrà essere inserito, per
l'appunto, all'interno del form di "**Registrazione Utente**".

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_newsletter.bmp](./assets/media/image11.png)

In queste condizioni, una volta configurato correttamente il componente
in oggetto, all'interno del form di registrazione al sito verrà
visualizzato anche un Radio Button con le due opzioni **Si / No**,
**opzioni queste che** **permetteranno all'utente di poter decidere se
iscriversi o meno anche alla Newsletter**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_newsletter_mailchimp_1.bmp](./assets/media/image12.png)

**ATTENZIONE!** per poter visualizzare il Radio Button "**Iscrizione
alla Newsletter**" è necessario aver configurato su BrainLead almeno un
campo custom di tipo GDPR e averlo poi dichiarato, in fase di
configurazione del Componente Passweb "**Newsletter (MailChimp o
BrainLead)",** in corrispondenza del parametro "**Custom Field per
consenso Marketing**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\brainlead_campo_gdpr_marketing.bmp](./assets/media/image13.png)

Nel caso in cui l'utente dovesse decidere di registrarsi al sito senza
iscriversi alla Newsletter (opzione **No**), il campo Custom dichiarato
in corrispondenza del parametro "Custom Field per consenso Marketing"
verrà valorizzato di conseguenza (quindi a No) anche su BrainLead, e
eventuali altri campi del form di iscrizione definiti su Brainlead non
verranno mai visualizzati.

Nel momento in cui l'utente dovesse invece decidere di iscriversi anche
alla Newsletter (opzione **Si**), il campo Custom dichiarato in
corrispondenza del parametro "Custom Field per consenso Marketing" verrà
valorizzato di conseguenza (quindi a Si) anche sui BrainLead e, inoltre,
verranno anche visualizzati **i campi custom (ed eventualmente il campo
mail)** che si è deciso, in fase di configurazione, di voler
effettivamente visualizzare.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\newsletter_registrazione3.bmp](./assets/media/image14.png)

Per maggiori informazioni relativamente a come poter gestire il form di
iscrizione alla newsletter Brainlead all'interno del form di
registrazione utente si veda quanto indicato nel capitolo *"Componenti
Interazione Utente -- Componenti interni ai componenti interazione
utente -- Componente Newsletter -- Iscrizione alla Newsletter Brainlead
in fase di registrazione al sito"* di questo manuale

**ATTENZIONE!** a differenza delle cosiddette mail transazionali
(conferma ordine, carrelli abbandonati ...) le mail generate da un
sistema di newsletter sono, tipicamente, mail di carattere marketing

Si consiglia quindi, in fase di creazione del form di iscrizione, di
prestare sempre particolare attenzione al fatto di aver gestito in
maniera adeguata anche tutti i campi necessari per i diversi consensi
marketing, consensi questi che, in accordo con la vigente normativa in
materia di GDPR, gli utenti dovranno poi andare a fornire prima di
potersi effettivamente iscrivere al servizio.

In questo senso sarà possibile creare su BrainLead appositi campi custom
di tipo GDPR che serviranno proprio a raccogliere questo tipo di
consensi e che dovranno quindi essere riportati anche all'interno dei
form di iscrizione presenti sul proprio sito Passweb.

Nello specifico poi, come precedentemente evidenziato, uno di questi
campi GDPR dovrà essere utilizzato obbligatoriamente per gestire il
consenso all'iscrizione al sistema di Newsletter e alla ricezione dunque
delle mail di carattere Marketing.

Tale campo dovrà essere dichiarato in fase di configurazione del
componente **"Newsletter (MailChimp o BrainLead)"** (parametro "**Custom
Field per consenso Marketing**") e sarà, di fatto, quello collegato al
Radio Button "Iscrizione alla Newsletter Si / No" che potrà comparire,
ad esempio, all'interno del form di registrazione al sito e/o
all'interno del form di profilo utente.

Eventuali altri campi custom di tipo GDPR creati su BrainLead potranno
invece servire per inserire all'interno del proprio form di iscrizione
dei check per la raccolta, ad esempio, del consenso relativo alla
ricezione di SMS, di telefonate o di qualsiasi altro consenso che possa
effettivamente essere richiesto dalla normativa vigente

**ATTENZIONE!** **ovviamente tutte le campagne e le automazioni create
su BrainLead dovranno tener conto dei consensi espressi dagli utenti e
dunque dal valore assunto dai diversi campi custom di tipo GDPR**

Per maggiori informazioni relativamente a come poter creare un form di
iscrizione alla Newsletter Brainlead GDPR compliance, e a come poter
gestire correttamente le varie campagne e automazioni, si rimanda alla
specifica documentazione di prodotto e/o al relativo supporto tecnico.

Infine, parlando sempre di componenti nativi di Passweb, è bene
sottolineare la possibilità di inserire il componente "**Newsletter
(MailChimp o BrainLead)"** anche all'interno:

- **del form di "Profilo Utente"**: in questo modo gli utenti che hanno
  effettuato la registrazione al sito Passweb avranno la possibilità di
  gestire i vari consensi e di annullare la propria iscrizione operando
  direttamente dal loro profilo (per maggiori informazioni in merito si
  veda anche quanto indicato all'interno del capitolo "*Componenti
  Interazione Utente -- Componenti interni ai componenti interazione
  utente -- Componente Newsletter -- Iscrizione alla Newsletter
  MailChimp / Brainlead in fase di modifica dei dati utente*" di questo
  manuale)

- **di un qualsiasi "Form Generico"**: in questo modo sarà possibile
  gestire un form di iscrizione alla Newsletter, scollegato dal form di
  registrazione al sito, utilizzando comunque i componenti nativi di
  Passweb anziché uno dei metodi di integrazione messi a disposizione da
  Brainlead (per maggiori informazioni in merito si veda anche quanto
  indicato all'interno del capitolo "*Componenti Interazione Utente --
  Componenti interni ai componenti interazione utente -- Componente
  Newsletter -- Iscrizione alla Newsletter MailChimp / Brainlead
  mediante form generico*" di questo manuale)

> **ATTENZIONE!** Nel caso in cui si sia deciso di utilizzare BrainLead
> come sistema di gestione delle Newsletter e il componente "Form"
> generico di Passweb per gestire il form di iscrizione al servizio, gli
> unici dati passati a BrainLead al momento dell'iscrizione, potranno
> essere soltanto l'indirizzo mail ed eventuali campi custom.

