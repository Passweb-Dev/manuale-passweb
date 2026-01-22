# TAGLIE E COLORI CON ARTICOLO STRUTTURATI



Nei precedenti capitoli di questo manuale abbiamo messo in evidenza
come, nei siti Ecommerce collegati a Mexal, sia possibile gestire
articoli a taglie oppure a colori sfruttando per questo Tabella Taglie
(*Magazzino -- Tabelle Aziendali -- Taglie*) presente all'interno del
gestionale

**Nel caso in cui l'esigenza dovesse invece essere quella di gestire
articoli che siano contemporaneamente a Taglie e a Colori sarà
necessario ricorre, per forza di cose, agli articoli strutturati e al
relativo configuratore di prodotto.**

**ATTENZIONE!** Attraverso la Tabella Taglie di Mexal è possibile
gestire solo articoli a taglie oppure solo articoli a colore.

Questo tipo di esigenza potrebbe quindi essere gestita realizzando in
Mexal una struttura del tipo di quella qui di seguito riportata.

![](./assets/media/image395.png)

**Attraverso questa struttura verranno quindi gestiti i colori degli
articoli mentre le taglie saranno gestite attraverso l'apposita tabella
Mexal.**

Supponiamo ora di aver codificato tra i nostri articoli un articolo
FELPA a taglie, padre della struttura sopra evidenziata, al quale è
stato associato una Cartella Abbinamenti, anch'essa a tre livelli, del
tipo di quella qui di seguito riportata:

  --------------------------------------------------------------------
  **COLLEZIONE**         **LINEA**              **COLORE**
  ---------------------- ---------------------- ----------------------
  2009 - 2010            EST - INV              BI -- NER -- ROS --
                                                BLU - VER

  --------------------------------------------------------------------

e supponiamo di aver codificato, come articoli a taglie, anche i
seguenti articoli figlio:

FEL2009ESTBIA

FEL2009ESTNER

FEL2010INVNER

Dopo aver esportato all'interno del sito sia l'articolo padre che i due
articoli figlio, potrebbe sorgere ora la necessità di visualizzare
all'interno del negozio web e di far così selezionare all'utente, non
direttamente i due articoli figlio ma solamente l'articolo padre FEL, in
modo tale da poter poi utilizzare il configuratore secondo quelle che
potrebbero essere le specifiche esigenze del caso.

Per soddisfare questa esigenza sarà quindi necessario ricorrere alla
funzionalità Mexal **"Visualizza articoli in Negozio"** attraverso la
quale nascondere all'interno del Catalogo E-commerce i due articoli
figlio e visualizzare così il solo articolo padre.

Nulla vieta comunque di visualizzare all'interno del negozio web e di
far quindi scegliere all'utente direttamente sia l'articolo padre che i
due articoli figlio.

Supponiamo poi di aver impostato il Configuratore in maniera tale da
fare in modo che inizialmente visualizzi solo il primo livello della
struttura con le diverse possibili opzioni di scelta e sulla base delle
scelte effettuate dall'utente per questo primo livello vengano poi
visualizzati i restanti campi con i corretti valori ammessi (**Tipologia
di Visualizzazione = Vincolante al precedente livello).**

Supponiamo inoltre di aver impostato per il Configuratore una modalità
di visualizzazione lineare (**Modalità di Visualizzazione = Lineare**)

Supponiamo infine di aver impostato il Configuratore anche in maniera
tale da fare in modo che le diverse possibili configurazioni di prodotto
finto a cui l'utente potrà arrivare utilizzando il configuratore, siano
determinate sulla base degli articoli figlio già codificati in Mexal e
correttamente esportati all'interno del sito web.

In queste condizioni dunque nel momento in cui l'utente andrà a
selezionare all'interno del sito web l'articolo FEL verrà ricondotto
alla specifica pagina prodotto con all'interno il Componente
Configuratore trovandosi quindi in una situazione del tipo di quella qui
di seguito riportata

Selezionando come opzione del primo livello la voce "Collezione 2009" si
abiliterà il secondo livello di scelta con al suo interno la sola voce
EST

Selezionando quindi l'opzione EST si abiliterà il terzo livello di
scelta con al suo interno le voci BIA e NER

Effettuata una scelta anche per il terzo e ultimo livello l'articolo
sarà completamente configurato. Inoltre essendo questa configurazione
corrispondente ad un articolo figlio già presente nelle anagrafiche di
Mexal ed esportato sul sito, nel caso in cui siano state associate ad
esso determinate immagini queste verranno visualizzate e sostituite alle
immagini originarie dell'articolo padre.

A questo punto dunque l'articolo è pronto per essere inserito in
carrello e per poter essere acquistato. Essendo questo poi un articolo a
taglie, come del resto il corrispondente articolo padre, ed essendo
stata abilitata per la specifica serie di taglie la grafica Estesa,
l'utente potrà decidere per ogni singola taglia la quantità del prodotto
da inserire in Carrello.

Ovviamente operando in questo modo, prima di poter inserire le taglie da
acquistare, l'utente dovrà per forza di cose terminare la configurazione
di un articolo figlio.

Nel caso in cui l'esigenza dovesse essere invece quella di mettere
l'utente nelle condizioni di inserire più rapidamente per diversi
articoli figlio e per diverse taglie le quantità da inserire in carrello
si potrebbe allora pensare di utilizzare per il configuratore non una
grafica lineare ma bensì una grafica di tipo tabellare, impostando per
questo, in fase di configurazione della struttura, il parametro
**Modalità di Visualizzazione** su uno dei valori **Tabella Esplosa,
Tabella Esplosa Divisa o Tabella Matrice**.

Per maggiori informazioni in merito alle modalità di visualizzazione con
grafica tabellare per il configuratore di prodotto si veda anche il
precedente capitolo ("*Modifica Struttura*") di questo manuale.

