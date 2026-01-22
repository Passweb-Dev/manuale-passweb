# PRENOTAZIONE DI UN SERVIZIO / TRATTAMENTO VIA WEB



All'interno del sito la procedura attraverso cui dovrà passare l'utente
per confermare la prenotazione di un servizio/trattamento potrà essere
composta da uno o due step a seconda del fatto che si sia deciso di
visualizzare o meno anche la selezione della modalità di pagamento.

In particolare, **[nel caso in cui si sia deciso di non visualizzare la
selezione della modalità di pagamento]{.underline}**, portandosi nella
pagina Prenotazione il cliente visualizzerà un unico step all'interno
del quale verranno riportati:

- il nome del servizio/trattamento che intende prenotare (1)

- un campo Data grazie al quale poter selezionare la specifica data in
  corrispondenza della quale effettuare la sua prenotazione (2)

- un elenco delle risorse collegate al servizio, e correttamente gestite
  sul sito, con il relativo planning di disponibilità oraria (3)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\prenotazione_1.bmp](./assets/media/image338.png)

Accedendo alla pagina il campo **Data** verrà automaticamente
valorizzato con la data odierna; sarà comunque possibile indicare una
qualsiasi altra data di prenotazione (ovviamente successiva a quella
odierna) selezionandola dall'apposito calendario che verrà visualizzato
cliccando all'interno del campo stesso.

Una volta selezionata la data verrà visualizzato, **prelevando le
relative informazioni in tempo reale dal gestionale Ho.Re.Ca.**,
l'elenco delle risorse associate al servizio/trattamento indicato,
risorse queste che dovranno essere preventivamente configurate,
all'interno del gestionale, per poter esser gestite anche sul del sito.

> **NOTA BENE:** per maggiori informazioni relativamente a come
> configurare all'interno del gestionale Ho.Re.Ca. uno specifico
> trattamento/servizio, con le relative risorse ad esso associate,
> affinché questo possa essere correttamente gestito anche all'interno
> del sito web, si veda la corrispondente sezione di questo manuale
> (Configurazione -- Horeca Configurazione gestionale --
> Esportazione/Eliminazione di servizi/trattamenti dal gestionale
> Ho.Re.Ca. al sito web) .

Per ciascuna di queste risorse verrà infine mostrato il relativo
planning di disponibilità con all'interno tutti gli orari in
corrispondenza dei quali la relativa risorsa potrà essere prenotata per
quello specifico servizio/trattamento.

> **NOTA BENE:** la granularità del planning orario dipenderà ovviamente
> dalla durata dello specifico trattamento/servizio e conseguentemente
> da quanto impostato all'interno del gestionale Ho.Re.Ca nel
> corrispondente campo "**Tempo di Produzione**".

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\prenotazione_2.bmp](./assets/media/image339.png)

**ATTENZIONE!** Nel caso in cui per il giorno selezionato non sia
disponibile nessuna risorsa, o il centro sia chiuso, verrà visualizzato
un apposito messaggio di avviso.

Una volta selezionato, tra quelli disponibili all'interno del planning,
lo specifico orario in corrispondenza del quale prenotare il
servizio/trattamento desiderato, cliccando sul pulsante "**Procedi**"
l'utente verrà immediatamente ricondotto alla pagina di riepilogo per la
conferma della prenotazione.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\prenotazione_5a.bmp](./assets/media/image340.png)

Il servizio / trattamento prenotato sarà inserito all'interno di una
griglia responsiva le cui colonne possono essere definite direttamente
all'interno della sezione "**Gestione Contenuti**" presente nella
maschera di gestione e configurazione del Componente Prenotazione Custom

**ATTENZIONE! i Totali del documento verranno visualizzati solo ed
esclusivamente nel caso in cui tra i componenti inserti all'interno del
Componente Prenotazione Custom sia presente anche il componente Prezzo e
solo ed esclusivamente nel momento in cui il componente Prezzo sia
effettivamente visibile all'utente che sta effettuando l'ordine.**

Cliccando quindi sul pulsante **"Conferma"** la prenotazione verrà
inserita all'interno del gestionale Ho.Re.Ca., dove verrà memorizzata
nello stato di **"Preventivo"**.

**In queste condizioni dovrà quindi essere il gestore a confermare o,
eventualmente, ad annullare la prenotazione direttamente all'interno del
gestionale Ho.Re.Ca.**

