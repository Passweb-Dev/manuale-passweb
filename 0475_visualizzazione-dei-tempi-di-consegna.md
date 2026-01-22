# VISUALIZZAZIONE DEI TEMPI DI CONSEGNA



Nel momento in cui l'esigenza dovesse essere quella di utilizzare il
componente "Spedizione" per visualizzare una data di prevista consegna
per i singoli prodotti presenti all'interno di Componenti Ecommerce di
primo livello quali la Scheda Prodotto, il Catalogo Ecommerce, gli
Abbinati ... sarà necessario:

- Selezionare il parametro "**Abilita stima costi/consegna**" presente
  nella maschera di configurazione del metodo di trasporto in relazione
  al quale si vuol visualizzare una data di prevista consegna

> **ATTENZIONE!** Il componente "Spedizione" prenderà in considerazione
> solo ed esclusivamente i metodi di trasporto per i quali è stato
> flaggato il parametro "**Abilita stima costi/consegna**"
>
> **ATTENZIONE!** Per poter visualizzare il parametro "**Abilita stima
> costi/consegna**" è necessario attivare, su Passstore, il modulo
> "Stima Trasporto"

- Verificare di aver attivato e configurato correttamente (in relazione
  alle specifiche esigenze del caso) il modulo (gratuito) **"Consegne a
  Domicilio"**

> **ATTENZIONE!** L'attivazione del modulo "Consegne a Domicilio" è
> indispensabile per la visualizzazione della data di prevista consegna.

- Verificare di aver inserito all'interno del campo "**Template
  Spedizione**", presente nella maschera di configurazione del
  componente "Spedizione", il segnaposto "**Data**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\spedizione_segnaposto_data.bmp](./assets/media/image456.png){width="4.631944444444445in"
height="2.938888888888889in"}

Supponendo dunque di aver soddisfatto le due condizioni sopra indicate e
di aver inserito il componente "Spedizione" all'interno, ad esempio,
della scheda prodotto, potremo ottenere un risultato del tipo di quello
evidenziato in figura.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\spedizione_segnaposto_data_2.bmp](./assets/media/image457.png){width="5.3805555555555555in"
height="3.34375in"}

La data di prevista consegna dipenderà poi, ovviamente, dalla zona di
spedizione considerata (per la quale valgono esattamente le stesse
considerazione fatte per i costi di spedizione) e da come è stato
impostato e configurato lo schema delle consegne associate, per tale
zona, allo specifico metodo di trasporto.

**ATTENZIONE!** Per maggiori informazioni relativamente all'utilizzo del
modulo "Consegne a Domicilio" si consiglia di fare riferimento al
relativo capitolo di questo manuale ("*Ordini -- Consegne*")

Di base si tratterà di impostare per ogni schema di consegne:

- Il tempo necessario per la preparazione dei pacchi (parametro "Ore
  Preparazione")

- Un set di "Regole di Preparazione" da tarare in relazione a quello che
  è l'orario lavorativo dell'esercente

- Il tempo necessario per la consegna (parametro "Ore Consegna") in
  relazione eventualmente alla zona in cui dovrà essere effettivamente
  spedita la merce

- Un set di "Regole di Consegna" da tarare in relazione a quelli che
  sono gli orari e i giorni in cui il relativo Corriere potrà effettuare
  la consegna.

Per comprendere meglio come dover operare è bene considerare un semplice
esempio.

**[ESEMPIO]{.underline}**

Supponiamo di dover gestire un Metodo di Trasporto che utilizza un
corriere (es. Bartolini) che effettua consegne:

- dalle 8.00 alle 18.00 dal lunedì al giovedì

- dalle 8.00 alle 13.00 il venerdì

- non effettua consegne il sabato e la domenica

Supponiamo inoltre che il Vettore in esame indichi tempi di consegna di:

- 1 giorno lavorativo sull'Emilia Romagna

- 2 giorni lavorativi sul Piemonte.

Supponiamo infine di dover gestire un tempo di preparazione per la
spedizione pari a 2 ore (dal momento della ricezione dell'ordine) e che
l'orario lavorativo dell'esercente sia:

- dal lunedì al venerdì dalle 8.00 alle 18.00

- chiuso il sabato e la domenica

In queste condizioni per visualizzare una stima corretta dei tempi di
consegna dovremo:

- Flaggare il parametro "**Abilita stima costi/consegna"** presente
  nella maschera di configurazione del Metodo di Trasporto in esame

- Inserire il componente "Spedizione" all'interno, ad esempio della
  Scheda Prodotto, verificando di aver gestito correttamente il
  segnaposto "Data" all'interno del campo "Template Spedizione"

- Definire due diversi schemi di Consegne, uno sull'Emilia Romagna e uno
  sul Piemonte, con le caratteristiche di seguito indicate

[CONSENGE IN EMILIA ROMAGNA]{.underline}

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\tempi_di_consegna_1.bmp](./assets/media/image458.png){width="5.791666666666667in"
height="3.3618055555555557in"}

- **Gestione Calendario**: No

- **Ore preparazione**: 2 -- tempo necessario alla preparazione del
  pacco da spedire una volta ricevuto l'ordine

- **Ore consegna**: 10

> Considerando l'intervallo di tempo in cui il vettore garantisce le
> consegne (dalle 8.00 alle 18.00) il giorno lavorativo indicato come
> tempo previsto per portare a termine le consegne in Emilia Romagna
> equivale esattamente a 10 ore

- **Quota limite giornaliera**: non valorizzato

- **Spedizione**: Corriere Espresso -- Bartolini

- **Aree di spedizione**: Tutte le provincie dell'Emilia Romagna

- **Regole di preparazione**:

  - Una regola di tipo "Intervallo Orario" dalle 8.00 alle 18.00 senza
    indicare in maniera specifica giorni mesi o anni

  - Una regola di tipo "Eccezione Giorno Settimanale" indicando come
    giorno il Sabato

  - Una regola di tipo "Eccezione Giorno Settimanale" indicando come
    giorno la Domenica

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\tempi_di_consegna_2.bmp](./assets/media/image459.png){width="5.791666666666667in"
height="3.3618055555555557in"}

