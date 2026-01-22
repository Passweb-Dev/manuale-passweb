# PERSONALIZZAZIONE DEL TOOLTIP QUANTITA' -- PREZZO PER SET OPZIONI



Come indicato all'interno del capitolo "**Catalogo -- Opzioni Articoli
-- Set**" di questo manuale, il prezzo degli articoli gestiti mediante
Custom Option potrebbe essere calcolato anche come somma tra il prezzo
base dell'articolo stesso e il prezzo delle varie opzioni selezionate in
fase di personalizzazione del prodotto (parametro "**Calcolo**"
impostato su "**Sommatoria**"). Il prezzo delle singole opzioni,
inoltre, potrebbe variare anche in relazione alla quantità dell'articolo
effettivamente inserita in carrello (parametro "**Tipo Prezzo**" della
singola opzione impostato sul valore "**Scaglioni**").

In queste condizioni ("**Calcolo = Sommatoria**" e "**Tipo Prezzo =
Scaglioni**") sarà possibile visualizzare, in corrispondenza di ogni
singola opzione, un messaggio per indicare all'utente, in maniera più
precisa, quello che sarà effettivamente il prezzo della relativa opzione
nel momento in cui la quantità dell'articolo inserita in carrello
dovesse ricadere in determinato scaglione

![Videate\\set_opzioni_scaglioni_prezzo_opzione.bmp](./assets/media/image465.png)

**ATTENZIONE!** il messaggio in esame non verrà visualizzato se
l'opzione è gestita mediante un controllo di tipo List

Per personalizzare questo messaggio è sufficiente accedere alla sezione
relativa alla gestione dei Testi dei Componenti (menu "**Sito -- Testi /
Messaggi del sito -- Testi dei Componenti**"), selezionare il componente
"**Set Opzioni**" e cliccare poi sul pulsante "**Modifica Testi**"
presente nella barra degli strumenti.

In questo modo verrà infatti visualizzata la maschera "**Testi
Componente -- Set Opzioni**"

![](./assets/media/image466.png)

all'interno della quale troveremo un editor HTML (sezione "**Tooltip
Quantità -- Prezzo**") da utilizzare per personalizzare il messaggio.

Il pulsante "**Seleziona un segnaposto**" presente immediatamente al di
sopra dell'editor HTML consente di inserire all'interno del messaggio
uno dei seguenti segnaposto

- **CICLO -- Quantità:** consente di inserire l'istruzione

> \$quantityItems:{
>
> }\$
>
> con cui poter ciclare tra tutti i diversi scaglioni di quantità/prezzo
> definiti per l'opzione in esame.

- **Quantità** (**\$it.quantity\$):** quantità minima con cui l'articolo
  dovrà essere inserito in carrello per poter applicare le condizioni
  del relativo scaglione (valore del campo "**Da**" nella definizione
  dello scaglione di prezzo)

- **Prezzo** **(\$it.price\$**): prezzo applicato all'opzione in esame
  nel momento in cui la quantità dell'articolo presente in carrello
  dovesse essere tale da far applicare il relativo scaglione

**ATTENZIONE!** considerando che il messaggio in questione verrà
effettivamente visualizzato sul front end del sito solo nel caso in cui
il prezzo dell'opzione in esame sia gestito mediante degli scaglioni
quantità, **i segnaposto "Quantità" e "Prezzo" per poter essere
valorizzati in maniera corretta dovranno necessariamente essere inseriti
all'interno dell'istruzione "Ciclo -- Quantità"** come nell'esempio di
seguito riportato:

\<ul class="list-unstyled small"\>

**\$quantityItems:{**

\<li\>+ **\$it.price\$** per acquisiti in qta maggiore di
**\$it.quantity\$**\</li\>

**}\$**

\</ul\>

Per maggiori informazioni relativamente a come poter impostare per le
opzioni del set il prezzo in base alla quantità dell'articolo
effettivamente inserita in carrello si veda quanto indicato all'interno
del capitolo "*Catalogo -- Opzioni Articoli -- Opzioni del Set*" di
questo manuale

