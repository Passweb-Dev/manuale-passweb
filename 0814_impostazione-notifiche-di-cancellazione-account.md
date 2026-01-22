# IMPOSTAZIONE NOTIFICHE DI CANCELLAZIONE ACCOUNT



A partire da Settembre 2021 eBay offre ai propri utenti un modo per
richiedere che i propri dati personali vengano eliminati dai sistemi di
eBay, nonché dai sistemi di tutti i partner eBay che
archiviano/visualizzano questi dati personali, inclusi sviluppatori di
terze parti.

**ATTENZIONE! A seguito di ciò diventa dunque obbligatorio configurare
il proprio developer account in maniera tale da abilitare tale
funzionalità**

Di seguito viene descritta la procedura per poter effettuare quanto
richiesto da eBay:

1.  Accedere al proprio developer account

2.  Portarsi all'interno della sezione "**Application Keys**" e cliccare
    sul pulsante "**Notification**" relativo alle chiavi dell'ambiente
    di produzione

![](./assets/media/image17.png)

3.  Nella sezione "**Alert & Notification**", selezionare l'opzione
    "**Marketplace Account Deletion**"

![](./assets/media/image18.png)

4.  Compilare poi i restanti campi della maschera come di seguito
    indicato:

    - **Not persisting eBay data**: lasciare deselezionato

    - **Email to notify if marketplace account deletion notification
      endpoint is down:** inserire un indirizzo mail cui verranno
      notificati eventuali stati di down dell'endpoint utilizzato da
      eBay per gestire questo tipo di notifiche

    - **Marketplace account deletion notification endpoint:** inserire
      il seguente indirizzo

> **https://\<url_sito\>/AccountDeletionEBay**
>
> dove al posto di \<url_sito\> andrà inserito, ovviamente, l'indirizzo
> del proprio sito web

- **Verification token:** inserire la stringa indicata di seguito

> **Vowop1bA4IZqLJck-Amj6q8R_YvVTH1nqhjQPmoLtDPhwuSqq89Q6INTTpQwzuMLDN-V3_tI20CVlDwm**

5.  Dopo aver impostato l' url dell\'endpoint di notifica e il valore
    del token di verifica, cliccare sul pulsante Salva.

> In questo modo si attiverà anche il processo di convalida, con il
> primo passaggio da parte di eBay che invia un codice di verifica
> all'endpoint. Se l'endpoint risponde correttamente al codice challenge
> di eBay, l' url dell'endpoint di notifica e il valore del token di
> verifica verranno salvati correttamente.

Una volta completato con successo il processo di iscrizione alle
notifiche di cancellazione/chiusura dell\'account del marketplace eBay,
è possibile inviare una notifica di prova cliccando per questo sul
pulsante "**Send Test Notification**".

