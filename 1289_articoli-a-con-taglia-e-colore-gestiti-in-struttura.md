# ARTICOLI A CON TAGLIA E COLORE GESTITI IN STRUTTURA



In queste condizioni, gestendo sia la taglia che il colore in struttura
ci troveremo a dover trattare:

- **un prodotto padre di struttura** con un suo codice, un suo url per
  la pagina prodotto ed eventualmente anche un suo prezzo specifico

- **un prodotto figlio** con un suo codice, un suo url per la pagina
  prodotto, un suo prezzo e una sua disponibilità per ogni singola
  colore e per ogni singola taglia

In definitiva dunque, siamo sostanzialmente nelle stesse condizioni del
caso precedente (articoli a taglie e a colori gestiti con struttura +
tabella taglie/colori di Mexal) e verranno quindi utilizzati gli stessi
JSON-LD sia per la pagina prodotto dell'articolo padre di struttura sia
per gli articoli figlio.

In questo caso però taglie e colori dovranno essere gestiti con gli
ultimi due livelli della struttura e tali livelli dovranno anche essere
marcati in maniera corretta come "livello colore" e "livello taglie".

In queste condizioni dunque ogni articolo figlio avrà esattamente una
singola taglia e un singolo colore e, in conseguenza di ciò, anche le
proprietà "*size*" e "*color*" inserite nel Json-ld della scheda
prodotto del figlio avranno entrambe sempre e comunque un unico valore

