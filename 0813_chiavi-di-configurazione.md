# CHIAVI DI CONFIGURAZIONE



Il primo passaggio per poter integrare il proprio sito Passweb con la
piattaforma di eBay è quello di procurarsi almeno un set di Chiavi di
Configurazione valide, chiavi queste relative ad una specifica
applicazione all'interno dell'ambiente developer di eBay, e che verranno
poi utilizzate dal sito per comunicare con eBay inviando tutti gli
articoli che l'utente ha deciso di mettere in vendita su questa
piattaforma e prelevando da questa stessa piattaforma eventuali nuovi
ordini con i relativi clienti.

**ATTENZIONE!** Per ogni set di chiavi di configurazione è possibile
generare un massimo di 5000 chiamate giornaliere alle API di eBay

Per ottenere un Set di Chiavi di Configurazione valide è necessario,
innanzi tutto, registrarsi al sito <https://go.developer.ebay.com>
cliccando per questo sul relativo pulsante presente in testata.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\ebay_1.bmp](./assets/media/image1.png)

Una volta effettuata la registrazione ed effettuato l'accesso
all'ambiente developer di eBay, sarà poi necessario creare una nuova
applicazione assegnandogli un nome, campo **"Application Title"** (1) e
successivamente cliccare sul pulsante "**Create a keyset**" presente in
corrispondenza della sezione **"Sandbox"** (2) o **"Production"** (3)
per creare il Set di Chiavi di Configurazione relativo rispettivamente
all'ambiente di Test oppure e a quello di Produzione

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\ebay_2.bmp](./assets/media/image2.png)

**ATTENZIONE! E' necessario creare il set di Chiavi di Configurazione
tanto per l'ambiente di Test quanto per quello di Produzione.**

All'interno di Passweb andranno infatti inserite le chiavi di
configurazione relative ad entrambi gli ambienti. In ogni caso il
processo di creazione delle chiavi relative all'ambiente di Test o a
quello di Produzione è esattamente lo stesso

Una volta confermati i dati dell'account cliccando sul pulsante
**"Continue to Create Keys"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\ebay_4.bmp](./assets/media/image3.png)

verranno generate tutte le chiavi di configurazione necessarie per
realizzare l'integrazione tra il proprio sito Ecommerce e la piattaforma
di eBay.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\ebay_5.bmp](./assets/media/image4.png)

Tali chiavi dovranno quindi essere inserite all'interno del proprio sito
Passweb.

Per fare questo è necessario accedere alla maschera **"Lista delle
Chiavi di Configurazione eBay"** presente all'interno della sezione
"**Catalogo -- eBay -- Chiavi di Configurazione**" del Wizard, maschera
questa all'interno della quale verranno visualizzate tutte le chiavi di
configurazione attualmente inserite all'interno del proprio sito

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ebay_7.bmp](./assets/media/image5.png)

Il pulsante **"Aggiungi Chiave" (**
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_aggiungi_chiave.bmp](./assets/media/image6.png) **)** presente nella contestuale barra
degli strumenti consente di creare un nuovo set di chiavi di
configurazione. Cliccando su di esso verrà infatti aperta la maschera
**Chiavi di Configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ebay_6.bmp](./assets/media/image7.png)

all'interno della quale poter inserire le chiavi di configurazione
precedentemente ottenute.

Nello specifico, ovviamente, all'interno della sezione "**Chiavi di
Produzione**" andranno inserite le chiavi relative al set configurato
per l'ambiente di Produzione, all'interno della sezione "**Chiavi della
Sandbox**" andranno invece inserite le chiavi relative al set
configurato per l'ambiente di Test

**ATTENZIONE!** Oltre alle tre chiavi "**App ID**", "**Dev ID**" e
"**Cert ID**", per completare la configurazione sarà necessario inserire
anche il "**RuName (eBay Redirect URL name)"** o "**Sandbox RuName"**,
dipendentemente dal fatto di lavorare sull'ambiente di produzione o su
quello di test

Per ottenere quest'informazione è necessario innanzitutto portarsi
nuovamente su eBay nella pagina di generazione delle chiavi di
configurazione e cliccare sulla voce **"User Tokens"** presente in
corrispondenza della chiave **"App ID"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\ebay_9.bmp](./assets/media/image8.png)

Aprire quindi la sezione **"Get a Token from eBay via Your
Application"** (1) e cliccare sul pulsante **"Add eBay Redirect URL"**
(2)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\ebay_10.bmp](./assets/media/image9.png)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\ebay_11.bmp](./assets/media/image10.png)

Una volta inserti i dati richiesti cliccando sul pulsante "**Continue to
create RuName**" verrà creato il proprio "**eBay Redirect URL**" che
potremo quindi prelevare ed inserire all'interno dell'apposito campo sul
Wizard di Passweb

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\ebay_12.bmp](./assets/media/image11.png)

Una volta inserita anche questa informazione, per completare la
creazione della "Chiave di Configurazione" necessaria per realizzare
l'integrazione tra Passweb ed eBay, sarà necessario assegnare un nome
alla Chiave (campo "Nome") e decidere se attivarla o meno (campo
"Attiva")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ebay_13.bmp](./assets/media/image12.png)

**ATTENIONE!** E' possibile impostare più chiavi di configurazione ma
sarà poi possibile attivarne soltanto una

I pulsanti presenti nella barra degli strumenti della maschera "Lista
delle Chiavi di Configurazione eBay" consentono, infine, di:

- **Aggiungi Chiave (**
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_aggiungi_chiave.bmp](./assets/media/image6.png) **):** consente di aggiungere un nuovo
  seti di chiavi di configurazione

- **Modifica Chiave (**
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_modifica_chiave.bmp](./assets/media/image13.png) **):** consente di modificare il set
  di chiavi di configurazione attualmente selezionato in elenco

- **Elimina Chiave (**
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_elimina_chiave.bmp](./assets/media/image14.png) **):** consente di eliminare il set di chiavi di
  configurazione attualmente selezionato in elenco

- **Attiva Chiave (**
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_attiva_chiave.bmp](./assets/media/image15.png) **) / Disattiva Chiave (**
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_disattiva_chiave.bmp](./assets/media/image16.png) **):** consente di attivare /
  disattivare il seti di chiavi di configurazione attualmente
  selezionato il elenco

**ATTENIONE!** Per poter realizzare l'integrazione tra il proprio sito
Passweb ed eBay è indispensabile aver attivato almeno un Set di Chiavi
di Configurazione

