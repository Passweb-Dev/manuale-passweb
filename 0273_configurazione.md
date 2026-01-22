# CONFIGURAZIONE



Una volta inserito il Componente all'interno della pagina web, verrà
aperta in automatico **la sua maschera di gestione e configurazione**

![](./assets/media/image80.png)

suddivisa in varie sezioni.

All'interno della sezione "**Dati Componente**" sarà possibile inserire
il contenuto e settare i principali parametri di configurazione del
componente.

In particolare, per la tipologia di Componente in questione, sarà
possibile impostare un valore per i seguenti parametri:

- **Nome** (obbligatorio), consente di inserire un nome per il
  Componente Paragrafo che si sta realizzando

- **Pubblico (selezionato a default):** consente di impostare la
  visibilità del componente lato sito web.

- **Periodo di Pubblicazione:** consente di associare al Componente in
  oggetto uno specifico periodo di pubblicazione, definendone
  l'effettiva data di pubblicazione e la corrispondente data di
  oscuramento.

> **ATTENZIONE!** Per maggiori informazioni relativamente ai parametri
> **Nome, Pubblico, Periodo di Pubblicazione** si veda anche quanto
> indicato all'interno del capitolo "*Configurazione Componenti --
> Caratteristiche generali* -- *Dati Componente* " di questo manuale

- **Statico**: consente di decidere se il componente in esame deve o
  meno essere reso statico

> **ATTENZIONE!** Per maggiori informazioni relativamente al parametro
> **Statico** si veda anche quanto indicato all'interno del capitolo
> "*Configurazione Componenti -- Caratteristiche generali* --
> *Staticizzazione e caricamento asincrono*" di questo manuale

- **Disabilita Cache:** consente di disabilitare la possibilità di
  inserire in cache il componente in esame.

> Per maggiori informazioni relativamente alla gestione della cache in
> Passweb si veda anche il relativo capitolo di questo manuale
> ("*Configurazione -- Cache*")

All'interno della sotto sezione "**Opzioni Galleria**" è possibile
invece decidere, il tipo di Galleria da utilizzare, il numero di
immagini che dovranno essere visualizzate all'interno dei questa stessa
galleria, su quante righe e colonne queste immagini dovranno essere
disposte, che dimensioni dovranno avere ...

Nello specifico dunque il parametro:

**Abilita galleria Mansory:** consente di impostare il tipo di Galleria
da utilizzare. E' possibile selezionare una delle seguenti opzioni:

- **No**: in questo caso verrà creata una classica Galleria in cui le
  immagini saranno disposte all'interno di un'apposita griglia suddivisa
  in righe e colonne

![Videate\\galleria_immagini.bmp](./assets/media/image81.png)

> In queste condizioni dunque è necessario che le dimensioni delle
> immagini presenti in Galleria siano sempre le stesse.
>
> In caso contrario potrebbero infatti crearsi degli "scalini" più o
> meno evidenti tra un' immagine e l'altra, determinati dalle diverse
> altezze, che andrebbero pregiudicare l'allineamento dei vari elementi
>
> **ATTENZIONE!** Il comportamento responsivo della griglia è tale per
> cui in corrispondenza di risoluzioni del dispositivo di
> visualizzazione inferiori a 992px le immagini della galleria si
> disporranno automaticamente su due colonne. Per risoluzioni inferiori
> ai 768 px invece tutta la galleria si linearizzerà disponendo le
> immagini una sotto l'altra

- **Si**: in questo caso verrà creata una Galleria di tipo "Mansory" in
  cui le varie immagini si disporranno automaticamente in base alle loro
  dimensioni (altezza e larghezza) mantenendo comunque sempre le stesse
  distanze l'una dall'altra

![](./assets/media/image82.png)

> Come si può notare dalla figura sopra riportata, in queste condizioni
> non è quindi strettamente necessario che tutte le immagini abbiano
> esattamente le stesse dimensioni per garantire una corretta
> visualizzazione della Galleria.
>
> A differenza del caso precedente, inoltre sarà possibile indicare
> quante immagini considerare per riga per risoluzioni inferiori ai 992
> px mentre per risoluzioni inferiori a 768 px il componente si
> linearizzerà e visualizzerà un'immagine sotto l'altra

**Dimensione Thumbnail (obbligatorio):** consente di indicare la
dimensione (in pixel) che dovranno assumere le anteprime delle immagini
presenti all'interno della galleria.

**ATTENZIONE!** Indipendentemente dalla tipologia di Galleria utilizzata
cliccando su una delle immagini presenti verrà visualizzata l'immagine
nelle sue dimensioni reali.

**Numero Immagini da Visualizzare -- solo per "Abilita Galleria Mansory
= No":** consente di indicare quante immagini dovranno essere
visualizzate complessivamente all'interno della galleria (parametro
"**Numero immagini da Visualizzare**")

**Numero di colonne della griglia per schermi con risoluzione maggiore
di 992px:** consente di indicare il numero di immagini da visualizzare
per singola riga per risoluzioni dello schermo superiori a 992px

**Numero di colonne della griglia per schermi con risoluzione minore di
992px -- solo per "Abilita Galleria Mansory = Si":** consente di
indicare il numero di immagini da visualizzare per singola riga per
risoluzioni dello schermo inferiori a 992px

Una volta settati i parametri di configurazione della Galleria sarà poi
necessario, ovviamente, caricare le singole immagini che dovranno
entrare a far parte della galleria stessa agendo, in questo senso, dalla
sezione "Gestione Immagini" presente nella maschera di configurazione di
questa specifica tipologia di componenti.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**", "**Distribuzione**" e "**Protezione**",
presenti nella maschera di gestione e configurazione di tutti i
componenti Passweb, si veda anche il capitolo " Varianti Responsive --
Configurazione Componenti -- Caratteristiche Generali " di questo
manuale.

