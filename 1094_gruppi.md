# GRUPPI



Come evidenziato nei precedenti capitoli, volendo, è possibile
configurare il proprio sito in maniera tale che determinate Tasse
Addizionali (quindi non di tipo IVA) vengano applicate solamente a
determinati utenti.

La sezione "**Gruppi**", visibile solo nel caso in cui il parametro di
configurazione "**Tipologia Tassa**" sia stato impostato sul valore
"**Tassa Extra**", consente infatti di associare la tassa addizionale
che si sta codificando ad uno o più Gruppi di Utenti

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_tassa_2.bmp](./assets/media/image448.png){width="5.616666666666666in"
height="3.4479166666666665in"}

**ATTENZIONE!** Per ovvie ragioni non è possibile associare Tasse di
tipo IVA a Gruppi Utente

Per creare un'associazione "Gruppo Utenti -- Tassa" è sufficiente
selezionare il Gruppo desiderato dall'elenco presente nel box di
sinistra, ed inserirlo nel box di destra cliccando sul pulsante
raffigurante una piccola freccia rivolta verso destra. Allo stesso modo
per eliminare l'associazione "Gruppo Utenti -- Tassa", sarà sufficiente
selezionare il gruppo desiderato dall'elenco di destra ed inserirlo in
quello di sinistra cliccando sul pulsante raffigurante una piccola
freccia rivolta verso sinistra.

Una volta creata un'associazione di questo tipo la corrispondente Tassa
verrà applicata solo ed esclusivamente nel caso in cui ad effettuare
l'ordine dovesse essere un utente appartenente ad uno dei gruppi
selezionati.

Nel momento in cui non dovesse invece essere creata nessuna associazione
la tassa in esame verrà sempre applicata indipendentemente da chi sta
effettuando l'ordine

**ATTENZIONE:** Nel caso in cui ad effettuare l'ordine dovesse essere un
Agente (Ecommerce Mexal) per conto dei suoi clienti verranno considerate
le tasse associate all'eventuale gruppo di appartenenza dell'Agente.

