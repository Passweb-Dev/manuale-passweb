# NOTIFICHE DISPONIBILITA'



L'integrazione tra Passweb e MailChimp può essere sfruttata non solo per
la realizzazione di un sistema di invio Newsletter, ma anche per creare
e gestire un sistema di notifiche mail automatico mediante il quale
poter avvisare gli utenti del sito, che ne hanno fatto esplicita
richiesta, relativamente ad un prodotto che è tornato ad essere
disponibile e quindi nuovamente acquistabile all'interno del nostro
sito.

In questo senso tutti i concetti di base relativamente alle
configurazioni di MailChimp, alla creazione e gestione di liste,
template e campagne analizzati in merito al sistema di gestione delle
Newsletter, continuano ovviamente ad essere perfettamente validi.

> **NOTA BENE**: per maggiori informazioni in merito alla gestione in
> MailChimp e/o in Passweb di liste, template e campagne si vedano i
> precedenti capitoli di questo manuale

In sostanza dunque per mettere in piedi questo sistema automatico di
notifiche si tratterà semplicemente di creare appositi **Template di
tipo Ecommerce** e **Campagne di tipo "Disponibilità Articolo"**, oltre
ovviamente al fatto di dover inserire all'interno del proprio sito il
componente "**Notifica Disponibilità**" e di gestire la vendita di
articoli sulla base delle disponibilità memorizzate in Passweb e
aggiornate quindi all'ultima sincronizzazione utile.

Di seguito vengono indicati in maniera puntuale i vari passi da
effettuare per abilitare e configurare correttamente il sistema di
Notifiche relative alla disponibilità dei prodotti venduti all'interno
del proprio sito Ecommerce.

1.  Creare un account MailChimp prelevando l'apposita API Key da
    inserire nel relativo campo della sezione "*Sito -- Preferenze*" del
    Wizard di Passweb in maniera tale da poter realizzare l'integrazione
    tra i due sistemi.

![](./assets/media/image94.png)

2.  Impostare la modalità di acquisto degli articoli in catalogo in
    maniera tale che questi stessi articoli possano effettivamente
    essere acquistati solo ed esclusivamente **nel caso in cui la loro
    disponibilità (in Passweb)** sia effettivamente maggiore di zero.

> Per questo è necessario impostare il parametro "**Gestione Acquisto**"
> presente all'interno della sezione "*Catalogo -- Configurazione
> Parametri Catalogo -- Catalogo Mexal/Ho.Re.Ca.*" del Wizard sul valore
> **"Acquista solo se disponibile"**

![](./assets/media/image95.png)

> **ATTENZIONE!** Nel momento in cui questo parametro dovesse essere
> impostato sul valore "Acquista Sempre" gli articoli presenti in
> catalogo sarebbero sempre acquistabili indipendentemente da quella che
> sarà la loro effettiva disponibilità. In queste condizioni ovviamente
> non avrebbe senso richiedere la notifica di disponibilità del
> prodotto. Per maggiori informazioni in merito si veda anche la sezione
> "*Catalogo -- Configurazione Parametri Catalogo -- Catalogo Mexal /
> Ho.Re.Ca."* di questo manuale.

3.  Impostare il parametro "**Gestione Notifica Disponibilità**"
    presente all'interno della sezione "*Catalogo -- Configurazione
    Parametri Catalogo -- Catalogo Mexal / Ho.Re.Ca.*" del Wizard sul
    valore **"Ai soli utenti registrati"** oppure sul valore **"A
    tutti"**

![](./assets/media/image96.png)

> **ATTENZIONE!** Nel caso in cui tale parametro dovesse essere
> impostato sul valore **"No"** il componente "**Notifica
> Disponibilità**" non verrà attivato e non sarà quindi possibile
> abilitare il sistema di gestione delle notifiche.

![](./assets/media/image97.png)

> Ovviamente il fatto di impostare questo parametro sul valore "A tutti"
> oppure "Ai soli utenti registrati" determinerà un diverso
> comportamento per il componente "Notifica Disponibilità". Per maggiori
> informazioni in merito si veda anche la sezione "*Catalogo --
> Configurazione Parametri Catalogo -- Catalogo Mexal / Ho.Re.Ca."* di
> questo manuale

