# PROTEZIONE



La sezione "**Protezione**" presente nella maschera di configurazione di
ogni singolo Componente Passweb consente di:

- impostare la visibilità del componente a livello di gruppi utente
  potendo quindi decidere quali utenti potranno visualizzare il
  componente e quali no -- sezione "**Protezione Componente sul sito
  (parte Pubblica)**"

- definire specifici filtri articolo e/o specifiche classi custom CSS in
  relazione alle quali poter poi impostare la visibilità del componente
  (solo per determinati componenti) -- sezione "**Protezione Componente
  sul sito (parte Pubblica)**"

- definire chi, fra i vari utenti del Wizard, potrà avere o meno la
  possibilità di gestire il componente -- sezione "**Protezione
  Componente sul Wizard**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_ruoli_res.bmp](./assets/media/image88.png){width="3.9555555555555557in"
height="2.4555555555555557in"}

Nello specifico dunque il parametro:

**Visibile da**: consente di specificare quali utenti potranno
visualizzare il componente e quali no. E' possibile selezionare uno dei
seguenti valori:

- **Tutti:** il componente sarà visibile ed accessibile a tutti i
  visitatori del sito.

- **Solo dai Gruppi:** il componente sarà visibile ed accessibile ai
  soli utenti appartenenti ai gruppi selezionati all'interno del
  parametro "**Gruppi che hanno accesso al componente**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\visibilita_componente_1_res.bmp](./assets/media/image89.png){width="3.9555555555555557in"
height="2.7909722222222224in"}

> Per maggiori informazioni relativamente alla creazione dei Gruppi
> Utente si veda la corrispondente sezione " *Utenti -- Siti Ecommerce
> -- Gruppi Utenti Sito*" di questo manuale.

**Filtro Visibilità Articoli**: consente di impostare uno specifico
filtro articoli che verrà poi valutato per determinare se il relativo
componente dovrà o meno essere visibile.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\visibilita_componente_2_res.bmp](./assets/media/image90.png){width="3.977777777777778in"
height="2.783333333333333in"}

Tale parametro è quindi disponibile, ovviamente, solo per componenti che
sono in qualche modo legati agli articoli pubblicati e venduti
all'interno del sito e che possono quindi essere inseriti all'interno di
componenti di primo livello quali ad esempio il Catalogo Ecommerce, le
Offerte/Novità, la Popolarità Prodotto ecc...

Nello specifico il parametro Filtro Visibilità Articoli sarà disponibile
solo ed esclusivamente per i seguenti componenti:

- **Aggiunta al Carrello**

- **Aggiunta alla Wishlist**

- **Aggiunta al Comparatore**

- **Prezzo**

- **Dati Articolo**

- **Disponibilità**

- **Spedizione**

- **Simulatore Pagamento**

- **Tasse**

**ATTENZIONE!** Una volta impostato, per uno dei componenti sopra
indicati, uno specifico filtro articoli il componente in esame verrà
visualizzato solo ed esclusivamente in corrispondenza di quegli articoli
che soddisfano il filtro stesso. In assenza di filtri il componente sarà
invece sempre visibile indipendentemente da quello che è lo specifico
articolo cui fa riferimento

Il parametro "Filtro Visibilità articoli" potrebbe rivelarsi
particolarmente utile nel momento in cui l'esigenza dovesse essere, ad
esempio, quella di visualizzare sempre all'interno del sito tutti gli
articoli gestiti facendo però in modo che quelli della "Categoria A"
possano essere effettivamente acquistati solo nel caso in cui ad
effettuare l'autenticazione sul sito sia un Agente.

Per gestire questo tipo di situazione sarà quindi necessario inserire
all'interno del componente "Catalogo Ecommerce" due distinti componenti
di "Aggiunta in Carrello" uno visibile solo agli utenti di tipo Agente e
l'altro visibile ai soli utenti di tipo Cliente (agendo in questo senso
dal parametro "Visibile da" precedentemente esaminato).

Sul componente visibile ai soli utenti di tipo Cliente andrà poi
impostato, agendo sul parametro "Filtro Visibilità articoli" un filtro
del tipo di quello indicato in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\visibilita_componente_3_res.bmp](./assets/media/image91.png){width="3.970138888888889in"
height="2.6194444444444445in"}

