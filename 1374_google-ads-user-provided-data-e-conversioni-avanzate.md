# GOOGLE ADS USER PROVIDED DATA E CONVERSIONI AVANZATE



Le conversioni avanzate per il web sono una funzionalità che può
migliorare la precisione della misurazione delle conversioni e
l'efficacia delle offerte integrando i tag di conversione esistenti con
dati proprietari dei clienti (es. indirizzo email) opportunamente
sottoposti ad hashing unidirezionale.

Di base il funzionamento di queste conversioni è piuttosto semplice:
quando un cliente completa una conversione all'interno del sito, posto
ovviamente che questo stesso cliente abbia prestato in maniera
preventiva tutti i consensi del caso a livello di privacy e GDPR, il
sistema di tracciamento si preoccuperà di acquisire alcuni dati di prima
parte di questo cliente (sostanzialmente indirizzo mail, nome, cognome /
ragione sociale, numero di telefono, indirizzo di casa), di hasharli in
maniera unidirezionale (in modo tale cioè che non possano essere
successivamente decodificati) e di inviarli poi a Google (nello
specifico a Google Analytics piuttosto che a Google Ads) che li
utilizzerà per abbinare l'utente a un click precedente su di un
annuncio.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\google_ads_ec_1.bmp](./assets/media/image1.png)

Per comprendere quanto questo sistema di gestione, che in buona sostanza
consente di identificare un utente mediante un indirizzo mail, possa
essere effettivamente più efficace rispetto al sistema di gestione
"standard" che prevede di identificare l'utente in base ai valori
presenti in un cookie del suo browser, basta pensare a quante volte
quello stesso utente potrà cambiare il suo indirizzo mail, rispetto a
quante volte invece potrà svuotare i cookie del suo browser o, molto più
banalmente, rispetto a quante volte potrà utilizzare un browser o un
dispositivo diverso!

In considerazione di ciò i principali vantaggi che si possono ottenere
implementando questo tipo di conversioni sono:

- **Maggiore osservabilità delle conversioni**: recupero delle
  conversioni perse e osservazione di nuove conversioni grazie ai dati
  di prima parte.

- **Miglioramento del bidding e dell'attribuzione**: dati di qualità
  superiore migliorano i modelli di bidding e attribuzione.

- **Incremento delle performance**: tassi di conversione migliori e
  maggiore efficienza dei costi.

- **Rispetto della privacy** mediante l\'hashing dei dati proprietari
  dei clienti

Detto che lo scopo di questo manuale non è certamente quello di
analizzare nel dettaglio il funzionamento delle conversioni avanzate di
Google Ads né tanto meno quello di spiegare il funzionamento dello
strumento Google Ads in sé, e che per questo si consiglia di fare sempre
riferimento alla relativa documentazione disponibile in rete fornita
direttamente da Google (es.
<https://support.google.com/google-ads/answer/9888656> ), nei successivi
capitoli di questo manuale vedremo rapidamente come poter attivare,
all'interno del proprio account di Google Ads, la gestione delle
conversioni avanzate in relazione anche alle diverse modalità attraverso
cui un sito Passweb può inviare ad Ads stesso i dati di prima parte
degli utenti (tracciamento diretto o tracciamento mediante Google Tag
Manager).

