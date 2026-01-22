# CAMPO CHECKBOX



Inserendo il componente "**Campo Checkbox**" all'interno del form di
Registrazione presente nel modulo di One Step Checkout, verrà aperta la
sua maschera di gestione e configurazione, dove troveremo, tra gli
altri, anche il campo "**Tipo di dato di Destinazione**" che ci
consentirà di specificare esattamente come dovrà essere utilizzato il
campo in esame all'interno del form

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\one_step_checkout_res_5.bmp](./assets/media/image305.png){width="4.607638888888889in"
height="2.938888888888889in"}

**Tipo di dato di Destinazione**: consente di specificare la modalità di
utilizzo del relativo check box che verrà inserito all'interno del form
di informazioni utente.

E' possibile selezionare una delle seguenti opzioni:

**Attributo Cliente:** selezionando questa opzione il componente in
esame manterrà il suo funzionamento classico limitandosi quindi a
memorizzare, all'interno dello specifico attributo indicato nel
successivo campo "**Attributo di Destinazione**", il fatto che l'utente
abbia selezionato o meno il relativo check.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\one_step_checkout_res_6.bmp](./assets/media/image306.png){width="4.601388888888889in"
height="2.938888888888889in"}

**Campo Cliente:** selezionando questa opzione sarà poi possibile
indicare all'interno del successivo parametro "**Campo di
Destinazione**" quello che dovrà essere l'effettivo funzionamento del
check box.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\one_step_checkout_res_7.bmp](./assets/media/image307.png){width="4.601388888888889in"
height="2.926388888888889in"}

In particolare nel momento in cui il parametro "**Campo di
Destinazione**" dovesse essere impostato sul valore:

- **Stesso Indirizzo per la Spedizione:** il componente check box verrà
  utilizzato per consentire all'utente di decidere, direttamente in fase
  di checkout, se utilizzare o meno gli stessi dati per l'indirizzo di
  fatturazione e per quello di spedizione.

> In questo caso all'interno del form di Registrazione dovranno dunque
> essere inseriti, necessariamente, i seguenti campi:

- **Indirizzo, Località, Provincia, Nazione e CAP**, mappati come noto
  con i relativi campi dell'Anagrafica Utente gestionale e utilizzati
  per definire l'**Indirizzo di Fatturazione**

- **Indirizzo n.2 (o n.3 / n.4), Località n.2 (o n.3 / n.4), Provincia
  n.2 (o n.3 / n.4), Nazione n.2 (o n.3 / n.4), CAP n.2 (o n.3 / n.4) e
  Nominativo n.2 (o n.3 / n.4)**, mappati come noto con i relativi campi
  dell' Anagrafica Indirizzi di spedizione, e utilizzati dunque per
  definire uno specifico **Indirizzo di Spedizione Merce**

> Nelle condizioni in esame, all'interno del form di informazioni
> utente, il check box così configurato **sarà selezionato a default** e
> i campi utilizzati per definire l'eventuale indirizzo di spedizione
> merce verranno nascosti (tipicamente dunque la label utilizzata per
> questo componente dovrebbe essere del tipo "**Utilizza lo stesso
> indirizzo per la spedizione**")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\one_step_checkout_res_8.bmp](./assets/media/image308.png){width="4.98125in"
height="2.7916666666666665in"}

> **ATTENZIONE!** **A default dunque verranno utilizzati gli stessi dati
> sia per l'indirizzo di spedizione che per quello di fatturazione**
>
> Nel momento in cui l'utente volesse utilizzare invece un diverso
> indirizzo di spedizione sarà sufficiente deselezionare il campo in
> esame. In questo modo verranno automaticamente visualizzati i campi
> Indirizzo n.2 (o n.3 / n.4), Località n.2 (o n.3 / n.4), Provincia n.2
> (o n.3 / n.4), Nazione n.2 (o n.3 / n.4), CAP n.2 (o n.3 / n.4) e
> Nominativo n.2 (o n.3 / n.4), che, come detto dovranno per forza di
> cose essere gestiti all'interno del form, e che l'utente potrà ora
> utilizzare per indicare un indirizzo di spedizione merce diverso da
> quello di fatturazione

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\one_step_checkout_res_9.bmp](./assets/media/image309.png){width="4.98125in"
height="2.7916666666666665in"}

> **ATTENZIONE!** Nel caso in cui l'esigenza dovesse essere quella di
> consentire all'utente di decidere, direttamente in fase di checkout se
> utilizzare o meno gli stessi dati per l'indirizzo di fatturazione e
> per quello di spedizione sarebbe possibile utilizzare anche il
> componente "Campo Radio" (per maggiori informazioni in merito si veda
> anche il successivo capitolo di questo manuale)
>
> **ATTENZIONE!** nel caso in cui siano attive determinate funzionalità
> (gestione iva oss, promozioni basate su determinate zone di spedizione
> ...) il cambiamento dell'indirizzo di spedizione potrebbe anche
> comportare dei cambiamento nei totali del documento

- **Crea Account**: il componente check box verrà utilizzato per
  consentire all'utente di decidere, direttamente in fase di checkout,
  se creare un Account per futuri accessi al sito o se proseguire in
  modalità guest completando quindi l'ordine come ospite senza creare
  nessun account.

> In questo caso all'interno del form di Registrazione dovranno dunque
> essere inseriti, necessariamente, anche i campi: **Username** e
> **Password**
>
> Nelle condizioni in esame, all'interno del form di informazioni
> utente, il check box così configurato **a default risulterà essere
> deselezionato** e i campi utilizzati per definire l'eventuale account
> (ossia Username, Password e Conferma Password) verranno nascosti.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\one_step_checkout_res_10.bmp](./assets/media/image310.png){width="4.98125in"
height="2.7916666666666665in"}

> **ATTENZIONE!** **a default il modulo di One Step checkout è
> configurato per realizzare acquisiti in modalità Guest senza creare
> quindi alcun account di accesso al sito**
>
> Nel momento in cui l'utente volesse invece creare, contestualmente
> all'inserimento dell'ordine, anche un nuovo account sarà sufficiente
> selezionare il check in esame. In questo modo infatti i campi Username
> e Password che, come detto dovranno per forza di cose essere gestiti
> all'interno del form, verranno automaticamente visualizzati e l'utente
> potrà utilizzarli per creare il proprio account di accesso al sito.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\one_step_checkout_res_11.bmp](./assets/media/image311.png){width="4.98125in"
height="2.7916666666666665in"}

