# MULTILINGUA



Nel momento in cui il sito Passweb da integrare con Clerk dovesse essere
multilingua la strada migliore da seguire, come indicato direttamente
anche nella relativa documentazione di prodotto
(<https://help.clerk.io/it/integrations/any-webshop/data-feeds/> -
sezione Multi-lingua), è quella che prevede di gestire all'interno di
Clerk Store distinti per ogni singola lingua. Questo per due diverse
ragioni:

- il fatto di poter impostare in maniera specifica la lingua di gestione
  direttamente in fase di configurazione dello Store (campo
  "**Language**")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\clerk_parametri_configurazione_store.bmp](./assets/media/image22.png){width="5.428472222222222in"
height="3.33125in"}

> farà si che la ricerca possa poi comprendere molto meglio eventuali
> errori grammaticali e di ortografia rendendo quindi i risultati più
> pertinenti e corretti anche in presenza di questi errori

- tipicamente clienti di paesi diversi tenderanno ad avere preferenze,
  comportamenti e schemi di ricerca diversi oltre che ad acquistare
  anche tipologie di prodotti differenti per cui, anche in questo caso,
  il fatto di creare uno store distinto per ogni singolo paese
  (separando di conseguenza, ad esempio, ordini e tracciamento degli
  utenti italiani, rispetto ad ordini e tracciamento degli utenti
  francesi piuttosto che di quelli spagnoli) permetterà a Clerk, anche
  in questo caso, di fornire effettivamente ai diversi utenti risultati
  più coerenti e pertinenti in relazione anche al loro paese di
  appartenenza

Ovviamente il fatto di configurare e gestire su Clerk Store distinti per
lingua comporterà, dall'altra parte, il fatto di dover gestire e
configurare anche su Passweb un Account di integrazione diverso per ogni
singolo Store presente su Clerk indicando, in fase di configurazione
dell'Account stesso (campo "**Lingua**"), la lingua di gestione dello
Store con cui ci svuole collegare

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\account_clerk_passweb_lingua.bmp](./assets/media/image23.png){width="5.428472222222222in"
height="3.33125in"}

**ATTENZIONE!** E' possibile creare un solo account per ogni lingua
gestita

In questo modo ordini e clienti condivisi con Clerk verranno smistati,
in base alla loro lingua, sul relativo store e, nel caso in cui
dovessero esserci ordini o clienti con associata una lingua diversa da
quelle gestite (per cui dunque non è stato impostato né uno store Clerk
né il corrispondente account all'interno di Passweb) questi verranno
automaticamente assegnati allo store di default (campo "**Account di
default**").

In maniera più precisa dunque, posto di aver configurato tutto
correttamente, nel caso di siti multilingua i vari diversi dati verranno
smistati sui singoli store secondo quanto di seguito indicato:

- **Il feed ordini** verrà generato tenendo in considerazione la Nazione
  selezionata dall'utente in fase di registrazione al sito (o quella
  eventualmente associata nella sua anagrafica gestionale nel caso in
  cui l'utente dovesse essere stato importato direttamente da Mexal).
  Dalla Nazione verrà poi ricavata la lingua e in base alla lingua
  l'ordine verrà inserito nel feed di uno store piuttosto che in un
  altro.

> I dati degli ordini inviati via API seguiranno, ovviamente, la stessa
> logica

- **Il feed clienti**, allo stesso modo del feed ordini, verrà generato
  tenendo in considerazione la Nazione selezionata dall'utente in fase
  di registrazione al sito (o quella eventualmente associata nella sua
  anagrafica gestionale nel caso in cui l'utente dovesse essere stato
  importato direttamente da Mexal). Dalla Nazione verrà poi ricavata la
  lingua e in base alla lingua il cliente verrà inserito nel feed di uno
  store piuttosto che in un altro

> I dati dei clienti inviati via API (in fase di registrazione e/o di
> variazione del profilo) seguiranno, ovviamente, la stessa logica

- **Il feed delle categorie** conterrà, indipendentemente dallo store
  considerato, sempre e comunque tutte le categorie merceologiche
  attualmente gestite all'interno del sito.

> Nel caso dei siti multilingua però i campi presenti all'interno del
> feed (es. "nome categoria") verranno valorizzati nella lingua
> impostata in fase di configurazione del relativo account Clerk

- **Il feed degli articoli** conterrà, indipendentemente dallo store
  considerato, sempre e comunque tutti i prodotti oggetto dell'eventuale
  filtro impostato in fase di configurazione del feed stesso.

> Nel caso dei siti multilingua però i campi presenti all'interno del
> feed (es. "nome categoria") verranno valorizzati nella lingua
> impostata in fase di configurazione del relativo account Clerk

- **Il feed dele pagine articoli** conterrà, indipendentemente dallo
  store considerato, sempre e comunque tutti i testi marcati per essere
  inseriti in questo stesso feed e tutti i post cms effettivamente
  pubblicati all'interno del sito

> Nel caso dei siti multilingua però i campi presenti all'interno del
> feed (es. "text") verranno valorizzati nella lingua impostata in fase
> di configurazione del relativo account Clerk

