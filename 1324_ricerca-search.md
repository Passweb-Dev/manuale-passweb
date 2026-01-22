# RICERCA -- SEARCH



Come evidenziato all'interno del capitolo "*Google Analytics 4 --
Universal Analytics e GA4 Principali Differenze -- Data Model e Gestione
degli Eventi*" in GA4 le ricerche interne al sito sono trattate come
"**Eventi di misurazione avanzata (Enanched Measurement)**" per cui, di
base, potrebbero essere tracciate semplicemente attivando e configurando
in maniera corretta, nel relativo Data Stream, questo tipo di evento.

Va detto però che affinché tutto possa funzionare in maniera corretta è
necessario che il sito utilizzi appositi parametri di query string per
gestire le ricerche interne, parametri questi che andranno poi
effettivamente dichiarati anche in fase di configurazione dell'evento
(posto che non coincidano già con quelli riconosciuti automaticamente da
GA4).

Il problema in questo senso è rappresentato dal fatto che Passweb non
utilizza parametri di query string per gestire questo tipo di ricerche
(potrebbero, in realtà, essere utilizzati per le ricerche di tipo CMS ma
non per le ricerche di tipo Ecommerce) per cui, l'attivazione del
corrispondente evento di misurazione avanzata non abiliterebbe, di
fatto, per il nostro sito la registrazione degli eventi di ricerca.

**In definitiva dunque, per un sito Passweb, le ricerche interne al sito
dovranno essere trattate come dei normali eventi e, in queste
condizioni, potranno essere registrate anche nel momento in cui
dovessimo decidere di non abilitare il corrispondente evento di
misurazione avanzata**

Fatta questa osservazione di fondamentale importanza possiamo ora
analizzare più nel dettaglio la struttura di questo evento e i parametri
ad esso correlati.

**Nome Evento**: search

**Requisiti di attivazione**: per attivare l'evento in esame è
necessario verificare di aver correttamente attivato il tracciamento
standard collegato ad una proprietà GA4 e aver selezionato il parametro
"**Google Analytics Ricerca sul Sito**" presente alla pagina "**Sito --
Preferenze**" del Wizard (tab "**Tracciamento Dati**")

**Generazione dell'evento**: l'evento in esame verrà attivato ogni volta
in cui verrà effettuata una ricerca sul sito utilizzando, per questo, i
relativi componenti presenti nativamente in ogni sito Passweb

L'attivazione dell'evento in questione determinerà l'invio ad analytics
dei dati e dei parametri ad esso correlati mediante una chiamata del
tipo di quella di seguito indicata:

*gtag('event', 'search',*

*{*

*search_category: 'Ricerca ECommerce',*

*search_Codice: 'prod01A',*

*search_Disponibilita: 1,*

*value: 1,*

*dateTime:'11/10/2022, 14:54:56'*

*});*

dove i parametri correlati all'evento verranno valorizzati come di
seguito indicato:

- **search_category:** Ricerca Ecommerce / Ricerca Testuale / Ricerca
  CMS

> **ATTENZIONE!** il parametro search_category assumerà uno dei tre
> valori sopra indicati in base alla tipologia del componente utilizzato
> per effettuare la ricerca sul sito

![](./assets/media/image20.png)

- **search_Nome_Tracciamento:** valore utilizzato per la ricerca

> dove
>
> **Nome_Tracciamento** coincide esattamente con quanto inserito nella
> maschera di configurazione del relativo componente di ricerca in
> corrispondenza del campo "Nome Tracciamento" (il tutto riportato in
> minuscolo)

![](./assets/media/image21.png)

> **ATTENZIONE!** Eventuali spazi presenti all'interno del campo
> evidenziato in figura verranno sostituiti dal carattere \_
>
> Nel momento in cui il campo in esame dovesse essere lasciato vuoto, al
> suo posto verrà utilizzato il nome (tutto in minuscolo) assegnato al
> componente
>
> A Google Analytics verrà quindi inviato un parametro di questo tipo
> per ciascuno dei campi utilizzati (e quindi correttamente valorizzati)
> per effettuare la ricerca. Il valore assunto da questi stessi
> parametri potrà variare, ovviamente, in relazione al tipo di campo
> utilizzato per la ricerca
>
> Nel momento in cui all'interno del pannello di ricerca dovesse essere
> inserito, ad esempio, un componente di tipo "Filtro Checkbox", il
> valore che esso potrà assumere sarà solamente 1 e questo si potrà
> verificare solo se, in fase di ricerca, il check in esame dovesse
> essere effettivamente selezionato
>
> Supponendo dunque di utilizzare un pannello di ricerca di tipo
> Ecommerce con all'interno:

- un componente "Filtro Testo" con "Nome Tracciamento = Codice"

- un componente "Filtro Checkbox" con "Nome Tracciamento =
  Disponibilità"

- un componente "Filtro TreeView" con "Nome Tracciamento = Categoria
  Merceologica"

> e di effettuare una ricerca con il check relativo al campo
> "Disponibilità" selezionato e con il campo relativo al "Codice"
> valorizzato con la stringa "prod01A", il corrispondente evento
> "*search*" inviato a GA4 avrà (come nell'esempio sopra indicato) i due
> parametri addizionali

- *search_codice: 'prod01A'*

- *search_disponibilita: 1*

<!-- -->

- **value:** 1 (valore di Default) oppure il valore personalizzato
  impostato per il parametro "**GA4 -- search**" presente alla pagina
  "***Sito Preferenze***" del Wizard, tab "***Tracciamento Dati***"
  sezione "***Parametro Value eventi Analytics e Tag Manager***". Per
  maggiori informazioni in merito si veda anche quanto indicato
  all'interno del relativo capitolo di questo manuale ("*Sito --
  Preferenze -- Tracciamento Dati*")

- **dateTime:** data e ora in cui si è verificato l'evento

**ATTENZIONE!** la chiamata ed i parametri sopra indicati sono validi
solo ed esclusivamente nel momento in cui l'evento di ricerca venga
tracciato lato client

Nel caso in cui si dovesse invece decidere di tracciare l'evento di
ricerca lato server questo determinerà l'invio ad analytics dei dati e
dei parametri ad esso correlati mediante una chiamata del tipo di quella
di seguito indicata:

*gtag('event', 'search',*

*{*

*search_term:*
*\[{"campo":"search_componenteRicercaText","valore2":"PROD63B"}\]*

*value: 1,*

*dateTime:'11/10/2022, 14:54:56'*

*});*

dove i parametri correlati all'evento verranno valorizzati come di
seguito indicato:

- **search_term**: lista dei valori presenti nei campi di ricerca del
  relativo pannello. Per ogni campo valorizzato in fase di ricerca verrà
  inserita la coppia "**chiave -- valore**" dove:

> **chiave = search_Nome_Campo** -- coincide esattamente con quanto
> inserito nella maschera di configurazione del relativo componente di
> ricerca in corrispondenza del campo "Nome Tracciamento" (il tutto
> riportato in minuscolo)

![](./assets/media/image21.png)

> **ATTENZIONE!** Eventuali spazi presenti all'interno del campo
> evidenziato in figura verranno sostituiti dal carattere \_
>
> Nel momento in cui il campo in esame dovesse essere lasciato vuoto, al
> suo posto verrà utilizzato il nome (tutto in minuscolo) assegnato al
> componente
>
> **valore** = valore inserito nel relativo campo di ricerca -- Anche in
> questo caso, ovviamente, il valore effettivamente passato ad Analytics
> potrà variare in relazione al tipo di campo utilizzato per la ricerca

