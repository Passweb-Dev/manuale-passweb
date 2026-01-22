# COMPONENTI E-COMMERCE -- DESCRIZONE



Il Componente Ecommerce **"Descrizione"**

![](./assets/media/image429.png)

corrisponde esattamente all'omonimo campo **"Descrizione"** presente
all'interno dell' anagrafica Passweb di ogni articolo (sezione
Descrizioni)

![](./assets/media/image430.png)

**Inserendo questo Componente all'interno di un Componente E-Commerce di
primo livello (es. Catalogo E-commerce), esso verrà quindi sostituito,
articolo per articolo, con il testo per essi inserito all'interno del
campo Descrizione sopra evidenziato.**

Il campo Descrizione potrà essere valorizzato in due modi differenti,
dipendentemente anche dalla tipologia di sito considerata.

Nello specifico:

**[ECOMMERCE MEXAL]{.underline}**

1.  Direttamente da Passweb attraverso la maschera di "Modifica
    Articolo" sopra evidenziata

2.  Allegando in Docuvision allo specifico articolo una risorsa di tipo
    D (Descrizione Aggiuntiva) corrispondente ad un file .txt

Nel caso in cui infatti sia stata associata in Docuvision allo specifico
articolo una risorsa di tipo D, dopo aver effettuato l'importazione
delle risorse dal gestionale, il campo Descrizione sopra evidenziato
verrà automaticamente valorizzato con il contenuto del corrispondente
file .txt associato all'articolo.

> **NOTA BENE:** per maggiori informazioni relativamente
> all'associazione mediante Docuvision delle varie risorse (immagini,
> schede tecniche e descrizioni aggiuntive) agli articoli gestiti
> all'interno del sito e alla loro importazioni in Passweb, si rimanda
> al relativo capitolo ("Associazione delle immagini e delle schede
> tecniche articolo all'interno del gestionale") di questo manuale.

**[ECOMMERCE HO.RE.CA.]{.underline}**

1.  Direttamente da Passweb attraverso la maschera di "Modifica
    Articolo" sopra evidenziata

2.  Alla sincronizzazione prelevando il relativo valore direttamente da
    quanto inserito nel gestionale all'interno del campo **"Descrizione
    Secondaria"** dell'anagrafica dello specifico articolo.

![](./assets/media/image431.png)

> **NOTA BENE:** i valori prelevati alla sincronizzazione dal
> corrispondente campo dell'anagrafica articoli possono andare a
> sovrascrivere eventuali variazioni apportate per questi stessi valori
> direttamente all'interno del Wizard di Passweb.

Rilasciando il Componente nella posizione desiderata verrà visualizzata
**la sua maschera di gestione e configurazione**

![](./assets/media/image432.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

- **Nome:** consente di impostare un nome per il Componente che si sta
  editando.

- **Pubblico (selezionato a default):** consente di impostare la
  visibilità del componente lato sito web. Se selezionato il
  corrispondente componente verrà correttamente pubblicato e
  visualizzato all'interno del sito. Nel caso in cui invece tale
  parametro non sia selezionato, il corrispondente componente passerà in
  modalità "Offline", sarà quindi visibile all'interno del Wizard, dove
  potrà essere normalmente gestito, ma non verrà pubblicato e
  visualizzato all'interno del sito.

- **Periodo di Pubblicazione:** consente di associare al Componente in
  oggetto uno specifico periodo di pubblicazione, definendone
  l'effettiva data di pubblicazione e la corrispondente data di
  oscuramento.

> Nel primo dei due campi disponibili occorrerà quindi indicare,
> utilizzando l'apposito calendario, la data di inizio pubblicazione.
> Nel secondo campo andrà invece specificata la data di fine
> pubblicazione.
>
> **ATTENZIONE!** Le date indicate all'interno di questi campi verranno
> considerate solo ed esclusivamente nel caso in cui il precedente
> parametro "Pubblico" sia stato selezionato

- **Massimo Caratteri del testo accorciato:** consente di specificare il
  numero massimo di caratteri che dovranno essere utilizzati per
  visualizzare il contenuto di questo componente **nel momento in cui
  questo dovesse essere inserito all'interno di componenti quali il
  "Catalogo E-commerce", "Offerte/Novità", "Abbinati" ecc...**

> **NOTA BENE:** nel caso in cui il componente in oggetto venga inserito
> all'interno della scheda prodotto verrà sempre visualizzato tutto il
> suo contenuto indipendentemente dal quanto impostato all'interno del
> campo "Massimo Caratteri del testo accorciato".

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

