# FORM DI RICHIESTA INFORMAZIONI



Il componente Form, presente tra i Componenti Comuni del proprio sito
Passweb, consente, come evidenziato anche nei precedenti capitoli di
questo manuale, di raccogliere e memorizzare automaticamente all'interno
del gestionale, richieste relative a soggiorni presso strutture gestite
con Passepartout Welcome.

In questo senso infatti inserendo un Componente Form all'interno di una
qualsiasi pagina di un sito Hotel troveremo tra i suoi parametri di
configurazione, in corrispondenza del campo "**Tipo Valore**", anche
l'opzione "**Richiesta di Passepartout Welcome**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\form_welcome_configurazione.bmp](./assets/media/image7.png)

Selezionando questa opzione, disponibile solo nel caso in cui il form
sia stato inserito all'interno di una pagina di un sito Hotel (tipologia
"Passweb") alla conferma i dati in esso contenuti creeranno
automaticamente una richiesta che verrà inserita all'interno della
corrispondente sezione del gestionale (menu "*Richieste*")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\welcome_richieste_prenotazione.bmp](./assets/media/image8.png)

Il campo "**Invia Email di Riepilogo al Cliente**", anch'esso
visualizzato solo nel caso in cui il campo "**Tipo Valore**" sia stato
impostato sull'opzione "**Richiesta di Passepartout Welcome**",
consentirà invece di decidere se alla conferma del form dovrà o meno
essere inviata una mail di riepilogo anche all'utente che lo ha
compilato.

**ATTENZIONE!** La mail di riepilogo verrà inviata direttamente da
Welcome utilizzando i relativi template. Per maggiori informazioni
relativamente a come poter eventualmente personalizzare questa mail si
rimanda quindi alla specifica documentazione del gestionale

**ATTENZIONE!** affinché i dati del form possano essere inseriti
correttamente nel gestionale sarà necessario:

- Aver impostato in maniera adeguata i parametri di configurazione
  presenti alla pagina "**Parametri Configurazione WebBooking**" del
  Wizard

- Configurare e strutturare il form in un certo modo

In questo senso occorre infatti sottolineare che per fare sì che tutto
possa funzionare correttamente il form di richiesta informazioni dovrà
essere creato con determinati campi e seguendo determinate regole.

Di seguito verrà quindi indicato l'elenco dei campi da inserire
all'interno di questo tipo di form e come questi stessi campi dovranno
essere configurati per fare in modo che l'informazione venga poi
memorizzata all'interno del corrispondente campo gestionale.

**ATTENZIONE!** I parametri di configurazione dei componenti Passweb non
indicati in maniera specifica all'interno dei successivi capitoli di
questo manuale potranno essere compilati secondo le specifiche esigenze
del cliente e secondo quando indicato nei relativi capitoli di questo
manuale

