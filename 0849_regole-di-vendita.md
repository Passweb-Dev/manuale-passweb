# REGOLE DI VENDITA



Il pulsante **Regole di Vendita** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_regole_vendita.bmp](./assets/media/image116.png) ) presente nella parte alta della
maschera "**Gestione Liste di Vendita"** accessibile dalla voce di menu
***"Catalogo -- Amazon"***, consente di visualizzare e gestire tutte le
Regole di Vendita attualmente codificate, oltre che ovviamente di
crearne di nuove.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\lista_regole_vendita_amazon.bmp](./assets/media/image271.png)

Ciascuna delle Regole presenti all'interno di questa sezione potrà
essere associata ad una o più Liste di Vendita e permetterà di fare in
modo che, nel momento in cui dovessero essere aggiunti nuovi articoli
alle Categorie Merceologiche indicate in fase di creazione della Regola
stessa, tali articoli possano poi essere aggiunti automaticamente anche
alla Lista di vendita collegata.

Il campo di ricerca attivabile cliccando sulla lente di ingrandimento,
presente in testata in corrispondenza della colonna Nome, consente di
filtrare i dati in griglia sulla base dei valori presenti all'interno
della colonna stessa.

Una volta impostato un filtro di ricerca, per poterlo poi eliminare sarà
sufficiente cliccare sull'icona raffigurante una piccola lente di
ingrandimento con un -- all'interno (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_elimina_filtro.bmp](./assets/media/image69.png) ) che comparirà in testata alla colonna
in corrispondenza della quale è stato impostato il filtro stesso.

Infine è anche possibile ordinare, in maniera crescente e/o decrescente,
gli elementi in griglia cliccando semplicemente sull'icona raffigurante
due piccole frecce (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_ordinamento_griglia.bmp](./assets/media/image70.png) )

I pulsanti presenti nella contestuale barra degli strumenti consentono
rispettivamente di:

- **Elimina Regola di Vendita** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_elimina_regola_vendita.bmp](./assets/media/image159.png) ): consente di eliminare la Regola di vendita
  attualmente selezionata in elenco.

> **ATTENZIONE!** E' possibile eliminare una Regola di Vendita solo se
> non associata ad alcuna Lista

- **Modifica Regola di Vendita** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_modifica_regola_vendita.bmp](./assets/media/image160.png) ): consente di modificare le
  caratteristiche della Regola di vendita attualmente selezionata in
  elenco.

- **Aggiungi Regola di Vendita** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_aggiungi_regola_vendita.bmp](./assets/media/image160.png) ): consente di creare una nuova Regola
  di vendita

In particolare cliccando su quest'ultimo pulsante verrà visualizzata la
maschera "**Dati Regola di Vendita**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\crea_regola_vendita.bmp](./assets/media/image272.png)

all'interno della quale poter indicare le specifiche della Regola che si
intende codificare.

Nello specifico sarà quindi possibile indicare un valore per i seguenti
parametri:

**Nome:** consente di assegnare un nome alla Regola di Vendita che si
sta realizzando