4.  Inserire il Componente "**Notifica Disponibilità**" all'interno di
    uno dei Componenti consentiti (es. Scheda Prodotto, Catalogo
    Ecommerce ecc...), configurandolo in maniera corretta

![](./assets/media/image98.png)

> Per maggiori informazioni relativamente alla configurazione e alla
> gestione del componente "Notifica Disponibilità" si veda anche la
> sezione *"Live Editing -- Lista Componenti Ecommerce -- Componenti
> interni ai Componenti Ecommerce -- Componente Notifica Disponibilità"*
> di questo manuale

5.  Realizzare in MailChimp un apposito Template che dovrà essere poi
    utilizzato nella costruzione delle mail di notifiche di "prodotto
    nuovamente disponibile"

> Per maggiori informazioni relativamente alla creazione di template in
> MailChimp si veda anche la sezione "*MailChimp -- Gestione ed utilizzo
> dei template*" di questo manuale

6.  Sincronizzare Passweb e MailChimp in maniera tale da rendere
    disponibile anche all'interno di Passweb il template creato al passo
    precedente

7.  Configurare il template appena importato in Passweb in maniera tale
    che risulti essere un **template di tipo Ecommerce**

![](./assets/media/image99.png)

> Per maggiori informazioni relativamente alla gestione e configurazione
> dei template in Passweb si veda anche la sezione "*MailChimp --
> Newsletter Passweb e MailChimp -- Gestione Newsletter -- Template*" di
> questo manuale.

8.  Creare in MailChimp un'apposita Lista all'interno della quale
    verranno poi inseriti tutti gli utenti del sito che hanno
    espressamente richiesto di essere avvisati nel momento in cui
    determinati articoli dovessero tornare disponibili.

> **ATTENZIONE!** I vari utenti verranno inseriti all'interno di questa
> lista solo ed esclusivamente nel momento in cui gli dovrà essere
> effettivamente inviata la mail di notifica.
>
> Per ogni utente verrà memorizzato in MailChimp il solo indirizzo mail
> e la lingua del sito in cui si è registrato al sistema di notifiche in
> maniera tale da potergli poi inviare la mail nella lingua corretta.
>
> Tali utenti verranno inoltre automaticamente rimossi non appena
> inviata la campagna e consegnate le relative mail di notifica (questo
> per garantire che il numero di utenti registrati in MailChimp non
> diventi eccessivo, soprattutto in considerazione del fatto che dal
> numero di iscritti può dipendere il fatto di dover passare ad un
> account MailChimp a pagamento).
>
> Per maggiori informazioni relativamente alla creazione e alla gestione
> delle liste di iscritti in MailChimp si veda anche il capitolo
> "*MailChimp -- Newsletter Passweb e MailChimp -- Gestione Newsletter
> -- Liste*" di questo manuale

9.  Creare in Passweb una Campagna di tipo **"Disponibilità Articolo"**
    selezionando per essa il Template configurato al punto 7

![](./assets/media/image100.png)

> Per maggiori informazioni relativamente alla creazione di Campagne in
> Passweb si veda anche la sezione "*MailChimp -- Newsletter Passweb e
> MailChimp -- Gestione Newsletter -- Campagne*" di questo manuale.

10. Gestire, per la Campagna creata al punto precedente, **un invio per
    ciascuna delle lingue presenti all'interno del sito**.

> Per poter effettuare quest'ultima operazione sarà necessario portarsi
> per prima cosa all'interno della sezione "Sito -- Gestione Newsletter
> -- Campagne" del Wizard, selezionare la Campagna creata al punto 9 e
> cliccare sul pulsante "**Gestisci invii per la Campagna**" (
> ![Videate\\pulsante_gestisci_invii_campagna.bmp](./assets/media/image101.png) ) presente nella barra degli strumenti
>
> Nella successiva maschera verranno visualizzati gli invii già
> codificati per la Campagna in esame. Per gestire un nuovo invio sarà
> quindi necessario cliccare sul pulsante "**Nuovo Invio Campagna
> Disponibilità**" (
> ![](./assets/media/image102.png) ): presente nella barra degli
> strumenti e inserire tutti i parametri necessari per la configurazione
> dell'invio.

