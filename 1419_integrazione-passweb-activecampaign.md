# INTEGRAZIONE PASSWEB -- ACTIVECAMPAIGN



**ATTENZIONE! Per usufruire dell'integrazione tra Passweb e
ActiveCampaign è necessario attivare il relativo modulo su Passstore**

Una volta attivato il modulo sarà poi necessario, per prima cosa,
cliccare sulla voce "**Gestisci Integrazioni**" presente all'interno
della sezione "**Integrazioni**" del menu principale

In questo modo si avrà infatti accesso alla maschera "**Lista degli
Account**"

![](./assets/media/image2.png)

contenente l'elenco di tutti gli Account relativi alle piattaforme di
Marketing (diverse da MailChimp) attualmente collegate e integrate con
il proprio sito Ecommerce.

Il pulsante **Aggiungi Account** ( ), presente nella barra degli
strumenti, consentirà di accedere alla maschera "**Dati Account**"
all'interno della quale poter impostare tutti i parametri necessari per
poter attivare l'integrazione tra il proprio sito Passweb e la
piattaforma di Marketing gestita

![](./assets/media/image3.png)

Nello specifico il campo:

- **Descrizione:** consente di assegnare un'etichetta identificativa
  all'Account che si sta configurando

- **Piattaforma:** consente di indicare, selezionandola tra quelle
  presenti in elenco, la specifica piattaforma di Marketing con cui si
  desidera realizzare l'integrazione.

Impostando quest'ultimo campo sul valore "**ActiveCampaign**" verranno
quindi visualizzati due ulteriori campi (sezione "**Credenziali**")
all'interno dei quali dovranno essere inseriti dei valori prelevati
direttamente dalla piattaforma di ActiveCampaign

![](./assets/media/image4.png)

In particolare il campo

- **Nome Account**: consente di impostare il nome dell'Account di
  ActiveCampaign con cui si desidera integrare il proprio sito Ecommerce

> Per ottenere questa chiave sarà necessario accedere al proprio Account
> di ActiveCampaign portandosi all'interno della sezione "**Impostazioni
> -- Sviluppatore**"

![](./assets/media/image5.png)

> dove troveremo, all'interno del campo "**URL**", l'indirizzo per poter
> accedere alle API della piattaforma.
>
> **ATTENZIONE! Il valore da inserire in corrispondenza del campo
> Passweb "Nome Account" corrisponde al nome del dominio di terzo
> livello assegnato a questo url**
>
> Facendo quindi riferimento all'esempio riportato in figura, dove il
> nome completo dell'Account corrisponde a
>
> **https://passepartoutspa1617115965.api-us1.com**
>
> il valore che dovremo andare ad inserire su Passweb, all'interno del
> campo "Nome Account" sarà semplicemente
>
> **passepartoutspa1617115965**

- **API Key**: consente di impostare la chiave di integrazione che
  permetterà di attivare la comunicazione tra le due piattaforme

> Il valore da inserire all'interno di questo campo potremo trovarlo,
> ancora una volta, nella sezione "**Impostazioni -- Sviluppatore**"
> dell'account di ActiveCampaign in corrispondenza del campo
> "**Chiave**" evidenziato in figura

![](./assets/media/image6.png)

Dopo aver impostato tutti i parametri presenti all'interno della
maschera "Dati Account" i due pulsanti presenti nella parte bassa della
pagina consentiranno rispettivamente di:

- **Salva**: consente di salvare le impostazioni di configurazione
  settate per l'Account in esame.

- **Test Connessione**: consente di avviare un test di connessione tra
  Passweb e la piattaforma terza

Ovviamente prima di effettuare il test di connessione sarà necessario
aver impostato correttamente, **e salvato**, tutti i parametri di
configurazione richiesti dallo specifico account.

Fatto questo, il risultato del test connessione verrà visualizzato
attraverso un piccolo pop up presente nella parte bassa della pagina

Infine, una volta effettuato il salvataggio dell'Account comparirà un
ulteriore sezione "**Ecommerce**" all'interno della quale sarà possibile
decidere quali dati Ecommerce dovranno essere trasferiti dal proprio
sito alla piattaforma di ActiveCampaign (per maggiori informazioni in
merito, si veda anche quanto indicato all'interno del successivo
capitolo di questo manuale).

**ATTENZIONE!** Non è possibile, ovviamente, creare e gestire più di un
Account ActiveCampaign contemporaneamente

