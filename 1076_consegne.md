# CONSEGNE



**ATTENZIONE! Per poter gestire le "Consegne a domicilio" è necessario
attivare il relativo modulo su Passstore**

La sezione **"Consegne",** accessibile dalla voce di menu principale
"Ordini" consente di definire e gestire le diverse tipologie di
"Consegna a domicilio" che potranno poi essere associate alle modalità
di spedizione gestite all'interno del sito.

Una volta effettuato l'accesso a questa sezione del Wizard verrà quindi
visualizzata la maschera **"Consegne"**

![](./assets/media/image372.png)

contenente l'elenco di tutte le tipologie di "Consegna a domicilio"
attualmente codificate.

**ATTENZIONE!** Ogni "Consegna" presente in elenco può differenziarsi
dalle altre in base alle proprie regole e/o all'area geografica di
applicabilità.

I pulsanti presenti nella contestuale barra degli strumenti consentono
rispettivamente di:

- **Elimina Consegna**
  (![](./assets/media/image373.png) ): consente di eliminare la tipologia di consegna a
  domicilio attualmente selezionata in elenco

- **Copia Consegna**
  (![](./assets/media/image374.png) ): consente di copiare la tipologia di
  consegna a domicilio attualmente selezionata in elenco

- **Modifica Consegna**
  (![](./assets/media/image375.png) ): consente di accedere alla maschera di
  configurazione e gestione della consegna a domicilio attualmente
  selezionata in elenco

- **Regole Preparazione**
  (![](./assets/media/image376.png) ): consente di accedere all'insieme di
  regole utili a definire quando la merce sarà pronta per essere spedita
  (per maggiori informazioni in merito si veda anche il successivo
  capitolo "*Regole di Preparazione*" di questo manuale)

