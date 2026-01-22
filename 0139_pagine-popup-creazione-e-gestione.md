# PAGINE POPUP -- CREAZIONE E GESTIONE



Passweb consente di creare e visualizzare una pagina generica sotto
forma di Popup. Tali pagine verranno poi identificate all'interno
dell'albero con uno sfondo giallo chiaro
(![Videate\\pagina_popup_res.bmp](./assets/media/image115.png) ).

Per fare in modo che una pagina generica possa essere visualizzata sotto
forma di Popup, è sufficiente seguire tre semplici passaggi:

1.  Marcare la pagina in esame in maniera tale che possa essere
    utilizzata e visualizzata come Popup impostando per questo il
    parametro "**Utilizza come Popup**" presente nelle proprietà della
    pagina stessa sul valore "Si"

![](./assets/media/image116.png)

> **ATTENZIONE!** Le pagine di tipo E-Commerce non possono essere
> marcate come pagine Popup
>
> Selezionando questo parametro la pagina non sarà più raggiungibile dal
> suo percorso Web, ma potrà essere richiamata solo ed esclusivamente
> sotto forma di Popup dai link che permettono di visualizzare questo
> tipo di elementi

2.  Editare la pagina, e quindi il contenuto del Popup, utilizzando le
    normali logiche di gestione di presenti in Passweb.

> **ATTENZIONE:** non tutte le tipologie di componenti potranno essere
> inserite all'interno delle Pagine di tipo Popup

3.  Inserire in una qualsiasi pagina del sito uno dei componenti che
    consentono di richiamare questo particolare tipo di pagine
    visualizzandole sotto forma di Popup.

> **In questo senso è attualmente possibile richiamare e visualizzare in
> maniera automatica una pagina di tipo Popup partendo da un componente
> di tipo Immagine, da un componente di tipo Menu o da un componente di
> tipo Paragrafo**
>
> Nello specifico tra i parametri di configurazione di un componente di
> tipo Immagine comparirà anche il parametro **"Apri come Finestra
> Modale"**

![](./assets/media/image117.png)

> Allo stesso modo anche in fase di configurazione delle singole voci di
> un menu, oppure utilizzando un componente Paragrafo per creare dei
> link a pagine interne al sito, comparirà lo stesso tipo di parametro

![](./assets/media/image118.png)

![](./assets/media/image119.png)

> **Selezionando questo parametro la pagina di destinazione del link di
> collegamento associato all'immagine, alla specifica voce di menu o
> allo specifico testo del componente Paragrafo, verrà aperta sotto
> forma di Popup**
>
> Ovviamente, in queste condizioni il parametro "Destinazione Link",
> attraverso il quale poter specificare dove aprire la pagina di
> destinazione associata ad un normale link, non verrà preso in
> considerazione.

**NOTA BENE:** i Popup gestiti all'interno di Passweb attraverso il
meccanismo sopra indicato non sono dei veri e propri Popup ma bensì
delle finestre modali e, in quanto tali, non sono sottoposti ai vincoli
di "Blocco Popup" che possono essere o meno attivati a livello client
sul browser del visitatore del sito

Ovviamente affinchè tutto il meccanismo possa funzionare in maniera
corretta è indispensabile che la pagina di destinazione del link
associato all'immagine, alla voce di menu, o allo specifico testo
all'interno del componente Paragrafo, sia stata marcata per poter essere
utilizzata come Popup secondo quanto descritto al punto 1.

**In caso contrario, nel momento in cui la pagina di destinazione del
link di collegamento non fosse stata marcata come pagina di tipo Popup,
non verrà aperta una finestra modale ma bensì un i-frame con tutto ciò
che ne consegue (ad esempio a livello di navigabilità all'interno dell'
i-frame stesso).**

