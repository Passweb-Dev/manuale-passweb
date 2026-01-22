# COMPONENTE CARRELLO CUSTOM



Il Componente **"Carrello Custom"** può **essere inserito unicamente
nella della pagina "Carrello"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_carrello_custom_res.bmp](./assets/media/image128.png){width="2.3618055555555557in"
height="2.8340277777777776in"}

dove mostrerà, all'interno di una griglia responsiva, tutti gli articoli
selezionati all\'interno del negozio, offrendo quindi un riassunto di
ciò che l'utente sta effettivamente per acquistare.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\componente_ecommerce_carrello_esempio_res.bmp](./assets/media/image129.png){width="6.257638888888889in"
height="4.288194444444445in"}

Inoltre, dipendentemente da chi sta effettuando l'ordine (un Cliente
oppure un Agente) e, ovviamente, da come sono stati settati i parametri
di configurazione di questo Componente, all'interno della pagina
Carrello sarà possibile effettuare anche tutta una serie di azioni come
ad esempio:

- Variare le quantità degli articoli in ordine

- Aggiungere articoli alla Wishlist

- Applicare eventuali buoni sconto

- Effettuare preventivi sulle spese di trasporto piuttosto che su
  eventuali spese accessorie legate a determinate modalità di pagamento

- Verificare i totali del documento nel momento in cui si dovesse
  decidere di utilizzare eventuali saldi di Gift Card o di Punti
  accumulati nell'ambito di determinate campagne di raccolta

- Modificare prezzi e/o sconti degli articoli in ordine (solo Agenti
  opportunamente abilitati)

- Verificare le provvigioni relative a ciascun articolo in ordine (solo
  Agenti)

- ...

In particolare per quel che riguarda le quantità dei singoli articoli
presenti in Carrello, modificabili direttamente da questo stesso
componente, vanno fatte le seguenti considerazioni:

- **E' possibile inserire quantità intere o decimali** in perfetto
  accordo con le relative impostazioni definite all'intero del
  gestionale. Nel caso di Mexal, ad esempio, è possibile impostare il
  numero di decimali gestiti direttamente sul singolo articolo.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\decimali_quantita_articoli.bmp](./assets/media/image130.png){width="3.147222222222222in"
height="2.0in"}

> **NOTA BENE:** per maggiori informazioni relativamente a come gestire
> in Mexal o su uno dei gestionali Ho.Re.Ca i decimali sulle quantità
> dei singoli articoli si rimanda allo specifico manuale.

- Dopo aver variato la quantità di un articolo presente in carrello, può
  essere necessario, dipendentemente dalle impostazioni di
  configurazione del componente stesso, confermare il dato immesso
  cliccando sul pulsante **"Aggiorna Dati"** presente in corrispondenza
  della relativa riga articolo, oppure sul pulsante globale "**Aggiorna
  Carrello**"

> Nel caso in cui siano stati inseriti in carrello **articoli a
> taglie/colori**, (gestiti cioè con la relativa tabella Mexal) per ogni
> singola riga verranno visualizzate, e sarà quindi possibile
> modificare, le quantità di ogni singola taglia/colore inserita per
> l'articolo considerato.
>
> Volendo è anche possibile decidere di visualizzare, per questa
> tipologia di articoli, le opzioni (taglie o colori) a quantità zero in
> maniera tale da consentire l'aggiunta in ordine di tali elementi
> (assegnandogli ovviamente una quantità diversa da zero) operando
> direttamente all'interno del carrello e senza dover per forza di cose
> passare dalla relativa scheda prodotto.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\articoli_a_taglie_carrello_res.bmp](./assets/media/image131.png){width="5.441666666666666in"
height="3.3805555555555555in"}

