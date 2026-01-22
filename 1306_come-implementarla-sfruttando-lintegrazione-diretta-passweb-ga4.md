# COME IMPLEMENTARLA SFRUTTANDO L'INTEGRAZIONE DIRETTA PASSWEB -- GA4



Nei precedenti capitoli di questo manuale abbiamo visto che cos'è la
Consent Mode e quelle che sono le sue due diverse possibilità di
implementazione (Base e Avanzata). Ora invece, considerando che i siti
Passweb offrono già la possibilità di integrare nativamente il
tracciamento del sito mediante GA4, senza di fatto dover andare ad
inserire il relativo script di tracciamento, vediamo come poter
integrare tutto ciò con l'attivazione anche della Consent Mode nella sua
versione Base e Avanzata.

In questo senso le operazioni da fare sono veramente molto semplici.

Sarà infatti sufficiente portarsi alla pagina "**Sito -- Preferenze**"
del Wizard, tab "**Tracciamento Dati**" e impostare il parametro
"**Blocco Preventivo dei cookie**" su una delle opzioni presenti
all'interno del relativo menu a tendina

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\consent_mode_1.bmp](./assets/media/image14.png){width="5.726388888888889in"
height="3.6180555555555554in"}

**ATTENZIONE!** come ormai dovrebbe essere chiaro la Consent Mode non è
una cosa che può prescindere dall'utilizzo di una piattaforma CMP per
cui il suo utilizzo va sempre attivato e considerato in relazione alla
specifica piattaforma CMP che si è deciso di implementare

**Allo stato attuale l'integrazione nativa tra Passweb e GA4 consente di
attivare la gestione della Consent Mode per le piattaforme di Iubenda
(in modalità Base o Avanzata), Cookiebot**

Nello specifico dunque:

- **No**: selezionando questa opzione non verrà attivato nessun blocco
  preventivo dei cookie e, conseguentemente, non verrà attivata neppure
  la gestione della Consent Mode.

> In queste condizioni quindi eventuali script di tracciamento verranno
> eseguiti sempre e comunque rilasciando tutti i cookie di cui hanno
> bisogno
>
> **ATTENZIONE! questa opzione rende il sito non compliance con quanto
> richiesto dal GDPR**

- **Iubenda + Consent Mode (v2 Avanzata):** selezionando questa opzione
  verrà attivata la Consent Mode di Iubenda in modalità Avanzata e sarà
  quindi necessario inserire lo snippet di codice fornito da Iubenda
  stessa all'interno del successivo campo "**Code Snippet Cookie**" e
  impostare anche un valore di default per i vari consensi (sezione
  "**Valori Consent Default**")

> Per maggiori informazioni su quello che è il funzionamento della
> Consent Mode in modalità Avanzata e su cosa comporta questa scelta si
> faccia riferimento a quanto indicato anche nei precedenti capitoli di
> questo manuale
>
> In queste condizioni sarà inoltre di fondamentale importanza:

- **Accertarsi di non avere attivato su Iubenda l'autoblocking.** In
  caso contrario infatti lo snippet di codice fornito da Iubenda
  andrebbe a bloccare tutti gli script presenti sul sito compresi quelli
  indispensabili per il corretto funzionamento del sito stesso

- **Eliminare dallo snippet di codice fornito da Iubenda, prima di
  inserirlo all'interno del relativo campo Passweb (Code Snippet
  Cookie), il seguente scritp**

> *\<script type=\"text/javascript\"
> src=\"//cs.iubenda.com/sync/XXXX.js\"\>\</script\>*
>
> Dove XXXX è un numero identificato del proprio account Iubenda.
>
> Tale script, se inserito in Passweb, demanderebbe infatti la gestione
> del valore di default dei vari consensi direttamente a Iubenda andando
> quindi a sovrascrivere eventuali impostazioni settate in questo senso
> direttamente all'interno di Passweb

- **Iubenda + Consent Mode (v2 Base):** selezionando questa opzione
  verrà attivata la Consent Mode di Iubenda in modalità Base e sarà
  quindi necessario inserire lo snippet di codice fornito da Iubenda
  stessa all'interno del successivo campo "**Code Snippet Cookie**"

> Per maggiori informazioni su quello che è il funzionamento della
> Consent Mode in modalità Base e su cosa comporta questa scelta si
> faccia riferimento a quanto indicato anche nei precedenti capitoli di
> questo manuale
>
> In queste condizioni sarà inoltre di fondamentale importanza:

- **Accertarsi di non avere attivato su Iubenda l'autoblocking.** In
  caso contrario infatti lo snippet di codice fornito da Iubenda
  andrebbe a bloccare tutti gli script presenti sul sito compresi quelli
  indispensabili per il corretto funzionamento del sito stesso

- **Eliminare dallo snippet di codice fornito da Iubenda, prima di
  inserirlo all'interno del relativo campo Passweb (Code Snippet
  Cookie), il seguente scritp**

> *\< script type=\"text/javascript\"
> src=\"//cs.iubenda.com/sync/XXXX.js\"\>\</script\>*
>
> Dove XXXX è un numero identificato del proprio account Iubenda.
>
> Tale script, se inserito in Passweb, demanderebbe infatti la gestione
> del valore di default dei vari consensi direttamente a Iubenda andando
> quindi a sovrascrivere il valore di default impostato da Passweb per i
> vari consensi, valore questo che come precedentemente indicato, in
> queste condizioni sarà sempre "Denied" e non potrà essere modificato.

- **CookieBot + Consenti Mode (v2)**: consente di attivare la gestione
  della Consent Mode di CookieBot e sarà quindi necessario inserire lo
  snippet di codice fornito dalla piattaforma stessa all'interno del
  successivo campo "**Code Snippet Cookie**"

> In queste condizioni sarà inoltre di fondamentale importanza:

- **Accertarsi di non avere attivato su CookieBot l'autoblocking.** In
  caso contrario infatti lo snippet di codice fornito da Iubenda
  andrebbe a bloccare tutti gli script presenti sul sito compresi quelli
  indispensabili per il corretto funzionamento del sito stesso

**ATTENZIONE!** indipendentemente dalla specifica piattaforma CMP
utilizzata, **per poter garantire il corretto ordine di esecuzione dei
vari script, e quindi la corretta implementazione della Consent Mode
Base o Avanzata, è indispensabile che tutti i vari snippet di codice
siano inseriti nei rispettivi campi presenti all'interno della sezione
"Tracciamento Dati" presente alla pagina "Sito -- Preferenze" del
Wizard**

Ciò significa dunque che nel momento in cui lo script di tracciamento di
Google o lo script di gestione della CMP dovesse essere inserito in
maniera manuale all'interno di campi come "Code Snippet -- Head /
Footer" o in altre sezioni del sito diverse da quelle presenti
all'interno della sezione "Tracciamento Dati", l'ordine di esecuzione
dei vari script potrebbe non essere quello corretto e, di conseguenza,
la Consent Mode potrebbe non funzionare come deve.

