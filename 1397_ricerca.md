# RICERCA



Come per Google Analytics anche in questo caso le ricerche interne al
sito potrebbero essere tracciate in maniera automatica attivando
semplicemente la relativa funzionalità in fase di configurazione del
sito su Matomo (parametro "**Ricerca sul sito**" presente nella maschera
"Gestione Misurabili" impostato sul valore "**Tracciamento Ricerca nel
sito abilitato**")

Va detto però che affinché tutto possa funzionare in maniera corretta è
necessario che il sito utilizzi appositi parametri di query string per
gestire le ricerche interne, parametri questi che andranno poi
effettivamente dichiarati anche in fase di configurazione su Matomo.

Il problema in questo senso è rappresentato dal fatto che Passweb non
utilizza parametri di query string per gestire questo tipo di ricerche
(potrebbero, in realtà, essere utilizzati per le ricerche di tipo CMS ma
non per le ricerche di tipo Ecommerce) per cui, l'attivazione del
parametro precedentemente indicato non abiliterebbe, di fatto, per il
nostro sito la registrazione degli eventi di ricerca.

**In definitiva dunque, per un sito Passweb, le ricerche interne al sito
dovranno essere trattate come dei normali eventi e, in queste
condizioni, potranno essere registrate anche nel momento in cui
dovessimo decidere di non abilitare, lato Matomo, il relativo
parametro**

Fatta questa osservazione di fondamentale importanza possiamo ora
analizzare più nel dettaglio la struttura di questo evento e i parametri
ad esso correlati.

**Nome Evento**: trackSiteSearch (corrispondente all'evento "search" di
GA4)

**Requisiti di attivazione**: per attivare l'evento in esame è
necessario verificare:

- di aver attivato il tracciamento standard di Matomo

- di aver selezionato il parametro **Abilita Tracciamento Ricerca**"
  presente alla pagina "**Sito -- Preferenze -- Tracciamento Dati**"
  (sezione "**Matomo -- Client**") del Wizard del proprio sito Passweb

**Generazione dell'evento**: l'evento in esame verrà attivato ogni volta
in cui verrà effettuata una ricerca sul sito utilizzando, per questo, i
relativi componenti presenti nativamente in ogni sito Passweb.

L'attivazione dell'evento in questione determinerà l'invio a Matomo dei
dati ad esso relativi mediante una chiamata del tipo di quella di
seguito indicata:

*\_paq.push(\[\'trackSiteSearch\',*

*\"search_Codice:Prod01A\", //stringa di ricerca nella forma
"searc_nomecomponente: Keywords di ricerca"*

*\"Ricerca Ecommerce\", //Categoria di ricerca*

*false*

*\]);*

dove, come evidenziato, i dati inviati relativamente alla ricerca
effettuata all'interno del sito saranno essenzialmente due:

- **search_nomecomponente: Keyword di ricerca**

> dove
>
> nomecomponente = nome (tutto in minuscolo) assegnato in passweb allo
> specifico componente utilizzato per implementare il campo di ricerca
>
> **ATTENZIONE!** Eventuali spazi presenti nel nome del componente
> verranno sostituiti dal carattere \_
>
> A Matomo verrà quindi inviato un parametro di questo tipo per ciascuno
> dei campi utilizzati (e quindi correttamente valorizzati) per
> effettuare la ricerca. Il valore assunto da questi stessi parametri
> potrà variare, ovviamente, in relazione al tipo di campo utilizzato
> per la ricerca
>
> Nel momento in cui all'interno del pannello di ricerca dovesse essere
> inserito, ad esempio, un componente di tipo "Filtro Checkbox", il
> valore che esso potrà assumere sarà solamente 1 e questo si potrà
> verificare solo se, in fase di ricerca, il check in esame dovesse
> essere effettivamente selezionato
>
> Supponendo dunque di utilizzare un pannello di ricerca di tipo
> Ecommerce con all'interno:

- un componente "Filtro Testo" di nome "Codice"

- un componente "Filtro Checkbox" di nome "Disponibilità"

- un componente "Filtro TreeView" di nome "Categoria Merceologica"

> e di effettuare una ricerca con il check relativo al campo
> "Disponibilità" selezionato e con il campo relativo al "Codice"
> valorizzato con la stringa "prod01A", il corrispondente evento di
> ricerca inviato a Matomo avrà (come nell'esempio sopra indicato) i due
> parametri addizionali

- *search_codice: 'prod01A'*

- *search_disponibilita: 1*

<!-- -->

- **Categoria di Ricerca** valorizzato come Ricerca Ecommerce / Ricerca
  Testuale / Ricerca CMS a seconda della tipologia del componente
  Passweb utilizzato per effettuare la ricerca sul sito

**ATTENZIONE!** Nel momento in cui per effettuare una ricerca interna al
sito dovesse essere utilizzato un pannello contenente 2 o più campi
differenti verrà effettuata una push dell'evento trackSiteSearch per
ogni campo effettivamente valorizzato in fase di ricerca