dove, ovviamente, 107 è il codice della "Categoria A" (per maggiori
informazioni relativamente alla creazione e alla gestione Filtri
Articolo si veda anche la corrispondente sezione di questo manuale
"*Utenti -- Siti Ecommerce -- Gruppi Utenti Sito -- Filtri Utente e
Filtri Articolo -- Filtri Articolo*" di questo manuale.)

In queste condizioni infatti un normale visitatore del sito che non ha
ancora effettuato l'autenticazione non vedrà mai il componente di
"Aggiunta in Carrello" e di fatto pur vedendo tutti gli articoli
presenti sul sito non ne potrà acquistare neppure uno.

Una volta effettuata l'autenticazione essendo un utente di tipo Cliente
gli verrà mostrato il componente di "Aggiunta in Carrello" che abbiamo
impostato come visibile solo a questa particolare tipologia di utenti.
Considerando però il filtro articoli impostato su questo stesso
componente l'utente avrà la possibilità di vedere il componente di
aggiunta in carrello per tutti gli articoli presenti sul sito tranne
quelli che appartengono alla "Categoria A"

In queste stesse condizioni, nel caso in cui ad effettuare
l'autenticazione, dovesse essere invece un Agente (che seleziona poi
ovviamente lo specifico cliente per il quale fare l'ordine) gli verrà
mostrato il componente di "Aggiunta in Carrello" che abbiamo impostato
come visibile solo a questa particolare tipologia di utenti e
considerando che su tale componente non è stato impostato nessun filtro
articoli questo sarà effettivamente visibile per tutti gli articoli
permettendo all'utente di acquistare anche quelli che appartengono alla
"Categoria A".

**Classi visibilità articoli**: consente di impostare una o più classi
CSS in relazione alle quali stabilire la visibilità del componente. Lo
scopo di questo parametro è, sostanzialmente, lo stesso del parametro
"Filtro visibilità articoli" appena esaminato, vale a dire quello di
poter rendere il componente in esame visibile solo per determinati
articoli.

Nel caso precedente il componente era visibile solo per gli articoli che
soddisfacevano il filtro impostato; in questo caso invece il componente
sarà visibile solo per quegli articoli che avranno una delle classi CSS
qui indicate

**ATTENZIONE!** Una volta impostate delle classi CSS all'interno di
questo campo, il componente in esame verrà effettivamente visualizzato
all'interno del sito solo in corrispondenza di quegli articoli che
risultano avere una delle classi CSS indicate.

Al contrario, nel momento in cui il campo in esame dovesse essere
lasciato vuoto il relativo componente sarà sempre visibile
indipendentemente da quelle che potranno essere le classi CSS associate
agli articoli a cui il componente stesso fa riferimento

Per associare ai vari prodotti presenti all'interno del sito determinate
classi CSS custom è possibile utilizzare i campo "**Classi Custom**" e
"**Classi Regole**" presenti nell'anagrafica passweb di ogni singolo
articolo gestito all'interno del sito (per maggiori informazioni in
merito si veda quanto indicato all'interno del capitolo "*Catalogo --
Gestione Articoli -- Articoli -- Anagrafica Articolo / Servizio --
Anagrafica Passweb -- Classi CSS*" di questo manuale)

![Videate\\dati_articolo_classi_custom.bmp](./assets/media/image92.png){width="5.709027777777778in"
height="3.4923611111111112in"}

Ovviamente anche il parametro "Classi visibilità articoli" sarà
disponibile solo per certi componenti. Nello specifico per il
componente:

- **Aggiunta al Carrello**

- **Aggiunta alla Wishlist**

- **Aggiunta al Comparatore**

- **Prezzo**

- **Dati Articolo**

- **Disponibilità**

- **Spedizione**

- **Simulatore Pagamento**

- **Tasse**

- **Contenitore / Contenitore Griglia / Contenitore Colonna -** solo se
  inseriti all'interno di un componente ecommerce di primo livello come
  il Catalogo Ecommerce, la Scheda Prodotto, le Offerte / Novità ecc...

**ATTENZIONE!** considerando che i due parametri "**Filtro visibilità
articoli**" e "**Classi visibilità articoli**" hanno esattamente lo
stesso scopo andrebbero utilizzati in maniera alternativa (o uno o
l'altro)

**In questo senso, tra i due, il consiglio è quello di utilizzare sempre
il parametro "Classi visibilità articoli" perché più performante
rispetto al "Filtro visibilità articoli"** (quest'ultimo infatti
richiede query aggiuntive per poter determinare se il componente in
esame dovrà o meno essere effettivamente visibile in corrispondenza di
ogni singolo prodotto presente nella pagina)

Infine, come precedentemente evidenziato, all'interno della sezione
"**Protezione Componenti sul Wizard**" avremo la possibilità di definire
chi, fra i vari utenti del Wizard, potrà effettivamente gestire lo
specifico componente e chi no.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\protezione_componente_wizard_res.bmp](./assets/media/image93.png){width="3.9625in"
height="2.6041666666666665in"}

In questo senso dunque il parametro:

**Proprietà del componente:** consente di definire chi, fra i vari
utenti del Wizard, potrà avere o meno in gestione lo specifico
componente. Sarà quindi possibile selezionare dal relativo menù a
tendina la tipologia di ruolo (o una combinazione di più tipologie) che
verrà considerata come "proprietario" del Componente.

Tutti gli utenti del Wizard appratenti alla tipologia di ruolo indicata
all'interno di questo campo avranno quindi la possibilità di gestire il
componente in esame secondo quello che è lo schema di permessi ad essa
associato (per maggiori informazioni in merito alla gestione dei Ruoli
Utente si veda anche il relativo capitolo di questo manuale *"Utenti --
Utenti Passweb"*).

**ATTENZIONE!** Il valore impostato a default all'interno di questo
campo dipende da quanto settato per il parametro **"Protezione
Default**" presente, per l'utente attualmente connesso, all'interno
della maschera "**Profilo Utente**" del Wizard

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\profilo_utente_wizard_protezione_default.bmp](./assets/media/image94.png){width="5.790972222222222in"
height="3.5076388888888888in"}

