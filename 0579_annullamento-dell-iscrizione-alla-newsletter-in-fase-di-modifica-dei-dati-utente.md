# ANNULLAMENTO DELL' ISCRIZIONE ALLA NEWSLETTER IN FASE DI MODIFICA DEI DATI UTENTE



Il fatto di inserire il componente "**Newsletter**" all'interno del form
di "Profilo" mette gli utenti del sito nelle condizioni non solo di
potersi iscrivere al servizio successivamente alla registrazione ma,
chiaramente, offre loro anche la possibilità di modificare i consensi
forniti e, volendo, di annullare l'iscrizione al servizio in un
qualsiasi momento.

**ATTENZIONE!** Come evidenziato nel precedente capitolo di questo
manuale, per fare in modo che l'utente possa effettivamente
visualizzare, una volta entrato nel suo profilo, la situazione
aggiornata relativamente alla sua iscrizione alla Newsletter e ai
consensi eventualmente forniti **è necessario accertarsi di aver
mappato, sia all'interno del componente Registrazione che all'interno
del componente Profilo, il campo Mail di iscrizione alla Newsletter con
il campo Mail utilizzato anche per la registrazione al sito**.

In queste condizioni infatti, supponendo che l'utente abbia già
effettuato l'iscrizione alla Newsletter fornendo anche determinati
consensi, entrando poi nel proprio Profilo si troverà il campo
"Iscrizione alla Newsletter" impostato a SI e, allo stesso modo, anche
eventuali check utilizzati per gestire i vari consensi (ricezione SMS,
telefonate ecc...) saranno selezionati o meno a seconda di quanto
precedentemente impostato.

A questo punto dunque operando direttamente dal Profilo sarà sempre
possibile modificare i consensi forniti, selezionando o deselezionando i
relativi check così come sarà sempre possibile riportare anche il radio
button "Iscrizione alla Newsletter" sul valore No, annullando di fatto
l'iscrizione al servizio.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_newsletter_mailchimp_1.bmp](./assets/media/image151.png)

**ATTENZIONE! quello che succederà effettivamente nel momento in cui
l'utente dovesse decidere di annullare l'iscrizione al servizio (radio
button "Iscrizione alla Newsletter" impostato sul valore No) dipenderà
dalla specifica piattaforma utilizzata per gestire il sistema di
Newsletter**

Nello specifico**, nel caso di MailChimp,** se un utente precedentemente
iscritto alla Newsletter dovesse impostare il Radio Button "Iscrizione
Newsletter" presente all'interno del suo Profilo, sul valore "**No**",
alla conferma la sua anagrafica verrà posta, all'interno della
corrispondente lista MailChimp, nello stato di "**Archiviato**"
lasciando comunque inalterati eventuali altri consensi da lui
precedentemente forniti.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\mailchimp_utente_archiviato.bmp](./assets/media/image53.png)

Nel caso di **ActiveCampaign** invece, se un utente precedentemente
iscritto alla Newsletter dovesse impostare il Radio Button "Iscrizione
Newsletter" presente all'interno del suo Profilo, sul valore "**No**",
alla conferma, l'utente verrà disiscritto dalla Lista indicata in fase
di configurazione del componente (campo "**Lista Associata**") lasciando
comunque inalterati, anche in questo caso i suoi dati anagrafici
compresi eventuali altri consensi da lui precedentemente forniti.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\annullamento_iscrizione_activecampaign_2.bmp](./assets/media/image163.png)

In queste condizioni starà dunque a chi gestisce l'invio delle varie
campagne e/o automazioni all'interno di ActiveCampaign accertarsi che le
mail a carattere commerciale siano inviate ai destinatari corretti.

**ATTENZIONE!** nel caso in cui il campo "**Lista Associata**" dovesse
essere stato impostato sull'opzione "**Tutte**" l'utente verrà
disiscritto da tutte le Liste presenti all'interno di ActiveCampaign

Nel caso di **BrainLead**, infine, se un utente precedentemente iscritto
alla Newsletter dovesse impostare il Radio Button "Iscrizione
Newsletter" presente all'interno del suo Profilo, sul valore "**No**",
alla conferma, nella relativa anagrafica Brainlead, il campo custom di
tipo GDPR settato in corrispondenza del parametro "**Custom Field per
consenso Marketing"**, verrà posto a No e allo stesso tempo l'utente
verrà effettivamente disiscritto dalla Newsletter (cosa questa
evidenziata anche dal piccolo badge rosso posto, nel dettaglio della
persona, in corrispondenza del suo indirizzo mail)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\brainlead_disiscrizione_profilo.bmp](./assets/media/image164.png)

Al solito, gli altri dati, compresi eventuali consensi precedentemente
forniti, non verranno invece modificati.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\brainlead_no_newsleeter_da_profilo.bmp](./assets/media/image165.png)

**ATTENZIONE! In tutti i casi (MailChimp, ActiveCampaign o Brainlead)
l'impostazione a No del radio button "Iscrizione Newsletter" presente
nel Profilo Utente non comporta l'eliminazione della relativa anagrafica
sulla piattaforma terza ma, semplicemente, mette l'utente stesso nelle
condizioni di non ricevere più mail di carattere commerciale.**

Ovviamente l'utente potrebbe sempre decidere, in un qualsiasi altro
momento, di iscriversi nuovamente al servizio fornendo gli stessi
consensi che aveva dato in precedenza o anche dei consensi diversi e, al
salvataggio del profilo (posto ovviamente che venga utilizzata sempre la
stessa Email), la sua anagrafica verrà aggiornata di conseguenza anche
sulla piattaforma terza.

Per quel che riguarda invece la possibilità/necessità di eliminare
completamente l'anagrafica dell'utente sul database della piattaforma
terza, questa è, ovviamente, un'operazione che potrà effettuare in
completa autonomia lo stesso utente operando sempre dal suo Profilo
utilizzando, nello specifico, **il pulsante "Elimina Profilo"**.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\elimina_profilo.bmp](./assets/media/image27.png)

**Cliccando su questo pulsante infatti oltre a cancellare la sua
anagrafica dal database di Passweb, questa verrà completamente eliminata
anche dal database della piattaforma terza utilizzata per la gestione
delle Newsletter.**

Nel momento in cui si dovesse implementare l'integrazione con una delle
piattaforme di newsletter gestite da Passweb si consiglia quindi di
personalizzare il messaggio di "conferma eliminazione del profilo"
indicando che i dati dell'utente verranno, eventualmente, cancellati
anche dalla piattaforma di newsletter utilizzata.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\messaggio_conferma_eliminazione_profilo.bmp](./assets/media/image28.png)

**ATTENZIONE!** In queste condizioni va ricordato inoltre che:

- se la piattaforma utilizzata per la Newsletter dovesse essere
  MailChimp, un utente eliminato in maniera definitiva potrà
  eventualmente reiscriversi alla stessa Newsletter **solo attraverso
  uno dei form nativi di MailChimp stesso** (l'iscrizione attraverso
  form Passweb, quindi, non potrà più essere utilizzata)

- La cancellazione dell'anagrafica utente effettuata dal backend
  (Wizard) del sito Passweb NON comporta l'eliminazione della stessa
  anagrafica anche dal database della piattaforma utilizzata per gestire
  la Newsletter.

