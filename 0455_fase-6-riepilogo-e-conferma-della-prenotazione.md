# FASE 6 -- RIEPILOGO E CONFERMA DELLA PRENOTAZIONE



Durante quest'ultimo step l'utente avrà la possibilità di visualizzare
un riepilogo dei dati della propria prenotazione e potrà quindi decidere
di confermarla in maniera definitiva effettuando, nel caso anche il
pagamento online.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\spiagge_configurazione_19.bmp](./assets/media/image390.png)

Una volta revisionati i dati della prenotazione, cliccando sul pulsante
**"Conferma"** il comportamento dell'applicazione sarà differente a
seconda della modalità di pagamento precedentemente selezionata
dall'utente.

In particolare **nel caso in cui il pagamento selezionato durante lo
step precedente dovesse essere un pagamento non immediato** (es.
contanti all'arrivo in struttura) la prenotazione verrà inserita
all'interno del gestionale in stato di **"Preventivo"**.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\spiagge_configurazione_23.bmp](./assets/media/image391.png)

In queste condizioni

- **il gestore dovrà decidere di confermare o, eventualmente, annullare
  la prenotazione direttamente all'interno del gestionale**
  (configurando magari il gestionale in modo tale che mandi apposita
  notifica al cliente)

- **fintanto che il gestore non avrà deciso se accettare o meno la
  prenotazione l'utente avrà sempre la possibilità di annullarla
  operando dalla pagina "Le mie prenotazioni" del sito**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\spiagge_configurazione_25.bmp](./assets/media/image392.png)

> Per le prenotazioni in stato di "Preventivo" è infatti presente oltre
> al pulsante "Visualizza" anche il pulsante "**Annulla**". Nel momento
> in cui l'utente dovesse quindi decidere di annullare la sua
> prenotazione cliccando sul relativo pulsante, questa verrà
> immediatamente posta, all'interno del gestionale, nello stato di
> "**Mancata**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\spiagge_configurazione_26.bmp](./assets/media/image393.png)

> **ATTENZIONE!** potranno essere annullate da sito solo ed
> esclusivamente prenotazioni in stato "Preventivo" che non risultino
> essere dunque già state pagate

Nel momento in cui **il pagamento selezionato durante lo step precedente
dovesse invece essere un pagamento on line** (es. Carta di credito) il
comportamento dell'applicazione sarà completamente diverso.

In questo caso infatti, una volta approvate le condizioni di vendita
cliccando sul pulsante **"Conferma"** la prenotazione verrà inserita
all'interno del gestionale, dove verrà memorizzata nello stato di
**"Confermata"** e, **contemporaneamente,** l'utente verrà ricondotto
sul sito del gateway di pagamento per portare a termine la transazione.

**Inoltre alla conferma della prenotazione sul sito, prima che questa
stessa prenotazione venga effettivamente inserita nel gestionale e
l'utente rediretto sul gateway di pagamento, verranno avviati dei
controlli su eventuali situazioni di overbooking**.

Nel caso in cui, dunque, si dovesse verificare per la prenotazione via
web una situazione di overbooking, subito dopo aver cliccato sul
pulsante "Conferma" verrà visualizzato un apposito messaggio di avviso e
la relativa prenotazione **non sarà inserita nel gestionale**.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\spiagge_configurazione_20.bmp](./assets/media/image394.png)

**ATTENZIONE! In ogni caso considerando che, a meno di overbooking, la
prenotazione verrà effettivamente inserita nel gestionale prima ancora
che l'utente abbia effettivamente completato il pagamento**, occorre
porre particolare attenzione alle possibili casistiche generate dalla
procedura di pagamento stessa.

In particolare nel caso in cui la procedura di pagamento venga portata a
termine in maniera corretta (l'utente passa attraverso tutti i vari step
proposti dal gateway di pagamento, inserendo quindi tutti i dati
richiesti e tornando alla fine sul sito Passweb), il gateway di
pagamento invierà a Passweb una risposta positiva sull'esito della
transazione per cui alla ricezione di questa risposta Passweb si
preoccuperà di inserire all'interno del gestionale il corrispondente
importo pagato.

Lato gestionale, l'esercente potrà quindi verificare questi dati
portandosi nella maschera "**Pagamento Web**" attivabile dall'omonima
voce presente nel contesto della relativa prenotazione

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\spiagge_configurazione_21.bmp](./assets/media/image395.png)

**Nel caso in cui entrambi i campi (Tipo di pagamento e Importo) della
maschera "Pagamento Web" sopra evidenziata siano correttamente
valorizzati, la relativa prenotazione web potrà ritenersi correttamente
pagata.**

**ATTENZIONE**! Se, al momento dell'inserimento nel gestionale
dell'importo effettivamente pagato, Passweb non dovesse riuscire per
qualche ragione a contattare il gestionale, verrà inviata immediatamente
una mail agli indirizzi configurati all'interno del campo "Indirizzi per
la Email di informazione" della pagina "Configurazione Ordini" del
Wizard, per informare chi di dovere che la prenotazione il cui codice
gestionale è inserito all'interno della mail stessa è stata
correttamente pagata.

Nel caso in cui, invece, durante una delle fasi di pagamento, l'utente
dovesse per qualsiasi ragione annullare la transazione cliccando sul
relativo pulsante di annullamento, il gateway di pagamento si
preoccuperà di reindirizzare l'utente stesso al sito di partenza
inviando anche a Passweb, in relazione al pagamento in questione, una
risposta negativa.

**Una volta ricevuta questa risposta negativa Passweb stesso si
preoccuperà di comunicarla al gestionale Ho.Re.Ca. ponendo la relativa
prenotazione (comunque già presente nel gestionale) nello stato di
"Mancata".**

Infine nel caso in cui la procedura di pagamento dovesse essere
interrotta dall'utente in maniera anomala (ad esempio chiudendo il
browser indipendentemente dal fatto di aver completato o meno la
transazione), il gateway di pagamento non avrebbe modo di inviare a
Passweb alcuna risposta relativamente al pagamento in questione.

In assenza quindi di risposte positive o negative che siano, Passweb non
potrà avere coscienza dell'esito della transazione per cui, considerando
anche che la prenotazione in questa fase si trova comunque già
all'interno del gestionale, non potrà ne considerare il pagamento andato
a buon fine (inserendo il corrispondente importo pagato all'interno del
gestionale) ne tanto meno considerare la relativa prenotazione come
annullata.

**In queste condizioni quindi le cose verranno lasciate esattamente come
sono, ossia con la prenotazione inserita all'interno del gestionale
nello stato di "Confermata" e la maschera di "Pagamento Web" con importo
nullo.**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\spiagge_configurazione_22.bmp](./assets/media/image396.png)

**ATTENZIONE!** Un **"Importo" nullo** all'interno della maschera di
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
> allo specifico manuale di prodotto.