> **ATTENZIONE**! Nel caso in cui si sia deciso di gestire le
> disponibilità articolo con i valori presenti nel database di Passweb
> impostando anche il parametro "**Gestione Acquisto**", presente alla
> pagina "**Catalogo -- Catalogo Mexal / Ho.Re.Ca.**" del Wizard sul
> valore "**Acquista solo se disponibile**", confermando eventuali
> variazioni agli articoli presenti in carrello, verrà automaticamente
> avviato un controllo per verificare che le nuove quantità soddisfino
> le disponibilità dei relativi articoli.
>
> In queste condizioni nel caso in cui un certo articolo non sia
> disponibile per la nuova quantità impostata verrà visualizzato un
> apposito messaggio per informare l'utente relativamente alla massima
> quantità acquistabile per quello stesso articolo.
>
> **NOTA BENE:** per maggiori informazioni relativamente alla gestione
> delle disponibilità articolo si veda anche la sezione "Catalogo --
> Catalogo Mexal / Ho.Re.Ca." di questo manuale.

Per quel che riguarda invece i dati e le informazioni visualizzate in
Carrello, come precedentemente accennato, queste potranno variare, oltre
che sulla base degli specifici parametri di configurazione e dei singoli
Componenti in esso inseriti, anche dipendentemente dal fatto che ad
effettuare l'ordine sia un Agente (Ecommerce Mexal) piuttosto che un
normale cliente del sito.

In generale dunque all'interno del Componente Carrello potremmo disporre
dei seguenti campi:

**Nota:** tale campo potrà essere visualizzato o meno, ai soli Agenti
oppure anche ai normali clienti che effettuano un ordine sul sito.

In particolare la visibilità del campo ai soli Agenti piuttosto che ai
normali clienti dipende dai permessi di visibilità assegnati al
componente "**Campo Testo**" che deve essere necessariamente inserito
tra i Componenti interni al Carrello e mappato sul campo "**Note**", per
gestire correttamente questo tipo di informazione

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\carrello_agente_res.bmp](./assets/media/image132.png){width="6.35in"
height="3.938888888888889in"}

Sfruttando tale campo l'utente avrà la possibilità di inserire, per
ciascuno degli articoli che intende acquistare, una specifica nota
(oltre a quella che sarà poi possibile inserire, a livello di intero
documento, anche in fase di conferma ordine)

Nel caso in cui siano state inserite delle note di riga, queste verranno
correttamente visualizzate nel riepilogo dell'ordine cosi come nella
stampa e in tutte le mail connesse a questo stesso ordine, **e questo
indipendentemente dal fatto che l'utente sia o meno un agente**. In
questo modo, dunque, importando ad esempio all'interno del sito un
ordine creato in Mexal e che contiene anche delle note di riga, l'utente
a cui è riferito il documento avrà comunque sempre la possibilità di
visionare il dettaglio del documento nella sua interezza, note di riga
comprese.

> **NOTA BENE:** le note di riga saranno memorizzate in Mexal come note
> riportabili o non riportabili dipendentemente da quanto impostato alla
> pagina "Configurazione Ordini" del Wizard in corrispondenza del
> parametro "Note sul Documento"
>
> **NOTA BENE:** in fase di importazione ordini dal gestionale, verranno
> considerate come note di riga solo le note (riportabili o non
> riportabili) specificate dopo il codice articolo.

**Sconto (solo Ecommerce Mexal):** questo campo potrà essere
visualizzato al verificarsi delle seguenti condizioni:

- All'interno del componente Carrello è presente, tra gli altri, anche
  un Componente **"Campo Testo"** mappato sul campo articolo
  "**Sconto**".

- Chi effettua l'ordine è un Agente opportunamente abilitato alla
  modifica degli sconti

In queste condizioni verrà dunque visualizzato per ogni singolo articolo
in Carrello il prezzo al netto di eventuali sconti, sconti questi che
potranno essere inseriti all'interno di un campo di testo liberamente
modificabile.

L'Agente opportunamente abilitato alla modifica degli sconti avrà quindi
la possibilità di inserire e/o modificare per ogni singolo articolo in
carrello determinati sconti, adottando, in questo senso, la stessa
logica degli sconti Mexal.

Sarà quindi possibile gestire:

