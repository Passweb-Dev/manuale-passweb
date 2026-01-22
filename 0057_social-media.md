# SOCIAL MEDIA



All'interno di questa sezione è possibile configurare l'integrazione tra
il proprio sito web diverse piattaforme di terze parti (es. Facebook,
Twitter, Google, Instagram, Amazon, PayPal ecc...) al fine di consentire
agli utenti di poter effettuare la registrazione e/o l'accesso al sito
utilizzando direttamente il loro account social piuttosto che il loro
account Amazon o PayPal

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\social_web_login1.bmp](./assets/media/image208.png){width="5.811805555555556in"
height="3.545138888888889in"}

Per realizzare questo tipo di integrazione Passweb utilizza il
protocollo **Open Authorization**, ampiamente supportato dalle varie
piattaforme social e giunto alla versione 2.0 (OAuth 2.0), un protocollo
questo mediante il quale un'applicazione o un servizio web può gestire,
in modo sicuro, l'accesso autorizzato a dati sensibili come possono
essere quelli dei propri profili social.

La procedura da seguire per effettuare questa integrazione è piuttosto
semplice, si tratta, in sostanza, di creare un'apposita App all'interno
dello specifico piattaforma, prelevare le Api Key (**ConsumerKey** e
**ConsumerKeySecret**) richieste dal protocollo OAuth e inserirle nei
relativi campi dell'apposita sezione presente all'interno di questa
pagina del Wizard.

Fatto questo si tratterà poi di configurare in maniera adeguata il
Componente di Login in maniera tale da rendere disponibili agli utenti
del sito anche questa specifica possibilità di autenticazione.

Per maggiori informazioni in merito alla configurazione del componente
di Login si veda la specifica sezione "*Live Editing -- Lista Componenti
Interazione Utente -- Componenti Interni ai componenti interazione
utente -- Social Login*" di questo manuale

Di seguito verranno invece analizzate le diverse procedure da seguire
per realizzare la propria App e prelevare le relative Api Key
all'interno di ciascuna delle piattaforme attualmente gestite da
Passweb.

**ATTENZIONE!** **Per una guida sempre aggiornata relativamente alle
procedure di creazione e gestione delle App all'interno della specifica
piattaforma si consiglia comunque di fare sempre riferimento alla
relativa documentazione presente in rete.**

Va anche detto poi che i dati restituiti dalle varie piattaforme social
e utilizzati da Passweb per effettuare la registrazione automatica
dell'utente potrebbero non essere sufficienti per il completamento del
primo ordine.

Nello specifico, infatti, in questo processo di integrazione verranno
sicuramente prelevati dal profilo social dell'utente:

- il suo **Nome**

- il suo **Cognome**

- il suo Indirizzo **Email**

dati questi obbligatori e necessari a Passweb per poter creare la nuova
anagrafica utente che, ovviamente, **sarà sempre quella di un utente**
**Privato.**

Tra i dati prelevati dal profilo social potrebbe quindi non essere
presente l'indirizzo dell' utente o perché la specifica piattaforma non
consente di accedere a questo tipo di informazione o più semplicemente
perché il dato potrebbe non essere stato inserito in quanto non
obbligatorio in fase di registrazione al social.

In queste condizioni dunque non ci sarebbero problemi relativamente alla
creazione in Passweb della nuova anagrafica (dove l'indirizzo non
rappresenta effettivamente un dato obbligatorio). Nel momento in cui
però l'utente dovesse effettuare il suo primo ordine l'assenza di questo
indirizzo si farà sentire in quanto di fatto verrebbero a mancare sia
l'indirizzo di fatturazione che quello di spedizione, dati questi
obbligatori per poter andare avanti nel normale processo di checkout.
Per poter completare l'ordine l'utente dovrà quindi accedere al suo
profilo Passweb ed inserire i dati relativi all' indirizzo di
fatturazione e ad eventuali indirizzi di spedizione secondari.