**Filtro articoli:** consente di impostare un Filtro Articoli mediante
il quale poter individuare i prodotti che dovranno poi essere
automaticamente aggiunti alle Liste di Vendita che utilizzeranno la
Regola in esame (per maggiori informazioni relativamente alla gestione
dei filtri articolo si veda anche quanto indicato all'interno del
capitolo "*Utenti -- Siti Ecommerce -- Gruppi Utente Sito -- Filtri
Utente e Filtri Articolo -- Filtri Articolo*" di questo manuale)

**ATTENZIONE**! L'aggiunta automatica, alla lista di vendita, degli
articoli che soddisfano il filtro potrà avvenire in due diversi momenti:

- al salvataggio della lista di vendita

- a seguito di una sincronizzazione sito -- gestionale in cui si
  dovessero individuare articoli nuovi e/o variati (lato gestionale o
  lato Passweb) che soddisfano il filtro impostato

Gli articoli aggiunti automaticamente potranno poi essere identificati,
rispetto a quelli aggiunti in maniera manuale, dal bordo grigio della
relativa riga (gli articoli aggiunti manualmente avranno invece un bordo
azzurro) oltre che dal valore presente nella corrispondente colonna
della tabella (quella identificata dall'icona
![Videate\\colonna_aggiunta_automatica.bmp](./assets/media/image133.png) )

![Videate\\liste_vendita_aggiunta_automatica_articoli.bmp](./assets/media/image250.png)

**ATTENZIONE! Gli articoli aggiunti automaticamente ad un lista di
vendita non possono essere gestiti in maniera manuale. Ciò significa
dunque che questi stessi articoli potranno, eventualmente, essere
eliminati dalla lista di vendita solo nel momento in cui non dovessero
più soddisfare il filtro impostato**.

Un'ultima cosa di fondamentale importanza da tenere sempre in
considerazione è che se un articolo aggiunto, inizialmente, alla lista
di vendita in maniera manuale dovesse, ad un certo punto, soddisfare un
eventuale filtro di aggiunta da quel momento in avanti verrà trattato
esattamente come tutti gli altri articoli aggiunti in maniera
automatica.

**Aggiunta di un articolo alla Lista di Vendita**: consente di indicare
l'azione da eseguire nel momento in cui dovessero esserci nuovi articoli
e/o articoli variati (lato gestionale o lato Passweb) rispetto
all'ultima sincronizzazione, che soddisfano il filtro impostato e che
dovrebbero quindi essere aggiunti alla lista in esame

E' possibile selezionare uno dei seguenti valori:

- **Nessuna Azione**: in questo caso, se anche a seguito di una
  sincronizzazione sito -- gestionale dovessero esserci nuovi articoli
  e/o articoli variati (lato gestionale o lato Passweb), che soddisfano
  il filtro impostato mediante il precedente parametro, non verrà
  comunque eseguita nessuna azione e, di fatto, non verrà quindi
  aggiunto alla lista di vendita nessun nuovo prodotto

> Eventuali muovi articoli dovranno quindi essere inseriti nella Lista
> di Vendita in maniera manuale

- **Aggiungi nella Lista di Vendita**: selezionando questa opzione se, a
  seguito di una sincronizzazione sito -- gestionale, dovessero esserci
  nuovi articoli e/o articoli variati (lato gestionale o lato Passweb)
  che soddisfano il filtro impostato, questi stessi articoli verranno
  automaticamente aggiunti alla Lista di Vendita e, volendo, potrebbero
  anche essere automaticamente pubblicati all'interno della relativa
  piattaforma.

**Rimozione di un articolo**: consente di indicare l'azione da eseguire
nel momento in cui dovessero essere rimossi degli articoli da Passweb o
dovessero esserci articoli variati (lato gestionale o lato Passweb)
rispetto all'ultima sincronizzazione, che non soddisfano più il filtro
impostato e che dovrebbero quindi essere rimossi dalla lista in esame

E' possibile selezionare uno dei seguenti valori:

- **Nessuna Azione**: in questo caso, se a seguito di una
  sincronizzazione sito -- gestionale dovessero essere rimossi da
  Passweb determinati articoli che prima erano stati inseriti nelle
  lista di vendita, questi verranno ovviamente eliminati anche dalla
  lista stessa ma non verranno arrestati sul corrispondente marketplace.

> Se invece, a seguito di una sincronizzazione sito -- gestionale
> dovessero esserci articoli variati (lato gestionale o lato Passweb)
> inseriti in lista e che non rispettano più il filtro impostato
> mediante il precedente parametro, non verrà eseguita, in relazione a
> tali articoli, nessuna azione e, di fatto, questi non verranno quindi
> né eliminati dalla lista né tanto meno verranno arrestati sul
> corrispondente marketplace.

- **Arresto dell'articolo dal Marketplace**: in questo caso se a seguito
  di una sincronizzazione sito -- gestionale dovessero essere rimossi da
  Passweb determinati articoli che prima erano stati inseriti nelle
  lista di vendita o se, allo stesso modo dovessero esserci articoli
  variati (lato gestionale o lato Passweb) che non rispettano più il
  filtro impostato, questi verranno prima arrestati sul corrispondente
  marketplace e poi rimossi dalla lista di vendita

**ATTENZIONE! in ogni caso indipendentemente da come si deciderà di
impostare il parametro "Rimozione di un articolo" Passweb non andrà mai
a eliminare articoli pubblicati sul corrispondente marketplace
limitandosi, al massimo, ad eseguire su di essi l'azione di "Arresto"**

**Considera gli articoli come già in vendita:** consente, se abilitato,
di porre **tutti i nuovi articoli** aggiunti alla lista di vendita che
utilizza la regola in esame, nello stato di "**In attesa di aggancio**"
rendendoli di fatto sensibili alle regole di "Rimessa in vendita"

**ATTENZIONE!** Lo stato "**In attesa di aggancio**" può essere gestito
solo ed esclusivamente a livello di intera Lista di Vendita. Non sarà
quindi possibile trovare articoli in questo stato all'interno di una
lista per cui non sia stato attivato il parametro "**Considera gli
articoli come in vendita**"

Tipicamente il parametro in esame dovrà essere attivato nel momento in
cui si dovessero agganciare articoli già presenti sul marketplace (ma
non pubblicati tramite Passweb) mediante l'applicazione di una regola di
Modifica in Vendita.

E' chiaro dunque che se l'esigenza dovesse essere quella di agganciare
un articolo già presente sul marketplace ma non pubblicato da Passweb
mediante una regola di modifica in vendita, questo stesso articolo
dovrebbe prima di tutto essere pubblicato tramite Passweb tramite
l'applicazione di una regola di pubblicazione o tramite una
pubblicazione manuale. Solo a questo punto infatti il prodotto potrebbe
poi essere modificato mediante una regola di modifica in vendita.

Lo stato "In attesa di aggancio" consente di saltare tutti questi
passaggi considerando, da subito, l'articolo come già presente sul
marketplace (anche se non pubblicato inizialmente da Passweb) e quindi
immediatamente sensibile all'applicazione di una eventuale regola di
modifica in vendita

**ATTENZIONE!** eventuali modifiche apportate ai parametri di
configurazione di una Regola di Vendita avranno effetto su tutte le
Liste collegate alla Regola stessa

