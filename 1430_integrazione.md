# INTEGRAZIONE



**ATTENZIONE! Per usufruire dell'integrazione tra Passweb e Clerk è
necessario attivare il relativo modulo su Passstore**

Una volta attivato il modulo sarà necessario, per prima cosa, cliccare
sulla voce "**Gestisci Integrazioni**" presente all'interno della
sezione "**Integrazioni**" del menu "**Sito**".

In questo modo si avrà infatti accesso alla maschera "**Lista degli
Account**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ac_2.bmp](./assets/media/image2.png){width="5.454861111111111in"
height="3.532638888888889in"}

contenente l'elenco di tutti gli Account relativi alle piattaforme di
Marketing (diverse da MailChimp) attualmente collegate e integrate con
il proprio sito Ecommerce.

Il pulsante **Aggiungi Account** ( ), presente nella barra degli
strumenti, consentirà di accedere alla maschera "**Dati Account**"
all'interno della quale poter impostare tutti i parametri necessari per
attivare l'integrazione tra il proprio sito Passweb e la piattaforma
selezionata

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ac_3.bmp](./assets/media/image3.png){width="5.7659722222222225in"
height="3.454861111111111in"}

In questo senso il campo

- **Descrizione:** consente di assegnare un'etichetta identificativa
  all'Account che si sta configurando

- **Piattaforma:** consente di indicare, selezionandola tra quelle
  presenti in elenco, la specifica piattaforma con cui si desidera
  realizzare l'integrazione.

Nel caso in esame sarà quindi necessario impostare quest'ultimo campo
sull'opzione "**Clerk**"

Verrà quindi visualizzata la sezione "**Credenziali**" all'interno della
quale troveremo due ulteriori campi "**Api Key**" e "**Private Key**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\clerk_1.bmp](./assets/media/image4.png){width="5.370138888888889in"
height="3.4611111111111112in"}

all'interno dei quali dovremo inserire rispettivamente:

- **Api Key**: consente di inserire la chiave pubblica da utilizzare per
  l'integrazione Passweb -- Clerk.

> Tale chiave può essere prelevata direttamente all'interno della
> sezione "**Developer -- API Keys**" (campo "**Public API key**") dello
> store creato all'interno del proprio account Clerk

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\clerk_public_api_key.bmp](./assets/media/image5.png){width="5.370138888888889in"
height="3.33125in"}

- **Private Key**: consente di inserire la chiave privata da utilizzare
  per l'integrazione Passweb -- Clerk

> Per ottenere questa chiave sarà necessario accedere, anche in questo
> caso, alla sezione **Developer -- API Keys**" dello store creato
> all'interno del proprio account Clerk e cliccare, questa volta, sul
> pulsante "**Create new**" presente in corrispondenza della sezione
> "**Private API Keys**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\clerk_private_api_key.bmp](./assets/media/image6.png){width="5.370138888888889in"
height="3.33125in"}

> **ATTENZIONE!** la chiave privata verrà visualizzata in forma completa
> solo in fase di creazione dopo di che verrà inserita asteriscata nella
> tabella sottostante e non sarà più possibile recuperarne il valore
>
> Nel caso in cui si rendesse necessario, per una qualsiasi ragione,
> reinserire questa chiave all'interno di Passweb sarà necessario
> invalidare la vecchia chiave (mediante il pulsante con i tre puntini
> presente a fianco della chiave stessa) e crearne una nuova.

**ATTENZIONE! chiave pubblica e chiave privata sono diverse per ogni
store Clerk**

Nel momento in cui l'esigenza dovesse quindi essere quella di gestire
siti in multilingua con la conseguente creazione di uno store Clerk per
ogni lingua gestita, sarà necessario creare anche account Clerk distinti
all'interno di Passweb e configurare ciascuno di essi utilizzando le
chiavi pubblica e privata dello store Clerk corretto.

Per maggiori informazioni relativamente all'integrazione Passweb --
Clerk nel caso di siti multilingua si veda anche quanto indicato nel
relativo capitolo ("*Passweb e Clerk -- Integrazione -- Multilingua*")
di questo manuale

Il pulsante "**Test Connessione**" presente nella parte bassa della
sezione "**Credenziali**" consente di verificare che le chiavi inserite
siano corrette e che quindi la comunicazione tra Passweb e Clerk può
effettivamente avvenire senza problemi.

Ovviamente prima di effettuare il test di connessione sarà necessario
aver impostato entrambe le chiavi e aver salto la pagina cliccando sul
pulsante "**Salva**". Il risultato del test di connessione verrà poi
visualizzato attraverso un piccolo pop up presente nella parte bassa
della pagina

Una volta salvate le due chiavi compariranno:

- La sezione "**Parametri Store**" all'interno del tab
  "**Configurazione**"

- I nuovi tab **Ordini**, **Clienti**, **Categorie**, **Articoli** e
  **Pagine**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\clerk_2.bmp](./assets/media/image7.png){width="5.370138888888889in"
height="3.33125in"}

Per maggiori informazioni relativamente a ciascuna delle sezioni sopra
evidenziate si vedano i successivi capitoli di questo manuale.

