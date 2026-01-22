# PASSWEB E CLERK



Clerk.io ( [[https://www.clerk.io]{.underline}](https://www.clerk.io) )
è una piattaforma di intelligenza artificiale specializzata nel
potenziare l'esperienza di acquisto degli utenti all'interno di
e-commerce. Utilizza tecniche di **machine learning** per analizzare
dati di navigazione, acquisto e inventario, con l'obiettivo di offrire
**raccomandazioni intelligenti, ricerca avanzata, email marketing
personalizzato e segmentazione dinamica** dei clienti.

![Videate\\clerk_0.bmp](./assets/media/image1.png){width="5.8375in"
height="3.49375in"}

La piattaforma è strutturata in moduli distinti, ciascuno dedicato a una
specifica funzionalità (ricerca, raccomandazioni, email, segmentazione,
chat), che **possono essere attivati e configurati singolarmente in base
alle esigenze del progetto**.

Nonostante la possibilità di utilizzo indipendente, **tutti i moduli
sono progettati per lavorare in sinergia**, condividendo dati
comportamentali e catalogo, al fine di garantire un'esperienza utente
coerente, personalizzata e ottimizzata lungo tutto il percorso
d'acquisto.

Ad esempio:

- I dati raccolti dalla ricerca migliorano le raccomandazioni e possono
  anche influenzare la segmentazione (audience) dei clienti

- Le audience segmentate possono essere usate nelle campagne email
  intelligenti

- Il comportamento di un utente registrato verso le raccomandazioni può
  influenzare i suggerimenti nei risultati di ricerca

- ...

Questa architettura modulare e interconnessa rende Clerk.io una
soluzione scalabile, perfetta sia per e-commerce in fase iniziale sia
per realtà strutturate che vogliono centralizzare le logiche di
personalizzazione e ottimizzazione delle vendite.

Il motore di Clerk.io si basa interamente sui dati raccolti dal sito
e-commerce, che alimentano i suoi algoritmi di intelligenza artificiale
per offrire risultati precisi, personalizzati e rilevanti. La
piattaforma apprende e ottimizza continuamente sulla base di tre flussi
principali di dati:

- **Dati di catalogo** -- prodotti, descrizioni, categorie, varianti,
  disponibilità, attributi personalizzati ...

- **Dati comportamentali** -- ricerche, click, visualizzazioni di
  prodotti, aggiunte al carrello, ordini effettuati ...

- **Dati cliente** -- segmenti, preferenze, storico di navigazione e
  acquisto ...

Ovviamente, per funzionare in modo ottimale, Clerk.io ha bisogno di
ricevere un flusso completo, coerente e aggiornato di questi dati. Più
informazioni vengono inviate alla piattaforma, più il sistema potrà:

- Migliorare la precisione delle raccomandazioni

- Restituire risultati di ricerca più pertinenti

- Creare segmentazioni clienti più intelligenti

- Personalizzare in modo efficace le email e i suggerimenti

- Consentire alla chat di dare risposte più coerenti e veritiere

- ...

Per maggiori informazioni relativamente a come poter condividere con
Clerk i dati di cui ha bisogno si veda quanto indicato nel successivo
capitolo "*Integrazione -- Sincronizzazione Dati*" di questo manuale.

Va da sé che dovendo comunque condividere tutta una serie di dati del
proprio ecommerce con una piattaforma terza, un punto fondamentale di
tutto il processo sarà ovviamente la conformità al GDPR.

Sotto questo punto di vista uno dei principali vantaggi offerti da
Clerk, oltre al fatto di avere i server localizzati in Europa (nello
specifico in Germania con backup in Irlanda) è quello di poter
utilizzare, a default, un sistema di tracciamento completamente
cookieless e dati pseudonimizzati.

Oltre a questo poi, in fase di configurazione, è comunque prevista anche
la possibilità di memorizzare i dati in maniera persistente in modo tale
da ottenere una profilazione degli utenti più precisa e utilizzare così
al meglio le opportunità di marketing offerte dalla piattaforma.

**ATTENZIONE! in ogni caso anche nel momento in cui si dovesse decidere
di utilizzare Clerk nella sua modalità cookieless, attivando magari solo
il modulo di ricerca e/o quello delle raccomandazioni sarà comunque
necessario fornire nella Privacy Policy del sito, un'informativa
adeguata circa l'utilizzo di questa piattaforma e dei dati che con essa
vengono raccolti**

In questo senso potrebbe quindi essere necessario:

- Indicare chiaramente nella privacy policy del sito il trattamento di
  dati pseudonimi

- Avere una base giuridica documentata tramite una valutazione di
  legittimo interesse (LIA)

- Prevedere per gli utenti del sito un' opzione di opt-out che, se
  esercitata, disattivi completamente tutti i moduli Clerk, compresa
  ricerca e raccomandazioni

- ...

**ATTENZIONE! Per maggiori informazioni relativamente all'utilizzo di
Clerk in maniera conforme al GDPR, e in relazione anche allo specifico
utilizzo che se ne fa all'interno del proprio sito, si consiglia
comunque di fare sempre riferimento alla relativa documentazione
(<https://help.clerk.io/it/platform/company/gdpr/>) e/o all'assistenza
di Clerk oltre che, ovviamente, al proprio legale / DPO**

Per maggior informazioni relativamente invece a come la configurazione
dell'integrazione tra Passweb e Clerk possa impattare in un modo
piuttosto che in un altro dal punto di vista del GDPR (sistema
cookieless o salvataggio dei dati di tracciamento in local storage,
pseudonimizzazione dei dati, raccolta e invio di indirizzi mail ...) si
veda anche quanto indicato all'interno del relativo capitolo ("*Passweb
e Clerk -- Privacy e GDPR*") di questo manuale.

**Si ricorda infine che lo scopo di questo manuale non è quello di
fornire una guida dettagliata all'utilizzo di Clerk che rimane comunque
uno strumento di terze parti e che, per poter essere utilizzato al
meglio, richiede specifiche conoscenze**.

In tal senso il consiglio è dunque quello di rivolgersi sempre alla
documentazione (<https://help.clerk.io/it/>) ufficiale e al relativo
supporto tecnico