- **Regole di consegna**:

  - Una regola di tipo "Intervallo Orario" dalle 8.00 alle 18.00 senza
    indicare in maniera specifica giorni mesi o anni

  - Una regola di tipo "Intervallo Orario" dalle 8.00 alle 13.00
    indicando in maniera specifica il giorno "Venerdì" (campo "Giorno
    Settimanale")

  - Una regola di tipo "Eccezione Giorno Settimanale" indicando come
    giorno il Sabato

  - Una regola di tipo "Eccezione Giorno Settimanale" indicando come
    giorno la Domenica

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\tempi_di_consegna_2a.bmp](./assets/media/image460.png){width="5.791666666666667in"
height="3.3618055555555557in"}

In queste condizioni:

- Ordini acquisiti il lunedì mattina alle 10.00 saranno pronti per
  essere spediti alle 12 del giorno stesso e avranno come data di
  prevista consegna il martedì. Delle 10 ore (il giorno lavorativo
  indicato dal Vettore) necessarie per la consegna infatti 6 verranno
  "consumate" il giorno stesso (dalle 12 alle 18) e le 4 restanti il
  giorno successivo (martedì dalle 8 alle 12). La data esatta di
  prevista consegna sarebbe quindi martedì alle 12 orario questo in cui
  il Vettore assicura effettivamente le consegne

- Ordini acquisiti il lunedì pomeriggio alle 17 saranno considerati
  pronti per la spedizione il giorno seguente alle 9 (delle due ore
  richieste per la preparazione una verrà usata il lunedì dalle 17 alle
  18 e una la mattina seguente dalle 8 alle 9). La data di prevista
  consegna sarà quindi il mercoledì. Delle 10 ore (il giorno lavorativo
  indicato dal Vettore) necessarie per la consegna infatti 9 verranno
  "consumate" il martedì (dalle 9 alle 18) e l'ora restante verrà invece
  utilizzata il mercoledì (dalle 8 alle 9). La data esatta di prevista
  consegna sarebbe quindi mercoledì alle 9 orario questo in cui il
  Vettore assicura effettivamente le consegne

- Ordini acquisiti il venerdì mattina alle 12 saranno considerati pronti
  per la spedizione il giorno stesso alle 14 e la data di prevista
  consegna sarà quindi il lunedì seguente. Considerando infatti che il
  Vettore non effettua consegne il Venerdì pomeriggio e neppure il
  Sabato e la Domenica, le 10 ore (il giorno lavorativo indicato dal
  Vettore) necessarie per la consegna verranno usate tutte il lunedì
  seguente (dalle 8 alle 18). La data esatta di prevista consegna
  sarebbe quindi lunedì alle 18 orario questo in cui il Vettore assicura
  ancora le consegne

- Ordini acquisiti il venerdì pomeriggio alle 17 saranno considerati
  pronti per la spedizione il successivo lunedì mattina alle 10. Le due
  ore richieste per la preparazione verranno usate una il giorno stesso
  dalle 17 alle 18 e una il lunedì seguente dalle 8 alle 9.

> La data di prevista consegna sarà quindi martedì. Delle 10 ore (il
> giorno lavorativo indicato dal Vettore) necessarie per la consegna
> infatti 9 verranno "consumate" il lunedì (dalle 9 alle 18) e l'ora
> restante verrà invece utilizzata il martedì (dalle 8 alle 9). La data
> esatta di prevista consegna sarebbe quindi martedì alle 9 orario
> questo in cui il Vettore assicura effettivamente le consegne

[CONSENGE IN PIEMONTE]{.underline}

Lo schema di consegne da applicare dovrà essere in tutto e per tutto
analogo a quello appena definito per l'Emilia Romagna sia a livello di
impostazioni della Consegna che a livello di Regole da applicare.

Le uniche differenze saranno relative all'Area di Spedizione che,
ovviamente, dovrà essere impostata su tutte le provincie del Piemonte, e
al parametro "Ore Consegna".

In questo caso infatti dovendo gestire sul Piemonte un tempo di consegna
di 2 giorni lavorativi, e considerando sempre l'orario lavorativo del
vettore, il parametro "**Ore Consegna**" dovrà essere impostato sul
valore 20.