- **Regole Consegna**
  (![](./assets/media/image377.png) ): consente di accedere all'insieme di regole utili
  a definire la data in cui la merce sarà consegnata (per maggiori
  informazioni in merito si veda anche il successivo capitolo "*Regole
  di Consegna*" di questo manuale)

- **Aggiungi Consegna**
  (![](./assets/media/image378.png) ): consente di creare una nuova tipologia di
  consegna a domicilio

Cliccando su quest'ultimo pulsante verrà infatti visualizzata la
maschera **"Configurazione Consegna"**

![](./assets/media/image379.png)

all'interno della quale poter impostare i parametri di configurazione
della tipologia di consegna che si intende realizzare.

In questo senso dunque il campo:

- **Nome:** consente di assegnare un nome identificativo alla consegna
  in esame in modo da poterla poi riconoscere ed identificare tra le
  altre presenti in elenco

- **Gestione Calendario:** consente di decidere se l'utente, in fase di
  acquisto, potrà selezionare la data di consegna ed, eventualmente, il
  relativo intervallo orario oppure se queste informazioni dovranno
  essere solo visualizzate senza dare però all'utente la possibilità di
  variarle.

> In particolare dunque, impostando il parametro in oggetto sul valore:

- **Si:** in questo caso (**consegna a domicilio**), in fase di ordine,
  l'utente avrà poi la possibilità di selezionare mediante appositi
  controlli il giorno e l'intervallo orario in cui desidererebbe
  ricevere la merce

![](./assets/media/image380.png)

> **ATTENZIONE!** i giorni effettivamente selezionabili all'interno del
> calendario così come i relativi intervalli orari dipenderanno da come
> sono stati impostati i parametri di configurazione della specifica
> consegna e, soprattutto, dalle regole ad essa associate (per maggiori
> informazioni in merito si veda anche il successivo capitolo "*Regole
> di consegna*" di questo manuale )

- **No:** in questo caso (**prevista consegna**), in fase di ordine,
  verrà visualizzato all'utente il primo giorno ed il primo intervallo
  orario utile in cui potrà essergli consegnata la merce senza però
  avere la possibilità di modificare queste informazioni (i campi
  relativi al giorno e all'orario saranno infatti campi in sola lettura)

![](./assets/media/image381.png)

> **ATTENZIONE!** anche in questo caso il giorno e l'intervallo orario
> visualizzati dipenderanno dal giorno e dall'orario in cui viene
> effettuato l'ordine e dalle regole associate alla consegna in esame
>
> Questa configurazione potrebbe quindi essere utilizzata non tanto per
> gestire una "consegna a domicilio" quanto più per mostrare all'utente
> quando gli verrà effettivamente consegnata la merce in relazione al
> momento in cui effettua l'ordine, alle consegne già programmate in
> quello stesso giorno piuttosto che in quella stessa fascia oraria, a
> dove dovrà essere consegnata la merce ecc...

- **Ore Preparazione:** consente di indicare il numero minimo di ore
  necessarie per preparare la merce affinché possa poi essere spedita.

> **ATTENZIONE!** Il valore indicato all'interno di questo campo andrà
> poi ad influire sugli intervalli di consegna effettivamente
> selezionabili dall'utente in fase di checkout.
>
> Supponendo dunque di indicare all'interno di questo campo il valore 0,
> ciò starà a significare che non appena ricevuto l'ordine saremo
> immediatamente pronti a spedire la merce. Non sarà quindi necessario
> del tempo aggiuntivo per preparare i relativi pacchi.
>
> Nel momento in cui invece all'interno di questo campo dovessimo
> indicare, ad esempio, il valore 2 ciò starà a significare che dal
> momento in cui abbiamo ricevuto l'ordine saranno necessarie almeno due
> ore per poter preparare il pacco e per avere quindi la merce
> effettivamente pronta per essere spedita.
>
> In conseguenza di ciò se l'utente dovesse effettuare l'ordine alle
> 14.40 e noi avessimo bisogno, come nell'esempio sopra riportato, di
> almeno due ore per preparare il pacco e avviare la consegna, allora il
> primo intervallo utile selezionabile dall'utente per farsi consegnare
> la merce non sarebbe quello dalle 15.00 alle 16.00 ma, ad esempio,
> quello dalle 16.00 alle 17.00 (in cui rientrerebbe l'orario di inizio
> consegna delle 16.40)

- **Ore Consegna:** consente di indicare il numero di ore necessarie per
  portare a termine la consegna

> **ATTENZIONE!** Il valore indicato all'interno di questo campo andrà
> poi a sommarsi alle "Ore di Preparazione" andando quindi ad influire,
> anch'esso, sugli intervalli di consegna effettivamente selezionabili
> dall'utente in fase di checkout.
>
> Supponendo dunque di lasciare vuoto il campo in esame (o di
> valorizzarlo a 0) ciò starà a significare che una volta preparata la
> merce (trascorse cioè le ore di preparazione indicate mediante il
> relativo parametro) non sarà necessario ulteriore tempo per portare a
> termine la consegna.
>
> In conseguenza di ciò se l'utente dovesse effettuare l'ordine alle
> 14.40 e, per portare a termine la consegna avessimo bisogno solamente
> di due ore per preparare il pacco (Ore Preparazione = 2 ; Ore Consegna
> = 0), allora l'orario di prevista consegna sarebbe quello delle 16.40
> e il primo intervallo orario utile e selezionabile dall'utente in fase
> di checkout potrebbe quindi essere quello che va dalle 16.00 alle
> 17.00
>
> Nel momento in cui dovessimo invece inserire, all'interno del campo in
> esame, ad esempio, il valore 3, ciò starà ad indicare che oltre al
> tempo necessario per preparare il pacco dovremo tener conto anche di
> ulteriori 3 ore per poter effettivamente portare a termine la
> consegna.
>
> In queste condizioni dunque, facendo riferimento allo stesso esempio
> precedentemente considerato, se l'utente dovesse effettuare l'ordine
> alle 14.40 dovremo considerare due ore per la preparare il pacco e per
> poterlo effettivamente spedire (16.40) più tre ulteriori ore
> necessarie per portare a termine la consegna. L'orario di prevista
> consegna sarebbe quindi quello delle 19.40 e il primo intervallo
> orario utile e selezionabile dall'utente in fase di checkout potrebbe
> quindi essere quello che va dalle 19.00 alle 20.00

- **Numero massimo di giorni:** visualizzato solo nel caso in cui il
  precedente parametro "**Gestione Calendario**" sia stato impostato sul
  valore Si.

> Consente di impostare il numero massimo di giorni, a partire dalla
> data odierna, selezionabili dall'utente sul calendario, in fase di
> scelta della data di consegna.
>
> Supponendo dunque di impostare questo parametro sul valore 7, in fase
> di checkout l'utente potrà scegliere, come giorno in cui ricevere la
> merce, uno qualsiasi dei prossimi 7 giorni utili, dove per giorni
> utili si intendono quelli in cui la consegna può effettivamente
> avvenire, in accordo con le regole per essa codificate.

- **Quota limite giornaliera:** consente di indicare il numero massimo
  di consegne gestibili in un giorno. Nel momento in cui il numero di
  consegne "prenotate", e quindi previste, per un dato giorno dovesse
  raggiungere il numero indicato in corrispondenza di questo parametro,
  non sarà più possibile selezionare questo stesso giorno per ulteriori
  consegne

> **ATTENZIONE!** Nel momento in cui il parametro in esame dovesse
> essere lasciato vuoto non verrà imposto alcun limite relativamente al
> numero di consegne effettuabili in un giorno

All'interno della sezione "**Spedizioni**" è possibile indicare i metodi
di spedizione cui associare la "Consegna a domicilio" che si sta
codificando.

![](./assets/media/image382.png)

Nel box di sinistra sono indicati tutti i metodi di trasporto
attualmente codificati all'interno della corrispondente sezione del
Wizard. Per ciascuno di essi è riportato, tra parentesi, l'id del
relativo metodo di trasporto e la descrizione ad esso assegnata.

Per assegnare la consegna in esame ad una data modalità di spedizione
sarà sufficiente selezionarla dal box di sinistra ed inserirla in quello
di destra cliccando sul pulsante raffigurante una piccola freccia
rivolta verso destra.

