# IMPLEMENTAZIONE DEL CONSENSO AL TRACCIAMENTO O ALL'USO DEI COOKIE CON IL MATOMO JAVASCRIPT TRACKING CLIENT



Nel momento in cui si dovesse comunque decidere di implementare un
sistema per gestire le richieste preventive di consenso utilizzando gli
strumenti messi a disposizione da Matomo occorre innanzitutto
considerare che Matomo permette di gestire due diverse tipologie di
consenso:

- **Consenso al tracciamento:** gestendo questo tipo di consenso non
  verrà installato nessun cookie sul browser dell'utente e non verrà
  inviata alcuna richiesta di tracciamento senza che l'utente abbia
  prima fornito esplicitamente il proprio consenso. Non appena il
  consenso verrà fornito, saranno installati i relativi cookie e
  verranno inviate all'applicativo tutte le richieste di tracciamento
  iniziando quindi a raccogliere i dati

- **Consenso all'utilizzo dei cookie**: gestendo questo tipo di consenso
  le richieste di tracciamento verranno sempre inviate. Tuttavia, i
  cookie saranno effettivamente utilizzati solo nel momento in cui
  l'utente avrà fornito il consenso al loro utilizzo e alla loro
  memorizzazione

Una volta compresi i due diversi tipi di consenso gestibili con Matomo
possiamo passare ad analizzare il processo da seguire per arrivare ad
implementare correttamente un sistema di gestione delle richieste
preventive di consenso, processo questo che dovrà passare
obbligatoriamente attraverso 3 distinti step:

- Step 1 -- Blocco preventivo

- Step 2 -- Richiesta del consenso

- Step 3 -- Acquisizione / Revoca del consenso

**[STEP 1 -- BLOCCO PREVENTIVO]{.underline}**

In questo primo step sarà necessario configurare tutto il sistema in
maniera tale da essere certi di soddisfare perfettamente il concetto di
consenso preventivo evitando quindi che vengano effettivamente
registrati i dati dell'utente prima ancora che esso abbia potuto
esprimere la sua preferenza.

Per far questo è sufficiente modificare il codice di tracciamento di
Matomo inserendo, dipendentemente dalla tipologia di consenso che si
vuole gestire, una delle seguenti istruzioni:

