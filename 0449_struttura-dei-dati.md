# STRUTTURA DEI DATI



Per comprendere in maniera un po' più dettagliata quello che avviene
durante i diversi step del processo di prenotazione è necessario fare
alcune considerazioni sulla struttura dati da creare all'interno del
gestionale

**ATTENZIONE! Per informazioni più dettagliate su come configurare e
gestire i dati sul gestionale in relazione a questo tipo di prenotazioni
si consiglia comunque di fare sempre riferimento alla specifica
documentazione di prodotto.**

Per avere una situazione più chiara supponiamo di dover gestire il
classico esempio della prenotazione di un ombrellone con la possibilità
di indicare anche il numero di lettini e / o di sdraio da aggiungere.

Per soddisfare questo tipo di esigenza sarà necessario ricorrere, in
Plan, all'utilizzo degli articoli strutturati associando ai relativi
prototipi specifiche tipologie di risorse e posizionando poi queste
stesse risorse su di una piantina grafica associata al centro di
produzione utilizzato per gestire la spiaggia.

Supponendo di avere a che fare con una spiaggia divisa in 4 distinti
settori potremmo pensare di creare 4 diversi tipi di risorsa, uno per
ciascun settore:

- OmbreS1 (ombrelloni del settore 1)

- OmbreS2 (ombrelloni del settore 2)

- OmbreS3 (ombrelloni del settore 3)

- OmbreS4 (ombrelloni del settore 4)

![Videate\\spiagge_configurazione_3.bmp](./assets/media/image372.png)

Il "**Tipo Risorsa**" identifica quindi il settore della spiaggia in cui
si troverà il singolo ombrellone.

Il passo successivo sarà quello di definire la struttura e i relativi
insiemi di valori che permetteranno all'utente di impostare le diverse
opzioni della sua prenotazione (numero di lettini, numero di sedie ...)
compreso anche i giorni in cui intende prenotare.

In questo senso, la tipica struttura cui fare riferimento potrebbe
essere quella indicata in tabella

  -------------------------------------------------------------------------------
  **Campo**     **Valori**          **Esempio di        **Note**
                                    valori**            
  ------------- ------------------- ------------------- -------------------------
  **Tipo**      Articolo            OS1, OS2, OS3, OS4  Campo radice
                identificativo                          
                della risorsa e del                     
                settore di                              
                riferimento                             

  **Durata**    Numero di giorni    1,3,7,14,30,60,90   Campo primario con flag
                della prenotazione  ...                 "Durata Servizio"
                                                        selezionato sul
                                                        corrispondente insieme di
                                                        valori

  **Lettini**   Prima variante      1,2,3 ...           Campo primario con valori
                                                        coerenti con il numero di
                                                        lettini da poter
                                                        aggiungere ad ogni
                                                        ombrellone

  **Sedie**     Seconda Variante    1,2,3 ...           Campo primario con valori
                                                        coerenti con il numero di
                                                        lettini da poter
                                                        aggiungere ad ogni
                                                        ombrellone
  -------------------------------------------------------------------------------

- Il primo livello della struttura sarà quello utilizzato come campo
  radice per i relativi prototipi. I valori di questo livello dovranno
  quindi essere i codici di articoli prototipo che possano identificare
  il tipo di risorsa e il relativo settore di riferimento (settore della
  spiaggia, fila di ombrelloni ...). Supponendo dunque di identificate
  con la lettera "**O = Ombrellone**" il tipo di risorsa e con **S1, S2
  ...** i vari settori della spiaggia, dovremo poi andare a codificare
  un prototipo appartenente alla struttura in esame con codice OS1 per
  identificare gli ombrelloni posizionati nel Settore 1, un prototipo
  con codice OS2 per identificare quelli posizionati nel settore 2 e
  così di seguito

- Il secondo livello della struttura verrà invece utilizzato per gestire
  i giorni della prenotazione. I valori da poter inserire all'interno di
  questo livello dovranno quindi rappresentare il numero di giorni per
  cui l'utente potrà prenotare uno degli ombrelloni della spiaggia

> **ATTENZIONE! In fase di creazione della struttura è di fondamentale
> importanza individuare, tra i diversi livelli, quello che dovrà essere
> utilizzato per gestire la durata della prenotazione**.
>
> Una volta definito tale livello sarà quindi necessario marcare il
> corrispondente "Insieme di Valori" utilizzando l'apposito parametro
> "**Durata Servizio**" presente nella maschera di definizione di questo
> stesso "Insieme di Valori"

