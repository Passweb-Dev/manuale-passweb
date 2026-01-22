# ISCRIZIONE AL SISTEMA DI NEWSLETTER MAILCHIMP ESTERNAMENTE AL FORM DI REGISTRAZIONE AL SITO



Nel momento in cui l'esigenza dovesse essere quella di creare un form di
iscrizione al sistema di Newsletter gestito da MailChimp esternamente al
form di Registrazione al sito sarà possibile seguire due strade
differenti:

- Utilizzare uno dei metodi di integrazione messi a disposizione da
  MailChimp

- Utilizzare i componenti nativi di Passweb

Nel primo caso, una volta creato il form di iscrizione direttamente su
MailChimp, sarà poi possibile decidere di visualizzarlo con un pop up
oppure utilizzando uno dei Widget messi a disposizione direttamente da
MailChimp

![](./assets/media/image36.png)

In ogni caso, in queste condizioni, la gestione del form è demandata
direttamente alla piattaforma terza (per maggiori informazioni
relativamente ai diversi metodi di integrazione messi a disposizione da
MailChimp si rimanda alla relativa documentazione)

Nel secondo caso sarà necessario invece utilizzare il componente di
primo livello "Iscrizione Newsletter" impostando i parametri di
configurazione "**Tipo di Integrazione**" e "**Tipologia Form**"
rispettivamente sui valori "**MailChimp**" e "**Iscrizione**"

![](./assets/media/image37.png)

In queste condizioni, impostati correttamente anche tutti gli altri
parametri di configurazione, al salvataggio del componente
l'applicazione si preoccuperà di contattare MailChimp, utilizzando l'API
Key inserita in fase di configurazione del sito (pagina "**Sito --
Preferenze**", tab "**Integrazioni**", campo "**MailChimp API Key**"),
prelevando il form associato alla lista selezionata (**Signup**
**form)** e andrà poi ad inserire automaticamente i relativi campi
all'interno della pagina del sito Passweb.

**ATTENZIONE!** **I campi presenti all'interno del form di iscrizione
dipenderanno, quindi, direttamente da come è stato costruito il
corrispondente form all'interno di MailChimp oltre che dal fatto di aver
creato o meno, sempre lato MailChimp, un form di iscrizione GDPR
compliance.** Per maggiori informazioni in merito si veda anche il
successivo capitolo di questo manuale ("Form di inscrizione alla
newsletter GDPR Compliance)

A questo punto sarà possibile personalizzare graficamente il form di
iscrizione alla Newsletter secondo le tradizionali modalità di editing
grafico disponibili in Passweb, come se fosse dunque un semplice
componente di tipo Form o di tipo Registrazione Utente.

**NOTA BENE**: gli unici componenti che possono essere inseriti
all'interno del form di iscrizione sono quelli appartenenti alla sezione
dei "Componenti Comuni".

Relativamente ai componenti del form di iscrizione alla Newsletter
(campi di input, radio button, combo box ecc ...) prelevati direttamente
da MailChimp, questi potranno essere sposati, modificando quindi il loro
ordinamento rispetto a quello impostato in MailChimp e personalizzati
graficamente **ma non sarà possibile né eliminarli né tanto meno
copiarli.**

**Questo tipo di operazioni dovranno infatti essere effettuate
obbligatoriamente all'interno di MailChimp**.

Sarà invece possibile modificare l'etichetta identificativa di questi
campi. Tali variazioni, poi, potrebbero o meno essere sovrascritte al
salvataggio del componente stesso, con i relativi valori presenti in
MailChimp dipendentemente dall'impostazione adottata per il parametro
**"Aggiorna sempre le Label da MailChimp"** presente all'interno del
menu "Preferenze"

**NOTA BENE**: in generale ogni volta che viene salvato il componente
"Iscrizione Newsletter" l'applicazione si preoccuperà di contattare il
relativo account MailChimp verificando eventuali variazioni (aggiunta di
nuovi campi, cancellazione di campi precedentemente esistenti ecc ...)
al form di iscrizione ed aggiornando, di conseguenza, il form presente
in Passweb.

Nel momento in cui l'esigenza dovesse essere quella di "sincronizzare"
il form di iscrizione alla Newsletter di Passweb con quello presente in
MailChimp, a seguito ad esempio di alcune modifiche apportate in
MailChimp stesso a questo form, sarà quindi sufficiente abilitare, in
Passweb, la modalità di gestione dei componenti, selezionare il
componente "Iscrizione Newsletter" desiderato e cliccare pio sul
pulsante "Modifica Contenuto" presente nel ROC di questo componente,
visualizzando così la stessa maschera "**Modifica Iscrizione
Newsletter**" precedentemente evidenziata.

A questo punto per allineare il contenuto del form presente in Passweb
con quello presente in MailChimp sarà sufficiente cliccare sul pulsante
"**Salva**" presente nella parte bassa di questa maschera.

Un'ultima considerazione di fondamentale importanza da fare è quella
relativa al fatto che, in queste condizioni, trattandosi di form di
iscrizioni alla Newsletter scollegati dal form di Registrazione al sito
si potrebbe pensare anche di gestire il tutto non con i componenti
nativi di Passweb ma integrando direttamente il form di iscrizione
creato su MailChimp con uno dei metodi di integrazione messi a
disposizione da MailChimp stesso (per maggiori informazioni in merito si
rimanda alla specifica documentazione di MailChimp)