> **NOTA BENE:** nel caso in cui in fase di configurazione del sito si
> sia scelto di non mostrare lo step per la selezione del pagamento, la
> relativa prenotazione **verrà sempre inserita nel gestionale** nello
> stato di "**Preventivo**", indipendentemente da eventuali situazioni
> di overbooking e/o di risorse obbligatorie non selezionate.

**Nel caso in cui si sia deciso di visualizzare anche lo step relativo
alla selezione del pagamento**, per poter confermare la propria
prenotazione, l'utente dovrà passare necessariamente attraverso un
secondo step, oltre a quello appena analizzato.

In queste condizioni quindi dopo aver selezionato data, risorsa e orario
della prenotazione, cliccando sul pulsante "Procedi" verrà aperta la
sezione relativa alla scelta della modalità di pagamento da adottare.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\prenotazione_6.bmp](./assets/media/image341.png)

**ATTENZIONE!** I pagamenti visualizzati all'interno di questa sezione
saranno solamente quelli per i quali, in fase di configurazione, è stato
correttamente selezionato il check "**Abilita pagamento per
prenotazioni**"

Sempre all'interno di questa sezione **e solo se per il sito è attiva
anche una Gift Card di tipo HoReCa**, oltre ai controlli per la
selezione della specifica modalità di pagamento verrà visualizzato anche
il campo "**Buno Sconto**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\abilitazione_step_pagamento_prenotazione_2.bmp](./assets/media/image342.png)

campo questo all'interno del quale l'utente avrà la possibilità di
inserire un eventuale Codice Gift Card in suo possesso per poter
usufruire dello sconto ad esso collegato (per maggiori informazioni
relativamente alla Gift Card HoReCa e alla possibilità di acquistare
Trattamenti e Servizi da poter eventualmente regalare a terzi si rimanda
a quanto indicato nel relativo capitolo di questo manuale "*Utenti --
Gift Card -- Gift Card Ho.Re.Ca.*")

**ATTENZIONE!** Se l'importo dell'eventuale Buono Sconto applicato
dovesse essere tale da coprire interamente l'acquisto del Trattamento
verrà nascosta la sezione relativa alla selezione della modalità di
pagamento e la prenotazione potrà quindi essere conclusa con importo
pari a 0

Una volta selezionata la modalità di pagamento desiderata, cliccando sul
pulsante "**Procedi**" l'utente verrà immediatamente ricondotto alla
pagina di riepilogo per la conferma della prenotazione.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\prenotazione_5.bmp](./assets/media/image343.png)

**ATTENZIONE!! Arrivati a questo punto prima di confermare in maniera
definitiva la prenotazione l'utente dovrà accettare esplicitamente le
condizioni di vendita.**

L'etichetta visualizzata a fianco del check di approvazione delle
condizioni di vendita è personalizzabile, così come il messaggio
visualizzato in caso di mancata approvazione da parte dell'utente,
sempre all'interno della sezione "*Sito -- Gestione Testi/Messaggi del
Sito*" selezionando il componente "Prenotazione Custom (Reservation)" ed
agendo sui rispettivi campi "**Check Condizioni d'ordine**" e
"**Messaggio Errore Condizioni Ordine**".

Una volta approvate anche le condizioni di vendita, cliccando sul
pulsante **"Conferma"** la prenotazione verrà inserita all'interno del
gestionale Ho.Re.Ca., dove verrà memorizzata nello stato di
**"Confermata".**

> **NOTA BENE:** nel caso in cui si sia deciso di visualizzare lo step
> relativo alla selezione del pagamento tutte le prenotazioni andate a
> buon fine verranno inserite nel gestionale, dove nasceranno nello
> stato di **"Confermato", contestualmente al reindirizzamento
> dell'utente sul sito della banca e prima ancora quindi dell'effettivo
> pagamento.**

Alla conferma della prenotazione sul sito, e prima che questa stessa
prenotazione venga effettivamente inserita nel gestionale, verranno
avviati dei controlli su eventuali situazioni di overbooking.

Nel caso in cui, dunque, si dovesse verificare per la prenotazione via
web una situazione di overbooking, subito dopo aver cliccato sul
pulsante "Conferma" verrà visualizzato un apposito messaggio di avviso e
la relativa prenotazione non sarà inserita nel gestionale.

**ATTENZIONE!** Nel caso in cui il pagamento selezionato dall'utente
dovesse essere uno dei pagamenti on line, occorre sempre considerare
che, **a meno di overbooking, la prenotazione verrà effettivamente
inserita nel gestionale prima ancora che l'utente abbia effettivamente
completato il pagamento.**

