# CONSENT MODE BASE



La modalità **Base** rappresenta l'approccio più restrittivo e semplice
di implementazione della Consent Mode. Offre la massima garanzia che
nessun dato venga raccolto senza consenso (è quindi ideale per chi
privilegia la massima tutela della privacy), ma sacrifica precisione e
quantità dei dati disponibili per le analisi del comportamento degli
utenti e per l'ottimizzazione delle campagne pubblicitarie.

In questo scenario infatti, i tag e gli script di tracciamento di Google
**non vengono caricati affatto finché l'utente non interagisce con il
banner di consenso** della CMP in uso al sito fornendo un'esplicita
preferenza.

Ciò significa che, prima di quell'interazione, non viene inviata alcuna
richiesta ai server di Google, non viene trasmesso alcun dato e non
viene comunicato nemmeno lo stato del consenso.

Una volta che l'utente dovesse poi accettare fornendo i relativi
consensi al tracciamento, i tag e gli script verranno caricati ed
eseguiti "in maniera tradizionale" salvando sul browser dell'utente i
relativi cookie e iniziando quindi a registrare eventi e a raccogliere
dati come previsto.

Nel momento in cui l'utente dovesse negare i consensi rifiutando il
tracciamento tutto resterebbe invece bloccato e a Google non verrebbe
mai inviato alcun tipo di dato (neppure i cosiddetti cookiless pings)

**ATTENZIONE!** con la Consent Mode Base durante il periodo in cui
l'utente non ha ancora scelto o ha rifiutato, nessun dato viene raccolto
né utilizzato per modellare conversioni o traffico.

Dal punto di vista tecnico, questa modalità è molto molto più semplice
da configurare. E' sufficiente infatti collegare il banner di consenso
della CMP in uso al sito in modo che carichi o meno i tag e gli script
di tracciamento in base alla scelta dell'utente.

In queste condizioni dunque nel flusso di gestione della Consent Mode
Base il primo script ad essere caricato è proprio quello di attivazione
e gestione del cookie banner della CMP (quello che con la Consent Mode
Avanzata veniva invece caricato per ultimo).

Successivamente verranno poi caricati gli script relativi
all'inizializzazione dei consensi e al tracciamento di Google Analytics
che, venendo comunque dopo lo script della CMP, risulteranno bloccati e,
di fatto, non invieranno quindi alcun dato a Google prima che l'utente
abbia espresso in maniera esplicita i relativi consensi.

**ATTENZIONE!** nell'implementazione Base della Consent Mode il valore
di default dei vari consensi sarà impostato automaticamente su "Denied"
e non potrà essere modificato.

Anche in questo caso, ovviamente, **per poter garantire il corretto
ordine di esecuzione dei vari script, e quindi la corretta
implementazione della Consent Mode Base, è indispensabile che tutti i
vari snippet di codice siano inseriti nei rispettivi campi presenti
all'interno della sezione "Tracciamento Dati" presente alla pagina "Sito
-- Preferenze" del Wizard**

Ciò significa dunque che nel momento in cui lo script di tracciamento di
Google o lo script di gestione della CMP (es. Iubenda) dovesse essere
inserito in maniera manuale all'interno di campi come "Code Snippet --
Head / Footer" o in altre sezioni del sito diverse da quelle presenti
all'interno della sezione "Tracciamento Dati", l'ordine di esecuzione
dei vari script potrebbe non essere quello corretto e, di conseguenza,
la Consent Mode potrebbe non funzionare come deve.

