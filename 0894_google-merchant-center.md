# GOOGLE MERCHANT CENTER



Lo scopo di questo manuale non è certamente quello di spiegare il
funzionamento del Merchant Center di Google (per questo si rimanda alla
specifica documentazione presente in rete). E' però importante chiarire
dove poter trovare, all'interno di questo strumento, gli articoli
esportati direttamente dal nostro sito Ecommerce.

In questo senso dunque, una volta terminato correttamente il processo di
pubblicazione sarà sufficiente accedere al Merchant Center e portarsi
all'interno della sezione "**Prodotti -- Tutti i prodotti**" cliccando
sulla corrispondente voce di menu

![](./assets/media/image515.png)

All'interno di questa sezione potremo infatti trovare l'elenco completo
di tutti i prodotti attualmente gestiti sul Merchant Center e, tra
questi, anche quelli esportati direttamente dal nostro sito Ecommerce

Cliccando su uno qualsiasi dei prodotti presenti in elenco potremo
accedere alla sua scheda dove troveremo in dettaglio tutte le
informazioni prelevate, in relazione all'articolo stesso, direttamente
da nostro sito Ecommerce (immagini, prezzi, attributi ecc...)

![](./assets/media/image516.png)

![](./assets/media/image517.png)

Sempre all'interno di questa sezione potremo trovare anche maggiori
informazioni relativamente ad eventuali problemi legati alla
pubblicazione dello specifico articolo (pannello "**Stato Articolo**")

![](./assets/media/image518.png)

In questo senso è bene chiarire alcune cose di fondamentale importanza.

**Google Merchant non mette a disposizione dell'utente una sandbox da
poter utilizzare per effettuare eventuali test di pubblicazione**

Come indicato da Google stesso (
<https://developers.google.com/shopping-content/v2/how-tos/testing> )
per effettuare dei test l'unica possibilità è quella di utilizzare un
Account Merchant Center diverso da quello di produzione e dedicato
esclusivamente a questo scopo.

**Inoltre è di fondamentale importanza non impostare ne rivendicare mai
sull'Account di Test l' url del proprio sito web**. **In queste
condizioni infatti tutti gli articoli pubblicati verranno
automaticamente posti in stato "Disapprovato"** e Google non effettuerà
in relazione ad essi nessun tipo di controllo.

Nel momento in cui si tentasse invece di impostare e rivendicare l' url
del proprio sito web (per correggere l'errore visualizzato all'interno
del Merchant Centre) Google avvierà tutte le procedure di validazione
degli articoli presenti all'interno del merchant center, articoli che,
in queste condizioni, dovranno necessariamente soddisfare tutti i
requisiti richiesti da Google stesso (in caso contrario si potrebbe
incorrere anche in una sospensione temporanea dell'account o di tutti
gli annunci legati allo specifico prodotto che non ha superato i test di
validazione).

Un ambiente di test così configurato è comunque sufficiente per testare
il corretto funzionamento dell'integrazione Passweb -- Merchant Center
anche se, per ovvie ragioni, troveremo sempre in relazione alla
pubblicazione di articoli su questo Account determinati errori (come
evidenziato nella figura precedentemente riportata) relativi al fatto ad
esempio di:

- Non aver ancora fornito né rivendicato l' url del sito web collegato
  all'Account

- Non aver sottoposto il prodotto alla fase di revisione

- Non aver impostato per il prodotto un codice gtin (EAN, UPC ...)
  valido

- ...

Ovviamente, alcuni di questi errori verranno automaticamente corretti
nel momento in cui passeremo a pubblicare sull'Account di produzione
(**dove sarà obbligatorio impostare e rivendicare l' url del proprio
sito web**) mentre altri (es. codice gtin non valido) verranno corretti
solo se avremo configurato e valorizzato in maniera adeguata tutti i
campi articolo coinvolti nell'integrazione Passweb -- Merchant Center.

Tornando ora alle informazioni relative ai prodotti pubblicati
all'interno del Merchant Center, occorre fare una precisazione
relativamente alla quantità con cui questi stessi articoli verranno
pubblicati. In questo senso infatti è bene sottolineare che:

**ATTENZIONE!** **Google Merchant per il campo quantità accetta
solamente i due valori \"in stock\" (Disponibile) e \"out of stock\"
(Non Disponibile)**

In conseguenza di ciò nel momento in cui la quantità dell'articolo
pubblicato sul Merchant Center dovesse essere maggiore di 0 (non importa
il valore esatto), in corrispondenza del campo "**disponibilità**"
troveremo il valore "**disponibile**" (in stock)

![](./assets/media/image519.png)

Al contrario nel momento in cui la quantità di pubblicazione dovesse
essere minore o uguale a 0 in corrispondenza dello stesso campo
"**disponibilità**" troveremo il valore "**non disponibile**" (out of
stock)