- **sconti a valore**, anteponendo il carattere \'-\' alla cifra (es.
  -100);

- **sconti in percentuale** con un massimo di due cifre decimali (es.
  10,48);

- **sconti a cascata** con un massimo di 9 valori ammessi (es. 10 + 20 +
  30 + 40)

- **sconti Merce** con valori compresi tra 100 e 109.

**ATTENZIONE!** Nel caso in cui per un certo articolo sia stata attivata
anche la funzionalità **"Sconto Massimo articolo"** e l'Agente tenti di
inserire per esso uno sconto superiore al massimo valore ammesso, verrà
visualizzato un apposito messaggio per informarlo che lo sconto inserito
è superiore a quello massimo consentito.

Infine nel caso in cui per un articolo sia già presente uno sconto, e
l'Agente decidesse di azzerare tale valore lasciando vuoto il relativo
campo, l'applicazione interpreterà questa azione come la volontà d parte
dell'Agente di non applicare all'articolo nessuno sconto.

> **NOTA BENE:** per gli articoli di tipo "Campionario" lo sconto
> indicato dall'agente verrà applicato a tutti i singoli articoli
> componenti il campionario stesso. Per gli articoli a confezioni invece
> lo sconto indicato dall'Agente verrà applicato sul singolo elemento
> della confezione.

**ATTENZIONE! Lo Sconto Massimo gestito per un certo articolo non è
legato ad un eventuale Prezzo Minimo impostato per l'articolo stesso**

Ciò significa dunque che se un Agente è stato abilitato alla modifica
dei prezzi e non è stato impostato correttamente il campo relativo al
prezzo minimo di vendita, l'Agente potrebbe anche applicare uno sconto
tale da portare il prezzo dell'articolo al di sotto del valore impostato
per il suo sconto massimo.

Per maggiori informazioni relativamente alle funzionalità Mexal
**"Blocca Modifica Sconto (Agente)**" e "**Sconto Massimo Articolo
(Agente)**" si vedano le relative sezioni di questo manuale
("*Configurazione Gestionale -- Mexal Parametri Configurazione
Gestionale Mexal Attivazione Passweb -- Funzionalità Mexal Articoli --
Gestione Sconto Massimo Articoli*" -- "*Configurazione Gestionale --
Mexal Parametri Configurazione Gestionale Mexal Attivazione Passweb --
Funzionalità Mexal Clienti -- Blocca Modifica Sconto*").

Anche in questo caso dopo aver impostato un nuovo sconto potrebbe essere
necessario confermare il dato immesso cliccando per questo,
dipendentemente dalle impostazioni di configurazione del componente
stesso, sul pulsante **"Aggiorna"** presente in corrispondenza della
relativa riga articolo, oppure sul pulsante globale "**Aggiorna
Carrello**"

**Prezzo (solo Ecommerce Mexal):** questo campo potrà essere
visualizzato al verificarsi delle seguenti condizioni:

- All'interno del componente Carrello è presente, tra gli altri, anche
  un Componente "**Campo Testo**" mappato sul campo articolo
  "**Prezzo**".

- Chi effettua l'ordine è un Agente opportunamente abilitato alla
  modifica dei Prezzi

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\carrello_modifica_prezzo.bmp](./assets/media/image133.png){width="5.01875in"
height="3.6319444444444446in"}

L'Agente opportunamente abilitato alla modifica dei prezzi avrà quindi
la possibilità, mediante il campo evidenziato in figura, di impostare
per ciascuno degli articoli presenti in carrello un nuovo prezzo di
vendita

Inoltre nel caso in cui per un certo articolo sia stata attivata anche
la funzionalità "**Prezzo Minimo**" (cosa questa assolutamente
indispensabile in questo tipo di gestione) e l'Agente tenti di impostare
per esso un prezzo inferiore a quello minimo consentito, , verrà
visualizzato un apposito messaggio di errore per informarlo che il
valore impostato non è corretto **e il prezzo dell'articolo verrà
automaticamente impostato sul prezzo minimo consentito.**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\carrello_modifica_prezzo2.bmp](./assets/media/image134.png){width="5.184027777777778in"
height="3.6319444444444446in"}

