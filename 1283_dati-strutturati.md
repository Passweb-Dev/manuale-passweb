# DATI STRUTTURATI



Viviamo in un'epoca in cui le pagine web non sono più soltanto documenti
destinati alla lettura da parte degli esseri umani.

Ogni giorno miliardi di informazioni vengono scambiate, analizzate e
interpretate non da persone, ma da macchine: motori di ricerca,
assistenti vocali, chatbot, sistemi di raccomandazione e intelligenze
artificiali che elaborano e collegano dati per fornire risposte,
suggerimenti o contenuti.

Il modo in cui una macchina vede ed analizza una pagina web non è però
lo stesso di un essere umano.

Quando un utente umano apre una pagina web vede testo, immagini,
pulsanti, video ... tutti elementi che lo mettono nelle condizioni di
capire immediatamente se quello che sta guardando è la scheda di un
prodotto, una biografia, la recensione di un ristorante ...

Un motore di ricerca, un sistema di intelligenza artificiale, un chatbot
... di fronte allo stesso codice HTML, vedono invece soltanto frammenti
di testo e tag. Senza un aiuto specifico e senza delle informazioni
strutturate in un certo modo queste macchine non possono sapere con
certezza che "€59,90" è il prezzo di un prodotto o che "Mario Rossi" è
l'autore di un articolo.

**L'HTML tradizionale fornisce una rappresentazione visiva e testuale
dei contenuti di una pagina web utile solo per gli utenti umani, non per
le macchine.**

E' proprio qui che entrano in gioco **i dati strutturati**, una delle
tecnologie più importanti ( e spesso più trascurate) del web
contemporaneo.

I dati strutturati consentono infatti di aggiungere un livello di
semantica al contenuto di una pagina web trasformando quello stesso
contenuto da semplice testo, comprensibile agli umani, a informazione
strutturata comprensibile anche ai sistemi automatici

In altre parole, se una pagina mostra un prodotto, un evento, una
ricetta o una recensione, i dati strutturati servono a far sapere
esplicitamente alle macchine che cosa rappresentano quelle informazioni,
come sono organizzate e quali relazioni esistono tra di esse

Immaginiamo, ad esempio, una scheda prodotto di un sito e-commerce che
mostra queste informazioni:

Scarpe da corsa modello SpeedRun

Prezzo: 89,90 €

Disponibilità: In magazzino

Valutazione: ★★★★☆ (4,5 su 5)

Per un utente umano queste informazioni sono chiarissime: si tratta di
un prodotto disponibile all'acquisto, con un prezzo e una valutazione
media positiva.

Per Google, per un assistente vocale, per un intelligenza artificiale
... senza dati strutturati questi valori sono solo puro e semplice
testo.

Aggiungendo i dati strutturati, possiamo far sapere esplicitamente anche
ai diversi sistemi automatici:

- che "Scarpe da corsa modello SpeedRun" è il nome di un prodotto;

- che "89,90 €" è il suo prezzo, espresso in euro;

- che "In magazzino" rappresenta la sua disponibilità;

- che "4,5" è un valore di rating medio, basato su un certo numero di
  recensioni.

Grazie a queste informazioni i motori di ricerca, ad esempio, potranno
poi mostrare il prodotto nei risultati arricchiti (i cosiddetti rich
results) con il prezzo, la disponibilità e le stelle di valutazione.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\microdati_3.bmp](./assets/media/image1.png)

L'utente trova subito l'informazione utile, e il sito ottiene maggiore
visibilità.

Dal punto di vista tecnico esistono diversi modi per implementare i dati
strutturati e inserirli all'interno di una pagina web e si basano tutti
sullo stesso vocabolario semantico di **Schema.org**
(<https://schema.org/>), un'iniziativa congiunta di Google, Microsoft,
Yahoo e Yandex che definisce migliaia di tipi di entità (Product,
Person, Event, Organization, Review, Article, ecc.) e proprietà (name,
description, price, image, url, brand, aggregateRating, ecc.) che
possono essere utilizzate per descrivere i contenuti di una pagina web.

I tre principali formati di dati strutturati sono:

1.  **RDFa (Resource Description Framework in Attributes)**

2.  **Microdata**

3.  **JSON-LD (JavaScript Object Notation for Linked Data)**

Pur basandosi, come detto, sullo stesso vocabolario semantico, ciascuno
dei formati sopra indicati differisce rispetto agli altri per il modo in
cui vengono rappresentate le informazioni.

Nel corso del tempo si è cercato infatti di semplificare la vita agli
sviluppatori. Il formato RDFa infatti, pur essendo molto potente
richiedeva conoscenze semantiche avanzate.

I microdati, invece, sfruttando una sintassi HTML5 basata sugli
attributi erano pensati per essere più facili da integrare nel codice
HTML.

Oggi, tuttavia, Google raccomanda il formato JSON-LD per la sua
chiarezza e, soprattutto, per la sua separazione dal contenuto visibile

Nei successivi capitoli di questo manuale esamineremo più nel dettaglio
i due formati di dati strutturati ("**Microdata**" e "**JSON-LD**")
gestiti da Passweb e cercheremo di capire come ognuno di essi tende a
rappresentare le informazioni e come fare per poterli implementare
all'interno del proprio sito Ecommerce