![Videate\\spiagge_configurazione_4.bmp](./assets/media/image373.png)

- Il terzo e il quarto livello della struttura verranno invece
  utilizzati per consentire all'utente di indicare il numero,
  rispettivamente di lettini e di sedie da poter aggiungere al proprio
  ombrellone. I valori da poter inserire all'interno di questo livello
  dovranno quindi essere coerenti con il numero di lettini / sedi che
  potrebbero effettivamente essere aggiunti ad un singolo ombrellone

Una volta costruita la struttura e definiti i corrispondenti insiemi di
valori il passo successivo sarà quello di andare a codificare gli
articoli prototipo (OS1, OS2, OS3, OS4) che dovranno essere utilizzati
per identificare gli ombrelloni posizionati nei diversi settori della
spiaggia.

**ATTENZIONE!** Ogni articolo prototipo dovrà essere associato al
corrispondente "Tipo Risorsa" utilizzando in questo senso la scheda
"**Risorse**" presente nell'anagrafica gestionale dell'articolo stesso

![Videate\\spiagge_configurazione_5.bmp](./assets/media/image374.png)

Il prototipo OS1 dovrà quindi essere associato al Tipo Risorsa
"OmbreS1", il prototipo OS2 al Tipo Risorsa "OmbreS2" ecc...

Infine, per consentire la prenotazione giornaliera delle relative
risorse, sarà necessario selezionare anche il parametro
"**giornaliero**" evidenziato in figura

In questa fase poi sarà necessario generare anche tutti gli articoli
figlio identificativi delle diverse possibili combinazioni (ombrellone +
lettini + sedie) che potranno effettivamente essere gestite.

**ATTENZIONE!** **Il fatto di esportare all'interno del sito i soli
articoli prototipo o anche tutti i relativi articoli figlio determinerà
la possibilità di impostare o meno, in Passweb, la gestione della
struttura come vincolata al precedente livello**.

In sostanza nel momento in cui dovessero essere esportati sul sito:

- i soli articoli prototipo, la relativa struttura Passweb dovrà essere
  impostata come "**Esplosa completamente**". In queste condizioni
  l'utente avrà la possibilità di selezionare una qualsiasi combinazione
  di lettini + ombrelloni. Se poi la combinazione indicata non dovesse
  corrispondere a nessuna di quelle effettivamente gestite (e quindi a
  nessuno degli articoli figlio codificati all'interno del gestionale)
  verrà visualizzato sul sito un apposito messaggio di errore

- gli articoli prototipo più tutti i relativi articoli figlio, la
  struttura Passweb potrebbe anche essere impostata come "**Vincolata al
  precedente livello**". In queste condizioni l'utente avrebbe quindi la
  possibilità di selezionare solo ed esclusivamente una delle
  combinazioni "lettino + ombrelloni + sedie" effettivamente gestite e
  corrispondente quindi ad uno degli articoli figlio codificati
  all'interno del gestionale

Arrivati a questo punto, dopo aver codificato la struttura e tutti gli
articoli necessari per gestire le prenotazioni l'ultimo passo sarà
quello di andare a creare il Centro di Produzione da utilizzare per
gestire la spiaggia.

Dovremo quindi creare la cartina della spiaggia (suddivisa in 4 settori)
in cui andare poi a posizionare e a configurare le varie risorse ossia i
singoli ombrelloni

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\spiagge_configurazione_7.bmp](./assets/media/image375.png)

**ATTENZIONE! Ogni risorsa, quindi ogni ombrellone, dovrà essere
associato al "Tipo Risorsa" corrispondente al settore in cui verrà
posizionato e all'articolo prototipo utilizzato per gestire e
identificare gli ombrelloni di quello stesso settore.**

Supponendo dunque di fare riferimento **agli ombrelloni del Settore 1**,
l'anagrafica delle relative risorse dovrà essere del tipo di quella
indicata in figura

![Videate\\spiagge_configurazione_6.bmp](./assets/media/image376.png)

- **Nome** = identificativo della risorsa

- **Tipo Risorsa** = OmbreS1

- **Predefinito** = OS1

