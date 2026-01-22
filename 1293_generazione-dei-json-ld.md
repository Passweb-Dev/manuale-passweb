# GENERAZIONE DEI JSON-LD



A differenza dei microdati che, come noto, sono inglobati nel markup
HTML e che proprio per questo non richiedono query aggiuntive oltre a
quelle necessarie per costruire la pagina stessa, i JSON-LD tendono
invece a separare le informazioni presenti al loro interno da quello che
è il markup HTML della pagina.

In conseguenza di ciò nel momento in cui si dovesse scegliere di
generare il JSON-LD in maniera dinamica, nello stesso momento cioè in
cui viene generata la pagina web, questo richiederebbe indubbiamente
l'esecuzione di query aggiuntive necessarie per ottenere i
corrispondenti dati strutturati con conseguente aumento dei tempi di
caricamento della pagina web.

Per evitare questo tipo di problemi in Passweb si è scelto di generare i
JSON-LD, secondo le impostazioni settate all'interno della pagina
"**Preferenze sito**" del Wizard (tab "**Integrazioni**", sezione
"**Dati Strutturati**") ma in maniera diversa a seconda del fatto di
considerare il JSON-LD delle briciole di pane (Schema BreadcrumbList)
piuttosto che quello dei prodotti (Schema Product).

Nello specifico infatti:

- **il JSON-LD delle briciole** **di pane** verrà creato in maniera
  dinamica nello stesso momento in cui viene costruita la pagina web.
  Per poterlo generare sarà quindi sufficiente attivare il relativo
  check (Schema BreadcrumbList) presente all'interno della sezione
  "Schema Ecommerce" e assicurarsi di aver gestito all'interno della
  pagina il Componente Passweb "Info navigazione"

- **il JSON-LD dei prodotti** verrà invece generato da un processo
  asincrono che può essere eseguito:

  - in relazione a tutti i prodotti gestiti sul sito, in maniera manuale
    cliccando sul pulsante "**Generazione JsonLD prodotti**"

> **ATTENZIONE!** il pulsante "Generazione JsonLD prodotti" avvia il
> processo di creazione del JSON-LD per tutti i prodotti attualmente
> gestiti sul sito. Tale processo potrebbe quindi richiedere diverso
> tempo in relazione al numero effettivo di prodotti da processare.
> L'amministratore del sito verrà avvisato mediante un'apposita mail al
> termine del processo

- a seguito di un import via csv dei dati articolo dal Wizard di Passweb
  (anche in questo caso in relazione a tutti i prodotti gestiti sul
  sito)

- in maniera automatica alla sincronizzazione in relazione però ai soli
  prodotti variati

- in maniera automatica al salvataggio, sul Wizard, di una specifica
  Anagrafica Articolo Passweb in relazione, però, soltanto a quello
  specifico prodotto

> **ATTENZIONE!** L'unica proprietà del JSON-LD che verrà creata sempre
> e comunque in maniera dinamica, nello stesso momento cioè in cui viene
> generata anche la pagina web, è quella relativa al prezzo

In questo modo dunque il JSON-LD dei prodotti verrà creato, di fatto,
prima della visualizzazione della pagina web, verrà inserito nel
database del sito, potrà essere visualizzato anche all'interno del
Wizard in corrispondenza del campo "**JsonLD Product**" presente
nell'anagrafica Passweb dell'articolo (tab "**Descrizioni**")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\json_ld_prdoduct_anagrafica_passweb.bmp](./assets/media/image31.png){width="5.532638888888889in"
height="3.415277777777778in"}

e, soprattutto, avrà un impatto minimo sui tempi di caricamento della
pagina web.

In considerazione di quanto appena detto è bene evidenziare quindi che
il pulsante "**Generazione JsonLD prodotti**" andrebbe utilizzato:

- subito dopo aver effettuato la prima configurazione della struttura di
  JSON-LD da utilizzare all'interno del sito, in maniera tale da essere
  certi di inserire i relativi dati strutturati in tutte le pagine
  prodotto

- nel caso in cui dovessero essere apportate delle variazioni alla
  struttura dei JSON-LD precedentemente in uso al sito (es. aggiunta o
  rimozione di proprietà standard o custom) in maniera tale poter
  aggiornare correttamente i dati strutturati di tutte le pagine
  prodotto secondo quella che è la nuova configurazione

- nel caso in cui si dovesse decidere di apportare delle variazioni, in
  maniera massiva (import di file csv) ai valori di eventuali Attributi
  Articolo Passweb inseriti (tramite Json Builder) nella struttura dei
  JSON-LD in uso al sito

- in qualsiasi altro caso in cui l'esigenza dovesse essere quella di
  ricreare da zero i dati strutturati di tutte le pagine prodotto

In tutti gli altri casi, una volta effettuata la prima creazione dei
JSON-LD dei prodotti gestiti sul sito, sarà poi Passweb a preoccuparsi
di rigenerare in maniera automatica, ad ogni sincronizzazione, i dati
strutturati di quei prodotti che dovessero risultare nuovi o variati
rispetto all'ultima sincronizzazione effettuata.

