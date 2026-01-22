# GIFT CARD HO.RE.CA.



Come già evidenziato all'interno dei precedenti capitoli di questo
manuale, le Gift Card di tipo Ho.Re.Ca. sono disponibili soltanto per i
siti Ecommerce collegati al gestionale Beauty e verranno utilizzate per
gestire l'acquisto di Voucher (Buoni Regalo) che, all'interno deli sito,
potranno poi essere spesi solo ed esclusivamente in fase di prenotazione
/ pagamento di uno o più trattamenti.

**ATTENZIONE!** **Le Gift Card di tipo Ho.Re.Ca. possono essere
utilizzate solo per la prenotazione di Trattamenti**. Nel caso in cui
l'esigenza dovesse essere quella di gestire delle carte regalo per
l'acquisto di prodotti sarà necessario ricorrere alle Gift Card Fisiche
e/o Virtuali

In conseguenza di ciò la gestione di questa particolare tipologia di
carte regalo è leggermente diversa rispetto a quella analizzata per le
Gift Card Fisiche o Virtuali.

Nello specifico il processo di creazione e gestione di una Gift Card di
tipo Ho.Re.Ca. dovrà passare attraverso i seguenti step:

1.  Codifica all'interno del wizard di passweb della gift card di tipo
    Ho.Re.Ca.

2.  Esportazione all'interno del sito di Trattamenti e/o articoli di
    tipo "Ricarica Promozione"

3.  Acquisto della Gift Card (Trattamento o Ricarica Promozione) sul
    front end del sito

4.  Utilizzo del Buono Sconto Beauty generato a seguito dell'acquisto di
    una Gift Card HoReCa

Ovviamente poi, affinché tutto il processo possa funzionare in maniera
corretta, anche il gestionale Beauty dovrà essere configurato in un
certo modo.

In questo senso dunque, considerando che la gestione delle Gift Card di
tipo HoReCa determina la creazione in Beauty, a fronte della ricezione
di determinati ordini web, di nuovi Buoni Sconto e che, volendo, tali
Buoni Sconto potrebbero anche consentire l'acquisto di più trattamenti
in momenti diversi sarà necessario:

- Abilitare in maniera corretta, **nella configurazione della Replica
  Dati del gestionale, il canale relativo ai "Buoni Sconto"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\replica_dati_beauty_buono_sconto.bmp](./assets/media/image331.png){width="5.188194444444444in"
height="3.1104166666666666in"}

- Impostare in maniera adeguata il formato dei Codici a barre da
  utilizzare per la generazione dei Buoni Sconto

> In questo senso sarà quindi necessario portarsi all'interno all'
> interno della sezione "**Articoli -- Codice a barre**" e definire il
> formato del codice da utilizzare impostando il campo "Predefinito per"
> sull\'opzione "Buono Sconto", come nella figura di seguito riportata

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\beauty_codici_a_barre.bmp](./assets/media/image332.png){width="5.279166666666667in"
height="4.0256944444444445in"}

- Portarsi in "**Configurazione -- Opzioni Installazione**" e
  selezionare il check "**Non azzerare il progressivo del buono
  sconto**" presente all'interno del tab "**Avanzate**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\beauty_configurazione_buoni_sconto.bmp](./assets/media/image333.png){width="6.272916666666666in"
height="4.0256944444444445in"}

- Infine, restando sempre in "**Configurazione -- Opzioni
  Installazione**" sarà necessario flaggare anche il parametro
  "**Utilizzo parziale buoni sconto**" presente all'intero del tab
  "**Buoni e caparre**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\beauty_configurazione_buoni_sconto_2.bmp](./assets/media/image334.png){width="6.272916666666666in"
height="4.0256944444444445in"}