**ATTENZIONE! Il prezzo minimo gestito per un certo articolo non è
legato ad un eventuale sconto massimo impostato per l'articolo stesso**

Ciò significa dunque che se un Agente è stato abilitato alla modifica
degli sconti e non è stato impostato correttamente il campo relativo
allo sconto massimo di vendita, l'Agente potrebbe anche applicare uno
sconto tale da portare il prezzo dell'articolo al di sotto del valore
impostato per il suo prezzo minimo

Per maggiori informazioni relativamente alle funzionalità Mexal
**"Modifica Prezzo**" e "**Prezzo Minimo**" si vedano le relative
sezioni di questo manuale ("*Configurazione Gestionale -- Mexal
Parametri Configurazione Gestionale Mexal Attivazione Passweb --
Funzionalità Mexal Articoli -- Prezzo minimo" -- "Configurazione
Gestionale -- Mexal Parametri Configurazione Gestionale Mexal
Attivazione Passweb -- Funzionalità Mexal Clienti -- Prezzo minimo
/Modifica Prezzo*").

**ATTENZIONE!!! Nel caso in cui si dovesse decidere di attivare questo
tipo di funzionalità e di concedere quindi a determinati Agenti la
possibilità di modificare, in fase di ordine all'interno del sito, i
prezzi degli articoli, diventa di assoluta importanza impostare per
ciascuno di essi un prezzo minimo.**

**In caso contrario infatti l'Agente abilitato alla modifica dei prezzi
non avrebbe alcun limite e, volendo, potrebbe anche azzerare
completamente il prezzo di vendita.**

**Scadenza (solo Ecommerce Mexal):** tale campo potrà essere
visualizzato o meno, ai soli Agenti oppure anche ai normali clienti che
effettuano un ordine sul sito.

In particolare la visibilità del campo ai soli Agenti piuttosto che ai
normali clienti dipende dai permessi di visibilità assegnati al
componente "**Campo Data**" che deve essere necessariamente inserito tra
i Componenti interni al Carrello e mappato sul campo "**Data Scadenza**"
per poter gestire correttamente questo tipo di informazione

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\data_scadenza_per_riga_res.bmp](./assets/media/image135.png){width="6.404861111111111in"
height="4.325in"}

Grazie a questo campo l'utente avrà quindi la possibilità di indicare
una specifica data di consegna/scadenza per ogni singolo articolo
presente in carrello, **data questa che verrà poi riportata, secondo le
stesse logiche gestionali, nelle corrispondenti righe del documento
Mexal.**

Nel caso in cui tale campo venga lasciato vuoto ci potrà comunque essere
sempre la possibilità di inserire, attraverso l'apposito campo del
modulo di checkout ordine, una data di scadenza per l'interno documento,
data questa che verrà quindi riportata, ancora una volta in perfetto
accordo con quelle che sono le logiche gestionali, come data di scadenza
in testata del corrispondente documento Mexal.

**Provvigione (campo in sola visualizzazione -- solo Ecommerce Mexal):**
questo campo potrà essere visualizzato al verificarsi delle seguenti
condizioni:

- Chi effettua l'ordine è un Agente

- Tra i Componenti interni al Carrello è stato inserito anche un
  Componente "**Dati Articolo**" mappato sul Campo Articolo
  "**Provvigione**"

Grazie a questo campo l'Agente avrà quindi la possibilità di
visualizzare esattamente la provvigione che gli spetta relativamente
allo specifico articolo inserito in carrello.

Infine è necessario chiarire bene altri due aspetti fondamentali
relativamente al funzionamento del componente Carrello Custom:

- **Gli articoli in omaggio e/o gli articoli di tipo S utilizzati
  all'interno delle Promozioni Mexal verranno automaticamente aggiunti
  in carrello al verificarsi delle condizioni di applicabilità della
  Promozione stessa.**