- **\_paq.push(\[\'requireConsent\'\]);** - istruzione da inserire nel
  momento in cui si voglia gestire il consenso al tracciamento

> Una volta eseguita questa istruzione non verranno inviate richieste di
> tracciamento a Matomo e non verrà installato nel browser dell'utente
> nessun tipo di cookie

- **\_paq.push(\[\'requireCookieConsent\'\]);** - istruzione da inserire
  nel momento in cui si voglia gestire il consenso all'utilizzo dei
  cookie

> Una volta eseguita questa istruzione le richieste di tracciamento
> verranno comunque inviate a Matomo ma sul browser dell'utente non
> verrà installato alcun cookie

**ATTENZIONE!** per ovvie ragioni le istruzioni sopra indicate dovranno
essere inserite come prime istruzioni del codice di monitoraggio. Solo
in questo modo sarà infatti possibile adempiere al concetto di "consenso
preventivo"

[Supponendo dunque di voler gestire il consenso al
tracciamento]{.underline}, il codice di monitoraggio standard di Matomo

*\<!\-- Matomo \--\>*

*\<script\>*

*var \_paq = window.\_paq = window.\_paq \|\| \[\];*

*/\* tracker methods like \"setCustomDimension\" should be called before
\"trackPageView\" \*/*

*\_paq.push(\[\'trackPageView\'\]);*

*\_paq.push(\[\'enableLinkTracking\'\]);*

*(function() {*

*var u=\"//www.sitodatracciare.it/\";*

*\_paq.push(\[\'setTrackerUrl\', u+\'matomo.php\'\]);*

*\_paq.push(\[\'setSiteId\', \'5\'\]);*

*var d=document, g=d.createElement(\'script\'),
s=d.getElementsByTagName(\'script\')\[0\];*

*g.async=true; g.src=u+\'matomo.js\'; s.parentNode.insertBefore(g,s);*

*})();*

*\</script\>*

*\<!\-- End Matomo Code \--\>*

dovrà essere modificato come di seguito indicato

*\<!\-- Matomo \--\>*

*\<script\>*

*var \_paq = window.\_paq = window.\_paq \|\| \[\];*

*/\* tracker methods like \"setCustomDimension\" should be called before
\"trackPageView\" \*/*

**\_*paq.push(\[\'requireConsent\'\]);***

*\_paq.push(\[\'trackPageView\'\]);*

*\_paq.push(\[\'enableLinkTracking\'\]);*

*(function() {*

*var u=\"//www.sitodatracciare.it/\";*

*\_paq.push(\[\'setTrackerUrl\', u+\'matomo.php\'\]);*

*\_paq.push(\[\'setSiteId\', \'5\'\]);*

*var d=document, g=d.createElement(\'script\'),
s=d.getElementsByTagName(\'script\')\[0\];*

*g.async=true; g.src=u+\'matomo.js\'; s.parentNode.insertBefore(g,s);*

*})();*

*\</script\>*

*\<!\-- End Matomo Code \--\>*

In questo modo andremo di fatto a impostare il default per ogni utente,
relativamente alle preferenze di tracciamento, sul "negato" e l'utente
potrà iniziare ad essere tracciato, con l'installazione dei relativi
cookie solo quando e se avrà espresso esplicitamente il suo consenso.

**[STEP 2 -- RICHIESTA DEL CONSENSO]{.underline}**

In questo secondo step sarà necessario gestire correttamente la
richiesta del consenso verso gli utenti che atterrano sul nostro sito e
questo dovrà essere fatto, da una parte, inserendo nelle varie
informative presenti sul sito tutto quanto necessario per avvisare gli
utenti che il sito utilizza Matomo come sistema di web analytics oltre
ovviamente a quelli che sono i dati che verranno poi raccolti e,
dall'altra parte, mettendo questi stessi utenti nelle condizioni di
poter scegliere se prestare o meno il loro consenso.

Sotto questo punto di vista, come spiegato anche nel precedente capitolo
di questo manuale, sarebbe preferibile non utilizzare il form di Opt Out
standard di Matomo (quello gestito mediante un iframe) ma ricorrere
all'utilizzo di un form customizzato, form questo che potrebbe essere
realizzato in Passweb con un semplice componente HTML seguendo le
istruzioni presenti a questo link
<https://developer.matomo.org/guides/tracking-javascript-guide#optional-creating-a-custom-opt-out-form>

Di seguito viene riportato un esempio del codice HTML utilizzabile per
realizzare un form di questo tipo

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\matomo_13.bmp](./assets/media/image14.png){width="5.526388888888889in"
height="3.3222222222222224in"}

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\matomo_14.bmp](./assets/media/image15.png){width="4.151388888888889in"
height="3.7694444444444444in"}

In sostanza si tratterà di verificare innanzitutto lo stato attuale del
consenso dell'utente che visita il sito mettendogli poi a disposizione,
un pulsante, un check o comunque un controllo mediante il quale poter
modificare lo stato di questo consenso.

Nell'esempio sopra indicato le righe dalla 1 alla 9 definiscono e
costruiscono il form. Le righe dalla 11 alla 19 controllano lo stato
attuale del consenso dell'utente selezionando o meno, di conseguenza, il
relativo check. Infine le righe dalla 21 alla 31 gestiscono
l'aggiornamento dello stato del consenso sulla base delle scelte
effettuate dall'utente che potrà selezionare o deselezionare secondo
quelle che sono le sue esigenze il relativo check.

**[STEP 3 -- ACQUISIZIONE / REVOCA DEL CONSENSO]{.underline}**

In quest'ultimo step sarà necessario acquisire in maniera definitiva la
scelta effettuata dall'utente attivando o bloccando, da questo momento
in poi, il sistema di tracciamento e la raccolta dei dati.

Nel form di esempio indicato nello step precedente infatti l'utente ha
la possibilità di effettuare la sua scelta e una volta fatto verrà
aggiornato di conseguenza lo stato del suo consenso ma senza le corrette
istruzioni, questa scelta non verrà memorizzata per cui cambiando pagina
si tornerà sempre nelle stesse condizioni iniziali.

Come indicato nella documentazione ufficiale di Matomo è possibile
risolvere questo problema in due modi diversi:

- Lasciando che sia Matomo a ricordarsi della scelta effettuata
  dall'utente

- Utilizzando un proprio Consent Tool per ricordare la scelta effettuata

Supponendo dunque di dover gestire il consenso al tracciamento (come
indicato anche negli step precedenti) e volendo far memorizzare
direttamente a Matomo le scelte effettuate dagli utenti (strada questa
più semplice rispetto a quella di doversi memorizzare autonomamente le
scelte degli utenti) sarà necessario modificare lo script di gestione
del form di opt out come di seguito indicato:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\matomo_15.bmp](./assets/media/image16.png){width="5.519444444444445in"
height="3.6708333333333334in"}

Nello specifico l'istruzione

- **\_paq.push(\[\'rememberConsentGiven\'\]);** (riga 25) consentirà a
  Matomo di ricordare che l'utente ha dato il suo consenso al
  tracciamento e gli permetterà quindi di raccogliere i dati durante la
  vista alle successive pagine del sito e anche durante successive
  visite al sito da parte dello stesso utente (con ovviamente lo stesso
  browser).

> Tecnicamente infatti l'esecuzione di questa istruzione installerà nel
> browser dell'utente un cookie chiamato "consent" e fintanto che questo
> cookie sarà presente Matomo saprà che l'utente ha prestato il suo
> consenso e potrà quindi continuare a tracciare e a raccogliere i dati
> automaticamente

- **\_paq.push(\[\'forgetConsentGiven\'\]);** (riga 28) consentirà a
  Matomo di "dimenticarsi" della scelta effettuata dall'utente
  riportandolo nelle condizioni di default che, come indicato nello Step
  1, saranno condizioni di "consenso negato".

> Tecnicamente l'esecuzione di questa istruzione porterà all'eventuale
> eliminazione del cookie "consent"