**In conseguenza di ciò è di fondamentale importanza prestare
particolare attenzione alle possibili casistiche generate dalle
procedure di pagamento on line.**

In particolare nel caso in cui la procedura di pagamento venga portata a
termine in maniera corretta (l'utente passa attraverso tutti i vari step
proposti dalla banca per completare il pagamento, inserendo quindi tutti
i dati richiesti e tornando alla fine sul sito Passweb), la banca
invierà a Passweb una risposta positiva sull'esito del pagamento per cui
alla ricezione di questa risposta Passweb si preoccuperà di inserire
all'interno del gestionale il corrispondente importo pagato.

Lato gestionale, l'esercente potrà quindi verificare questi dati
portandosi nella maschera "Pagamento Web" attivabile dall'omonima voce
presente nel contesto della prenotazione del relativo
servizio/trattamento.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\prenotazione_7.bmp](./assets/media/image344.png)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\prenotazione_8.bmp](./assets/media/image345.png)

> **NOTA BENE:** nel caso in cui entrambi i campi (Tipo di pagamento e
> Importo) della maschera **"Pagamento Web"** sopra evidenziata siano
> **correttamente valorizzati**, la relativa prenotazione web potrà
> ritenersi correttamente pagata.
>
> **NOTA BENE:** se, al momento dell'inserimento nel gestionale
> dell'importo effettivamente pagato, Passweb non dovesse riuscire per
> qualche ragione a contattare il gestionale, verrà inviata
> immediatamente una mail agli indirizzi configurati all'interno del
> campo "Indirizzi per la Email di informazione" della pagina
> "Configurazione Ordini" del Wizard, per informare chi di dovere che la
> prenotazione il cui codice gestionale è inserito all'interno della
> mail stessa è stata correttamente pagata.

Nel caso in cui, invece, durante una delle fasi di pagamento sul sito
della banca, l'utente dovesse per qualsiasi ragione cliccare sul
pulsante **"Annulla",** la banca si preoccuperà di reindirizzare
l'utente stesso al sito di partenza inviando anche a Passweb, in
relazione al pagamento in questione, una risposta negativa.

**Una volta ricevuta questa risposta negativa da parte della banca
Passweb stesso si preoccuperà di comunicarla al gestionale Ho.Re.Ca.
ponendo la relativa prenotazione (comunque già presente nel gestionale)
nello stato di "Annullata".**

Infine nel caso in cui la procedura di pagamento dovesse essere
interrotta dall'utente in maniera anomala chiudendo il browser
(indipendentemente dal fatto di aver completato o meno il pagamento), la
banca non avrebbe modo di inviare a Passweb alcuna risposta
relativamente al pagamento in questione.

In assenza quindi di risposte positive o negative da parte della banca,
Passweb non potrà avere coscienza dell'esito della transazione per cui,
considerando anche che la prenotazione in questa fase si trova comunque
già all'interno del gestionale, non potrà ne considerare il pagamento
andato a buon fine (inserendo il corrispondente importo pagato
all'interno del gestionale) ne tanto meno considerare la relativa
prenotazione come annullata.

**In queste condizioni quindi le cose verranno lasciate esattamente come
sono, ossia con la prenotazione inserita all'interno del gestionale
nello stato di "Confermata" e la maschera di "Pagamento Web" con importo
nullo.**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\prenotazione_9.bmp](./assets/media/image346.png)

**ATTENZIONE!** un **"Importo" nullo** all'interno della maschera di
**"Pagamento Web"** è da considerarsi come indice di una **procedura di
pagamento on line, sulla relativa prenotazione, terminata in maniera
anomala**.

Sarà quindi compito del gestore, in situazioni di questo tipo,
verificare, direttamente all'interno dell'applicazione di Back Office
della banca, se il pagamento è avvenuto o meno, e comportarsi poi di
conseguenza relativamente alla prenotazione inserita nel gestionale.

**In ogni caso, alla conferma e/o all'annullamento di una prenotazione
all'interno del gestionale, il gestionale stesso, se correttamente
configurato, potrà inviare all'utente apposite notifiche via mail e/o
via sms sullo stato della prenotazione.**

> **NOTA BENE:** per maggiori informazioni relativamente a come
> configurare le varie notifiche mail e/o sms sul gestionale si rimanda
> allo specifico manuale.