> **Tali articoli a differenza di quelli inseriti direttamente
> dall'utente, non potranno, ovviamene, essere variati in alcun modo.**
> Non sarà quindi possibile modificarne la quantità, lo sconto e/o il
> prezzo ne tanto meno sarà possibile inserire per essi una specifica
> nota.

- **Per visualizzare l'importo totale degli articoli presenti in
  carrello** (con il dettaglio delle relative voci quali IVA, Spese di
  spedizione ecc...) è necessario, da una parte, che tra i Componenti
  interni al Carrello sia stato inserito anche il Componente "Prezzo" e
  dall'altra parte che tale componente sia effettivamente visibile
  all'utente che sta effettuando l'ordine.

> **ATTENZIONE!** Nel caso in cui il componente Prezzo non sia stato
> inserito tra i Componenti interni al Carrello e/o non sia visibile
> all'utente che sta effettuando l'ordine, per ovvie ragioni, non verrà
> visualizzato ne il modulo per l'applicazione di eventuali Buoni Sconto
> ne tanto meno quello per il preventivo delle spese di spedizione.

Cliccando sul pulsante "**Continua con l'Ordine**", verranno salvate
eventuali modifiche apportate al carrello ma non ancora confermate in
maniera specifica e l'utente verrà automaticamente ricondotto alla
pagina "Ordine" dove potrà portare a termine, grazie all'apposito modulo
di checkout, la procedura di acquisto.

> **NOTA BENE:** nel caso in cui l'utente in esame non abbia codificato
> almeno un indirizzo di spedizione cliccando sul pulsante "Continua con
> l'ordine" verrà ricondotto alla pagina "Profilo Utente" da dove potrà
> codificare uno o più indirizzi di spedizione merce, indispensabili per
> poter portare poi a termine correttamente la procedura di conferma
> ordine.

Anche questa volta nel caso in cui si sia deciso di gestire le
disponibilità articolo con i valori presenti nel database di Passweb
impostando anche il parametro "Gestione Acquisto", presente alla pagina
"Catalogo -- Catalogo Mexal / Ho.Re.Ca." del Wizard sul valore "Acquista
solo se disponibile", prima del passaggio al Checkout Ordine, verrà
automaticamente avviato un controllo per verificare che le nuove
quantità soddisfino le disponibilità dei relativi articoli.

Nel caso in cui un certo articolo non sia più disponibile (perché magari
sono stati contemporaneamente confermati altri ordini contenenti gli
stessi articoli) verrà visualizzato un apposito messaggio per informare
l'utente relativamente alla massima quantità acquistabile per quello
stesso articolo.

Infine, nel caso in cui alcuni degli articoli presenti in carrello non
soddisfino eventuali condizioni di massimo/minimo fatturabile verrà
visualizzato un' apposito messaggio di errore e l'utente non potrà
proseguire nell'acquisto senza prima aver soddisfatto tali condizioni.

![\\\\192.168.0.84\\d\$\\ManPassweb_Ecommerce\\Videate\\carrello_errore_minimo_fatturabile.bmp](./assets/media/image136.png){width="5.055555555555555in"
height="3.1659722222222224in"}

**ATTENZIONE! Gli articoli visualizzati in Carrello, possono variare a
seconda del fatto che l'utente abbia già inserito degli articoli durante
la stessa sessione di navigazione e/o a seconda del fatto di aver
effettuato o meno l'autenticazione al sito.**

In generale, infatti, una volta effettuata l'autenticazione al sito,
verranno automaticamente visualizzati in Carrello (e conseguentemente
anche nel Carrellino), gli ultimi articoli inseriti dallo specifico
utente.

Nel caso in cui l'utente avesse concluso l'ordine e/o svuotato il
proprio carrello, all'autenticazione successiva questo risulterà
ovviamente vuoto e tale rimarrà fintanto che non verranno inseriti nuovi
articoli.

