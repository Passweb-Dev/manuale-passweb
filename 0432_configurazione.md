# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\reso_genera_template_res.bmp](./assets/media/image329.png){width="4.588888888888889in"
height="2.938888888888889in"}

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente stesso.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

- **Nome:** permette di inserire un nome per il campo che si sta
  editando;

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

- **Gestione Allegati:** consente di abilitare o meno la gestione degli
  allegati sul componente in esame.

> Se impostato a **SI**, gli utenti del sito avranno quindi la
> possibilità di allegare determinati file al proprio documento di reso
> merce direttamente in fase di creazione del reso.
>
> Al contrario nel momento in cui il parametro in questione dovesse
> essere impostato su **NO**, eventuali allegati al documento di reso
> merce potranno essere aggiunti e gestiti solo ed esclusivamente
> dall'amministratore del sito operando per questo dal gestionale
> (mediante Docuvision) oppure direttamente dal Wizard di Passweb ma, in
> ogni caso, sempre dopo che il documento in esame sia stato
> correttamente memorizzato.
>
> **ATTENZIONE!** Per maggiori informazioni relativamente alla
> possibilità di allegare determinati file ai documenti di reso merce si
> veda anche il successivo paragrafo "**Reso Merce -- Gestione
> Allegati**"

Anche in questo caso, come già fatto per il componente Ordine, per
comprendere al meglio il significato dei restanti di configurazione, è
bene ricordare come all'interno del modulo di richiesta reso merce
l'elenco degli articoli per i quali poter effettuare la richiesta di
reso è strutturato su di una griglia responsiva le cui colonne possono
essere definite direttamente all'interno della sezione "**Gestione
Contenuti**" presente nella maschera di gestione e configurazione del
Componente stesso

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\reso_griglia_articoli.bmp](./assets/media/image330.png){width="4.595138888888889in"
height="4.227083333333334in"}

Fatta questa considerazione, possiamo ora comprendere in maniera più
semplice il significato degli ultimi parametri presenti nella maschera
di configurazione del componente Ordine.

Nello specifico dunque il parametro:

**Larghezza Colonna dei Bottoni:** consente di impostare la larghezza
che dovrà assumere, all'interno della griglia articoli, la colonna
contenente il check di selezione degli articoli per i quali effettuare
le richiesta di reso.

Come per tutte le griglie responsive anche in questo caso la larghezza
di ogni colonna (compresa quella dei bottoni) si esprime definendo
quante delle 12 sezioni in cui risulta essere suddivisa ogni singola
riga, dovranno essere effettivamente occupate dalla colonna stessa.

**Posizionamento Colonna dei Bottoni**: consente di decidere se la
colonna dei bottoni dovrà essere posizionata a sinistra oppure a destra
delle informazioni relative allo specifico articolo

**Posizione dei campi di riepilogo dei Totali:** consente di definire
come dovranno essere posizionati i campi relativi ai Totali presenti nel
dettaglio del documento che verrà visualizzato, come per l'ordine, una
volta confermata la richiesta di reso.

E' possibile selezionare una delle seguenti opzioni:

- Allineati a Destra

- Allineati a Sinistra

- Centrati

- Opposti

**ATTENZIONE!** Indipendentemente da quella che sarà la larghezza
impostata per ogni singola colonna della griglia articoli il suo
comportamento responsivo è tale per cui **in corrispondenza di
risoluzioni inferiori ai 992 px la griglia stessa si linearizzerà
disponendo tutte le colonne una sotto l'altra**

Una volta settati i parametri di configurazione del Componente sarà
quindi necessario definirne i contenuti stabilendo innanzitutto il
numero di colonne in cui dovrà essere suddivisa ogni singola riga
articolo e, successivamente, andando ad inserire in queste stesse
colonne i componenti desiderati (Titolo, Prezzo, Immagine ecc...).

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

