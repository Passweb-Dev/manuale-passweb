# CREAZIONE DELL'INSERZIONE



Per poter pubblicare su una delle piattaforme gestite articoli con un
massimo di due elementi varianti (es. taglie e colori) **è necessario
utilizzare apposite inserzioni** definendo in maniera corretta tutte le
specifiche necessarie per poter consentire all'inserzione stessa di
gestire questa ben precisa tipologia di articoli.

**ATTENZIONE!** Per maggiori informazioni relativamente alle specifiche
addizionali da utilizzare per abilitare un'Inserzione alla pubblicazione
di articoli varianti si veda il capitolo "*Specifiche addizionali*"
relativo alla piattaforma verso cui si vuole realizzare l'integrazione

La particolarità delle specifiche che permettono di abilitare
un'Inserzione alla pubblicazione di articoli varianti è rappresentata
dal fatto che, oltre a poter essere utilizzate per fornire informazioni
aggiuntive su articoli "semplici", possono essere utilizzate anche per
gestire il corrispondente elemento di variazione dell'articolo.

Nel primo caso (specifica utilizzata per gestire informazioni aggiuntive
su articoli semplici) il campo "Modalità" dovrà essere impostato su una
delle seguenti opzioni**: Attributo Marketplace, Attributo Passweb**,
**Personalizzato**

Nel secondo caso (specifica utilizzata per gestire un elemento di
variazione dell'articolo) il campo "Modalità" dovrà essere impostato
sull'opzione (disponibile solo per queste particolari specifiche)
"**Elemento di Variazione**"

![](./assets/media/image413.png)

In queste condizioni il campo "**Valore**", utilizzato come sempre per
indicare da dove dovranno essere prelevati i valori da assegnare
articolo per articolo alla specifica in esame, potrà essere impostato su
una delle seguenti opzioni:

- **Tabella Taglie** (solo nel caso in cui Passweb sia collegato a
  Mexal)

- **Penultimo Campo Struttura**

- **Ultimo Campo Struttura**

Facendo riferimento, ad esempio, alla configurazione indicata in figura

![](./assets/media/image414.png)

il colore degli articoli pubblicati sulla piattaforma terza coinciderà
con i valori, indicati lato gestionale, nell'ultimo livello della
struttura utilizzata mentre le taglie verranno prelevate direttamente
dai valori indicati nella tabella taglie di Mexal.

Nel momento in cui una delle specifiche sopra indicate dovesse essere
inserita in un'Inserzione e mappata come Elemento di Variazione,
l'Inserzione stessa sarà abilitata alla sola pubblicazione di articoli
che presentano gli elementi di variazione indicati

Al contrario in assenza di tali specifiche l'inserzione potrà essere
utilizzata per pubblicare solo ed esclusivamente articoli di magazzino
"semplici"

**ATTENZIONE! Le inserzioni configurate con le specifiche indicate
all'interno di questo capitolo, e abilitate quindi per poter gestire
articoli a taglie / colori (o comunque con un massimo di due elementi
varianti), potranno essere utilizzate solo ed esclusivamente per la
pubblicazione di questa particolare tipologia di articoli**

Allo stesso modo inserzioni "tradizionali", utilizzate cioè per
pubblicare normali articoli di magazzino, non potranno mai essere
utilizzate per pubblicare articoli a taglie / colori o comunque con
elementi varianti

