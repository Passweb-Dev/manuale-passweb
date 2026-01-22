# FASE 1 -- SELEZIONE DEL CENTRO DI PRODUZIONE



In questa prima fase l'utente avrà la possibilità di selezionare lo
specifico **Centro di Produzione** (Spiaggia, Gestione Cabine ...) **su
cui effettuare poi la prenotazione**.

All'interno del Tab "**Centri**" verrà quindi visualizzata una lista di
Radio Button in cui ogni opzione corrisponderà ad un ben determinato
Centro di Produzione opportunamente codificato all'interno del
gestionale

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\spiagge_configurazione_9.bmp](./assets/media/image377.png){width="5.220833333333333in"
height="3.8652777777777776in"}

Per fare in modo che un Centro di Produzione possa essere visualizzato
all'interno di questa lista, abilitando quindi la prenotazione via web
delle relative risorse, sarà necessario:

- Definire ed associare al Centro di Produzione una specifica piantina

- Abilitare il Centro di Produzione per essere esportato e gestito
  all'interno del sito selezionando, in questo senso, il parametro
  "**Abilita Passweb**" presente all'interno della sezione "**Opzione
  Risorse**" nella maschera di configurazione del Centro di Produzione

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\spiagge_configurazione_1.bmp](./assets/media/image378.png){width="5.441666666666666in"
height="3.779166666666667in"}

- Definire l'intervallo temporale entro cui il Centro di Produzione
  potrà effettivamente essere disponibile consentendo quindi la
  prenotazione delle risorse ad esso associate.

> Sarà quindi necessario impostare una data di inizio e fine
> disponibilità agendo mediante i relativi campi presenti, anche in
> questo caso, all'interno della sezione "**Opzione Risorse**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\spiagge_configurazione_2.bmp](./assets/media/image379.png){width="5.441666666666666in"
height="3.779166666666667in"}

> **ATTENZIONE! le date di inizio e fine disponibilità evidenziate in
> figura condizioneranno poi, nel successivo step, i giorni
> effettivamente selezionabili per la prenotazione**
>
> Facendo riferimento alla situazione evidenziata il figura, lato web,
> l'utente avrà quindi la possibilità, in relazione al Centro di
> Produzione in esame, di effettuare delle prenotazioni esclusivamente
> per il periodo che va dal 01/05/2021 al 30/09/2021

Per maggiori informazioni relativamente a come codificare e gestire i
centri di produzione (con le relative piantine) all'interno di Plan si
rimanda alla specifica documentazione di prodotto.

**ATTENZIONE!** **Nel caso in cui si sia deciso di codificare e gestire
via web un solo Centro di Produzione il tab "Centri" non verrà
visualizzato e il processo di prenotazione inizierà direttamente dalla
fase 2 con la selezione delle date**