![](./assets/media/image103.png)

> Nello specifico sarà necessario indicare:

- **Nome della Campagna in Uscita:** nome identificativo per l'invio che
  si sta codificando

- **Oggetto della Campagna:** oggetto che dovrà essere utilizzato nelle
  mail inviate dalla campagna in esame

- **Indirizzo del mittente:** indirizzo mail che dovrà essere utilizzato
  come indirizzo del mittente nelle mail inviate dalla campagna in esame

- **Nome del Mittente:** nome del mittente che verrà associato
  all'indirizzo indicato nel campo precedente e che conseguentemente
  verrà visualizzato nei vari client di posta all'interno del campo "Da"

- **Nome del destinatario:** nome identificativo per i destinatari delle
  mail inviate dalla campagna in esame (es. "Richiesta disponibilità
  Articoli"). Tale nome verrà poi visualizzato nei vari client di posta
  all'interno del campo "A"

- **Attivo:** consente di marcare come Attivo l'invio che si sta
  codificando.

> Nel momento in cui dovranno essere effettivamente inviate le mail di
> notifica **verranno considerati solo ed esclusivamente gli Invii
> codificati per Campagne di tipo "Disponibilità Articolo" marcati come
> Attivi**

- **Lista a cui inviare la Campagna:** consente di selezionare la
  specifica lista di iscritti cui dovrà essere inviata la mail di
  notifica. Andrà ovviamente selezionata, tra quelle proposte, la lista
  creata al punto

- **Lingua della Campagna:** consente di associare lo specifico Invio ad
  una delle lingue gestite all'interno del sito. Necessaria per poter
  inviare agli utenti del sito la mail di notifica nella lingua
  corretta.

> Nel caso in cui il sito sia Multilingua sarà quindi necessario
> codificare un Invio per ciascuna delle lingue gestite
>
> **ATTENZIONE!** Nel caso in cui si dovesse configurare un solo invio
> per la lingua italiana, pur avendo il sito in multilingua, eventuali
> utenti che hanno richiesto la notifica di disponibilità prodotti
> visitando il sito in lingua estera non riceveranno mai tale notifica.
>
> **NOTA BENE**: è possibile attivare un solo invio per lingua. Nel caso
> in cui si dovesse selezionare il parametro Attivo per un invio
> associato ad un determinata lingua verranno quindi automaticamente
> disattivati eventuali altri invii codificati per la stessa lingua.

- **Versione Testuale (campo non obbligatorio):** consente di impostare
  una versione testuale per la mail di notifica. La versione testuale
  verrà visualizzata solo ed esclusivamente da quei client di posta che
  non risultino avere abilitata la visualizzazione delle mail ricevute
  in formato HTML

- **Template Newsletter:** all'interno di questa sezione sarà possibile
  impostare, in maniera definitiva, i contenuti della mail di notifica.

> In questo senso dunque, verrà visualizzato il Template selezionato al
> punto 9 e, per esso, sarà possibile impostare in maniera definitiva i
> soli contenuti delle sezioni che, in fase di configurazione del
> template, sono state impostate per accettare dei contenuti
> personalizzati (e non mappate dunque con eventuali campi articolo)
>
> **ATTENZIONE!** **A differenza degli Invii associati a Campagne
> Semplici o CMS, esaminate nei precedenti capitoli di questo manuale,
> in questo caso non sarà possibile schedulare l'invio delle mail ne
> tanto meno scegliere di inviarle immediatamente.**
>
> L'effettiva creazione della Campagna in MailChimp e il conseguente
> invio delle Mail di notifica avverrà infatti in maniera completamente
> automatica nel momento in cui a seguito di una sincronizzazione Sito
> -- Gestionale, e del conseguente aggiornamento delle disponibilità
> memorizzate in Passweb, alcuni prodotti fino a quel momento a
> disponibilità minore o uguale a zero tornino ad avere una
> disponibilità maggiore di zero e ad essere quindi nuovamente
> acquistabili all'interno del sito.

