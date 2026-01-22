# CREAZIONE E GESTIONE DI UN RESO MERCE



Per poter effettuare una richiesta di reso merce, correlata ovviamente
ad una certa fattura e/o corrispettivo, il cliente (o l'Agente per suo
conto) dovrà per prima cosa autenticarsi sul sito e portarsi alla pagina
"Ordini" dove potrà visualizzare, come noto, l'elenco di tutti i suoi
documenti (ordini, bolle, fatture ecc...)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gestione_resi1.bmp](./assets/media/image747.png)

Portandosi nella sezione relativa alle fatture l'utente avrà quindi modo
di visualizzare l'elenco di tutti i documenti a partire dai quali
possono, eventualmente, essere generate delle richieste di reso merce.

**Nel momento in cui, infatti, la data di una fattura (e/o di un
corrispettivo) rientri nell'intervallo di giorni entro cui poter
effettuare una richiesta di reso merce** (parametro questo impostato
all'interno della maschera di "**Configurazione Resi**" precedentemente
analizzata) comparirà, in corrispondenza di questo stesso documento,
oltre al pulsante di visualizzazione del dettaglio, anche il pulsante
grazie al quale poter avviare una nuova richiesta di reso merce.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gestione_resi2.bmp](./assets/media/image748.png)

Cliccando su questo pulsante (il cui testo può essere personalizzato
dalla sezione "*Testi / Messaggi del Sito*") l'utente verrà quindi
ridiretto alla pagina "**Reso**" del sito dove, grazie alla presenza
dell'apposito componente Passweb, avrà modo di configurare la sua
richiesta (per maggiori informazioni relativamente al componente Passweb
utilizzato per la creazione di una richiesta di reso merce si veda anche
la corrispondente sezione di questo manuale *"Lista Componenti Ecommerce
-- Componente Reso Custom"*).

All'interno di questa pagina verrà infatti visualizzato il dettaglio
della fattura (o del corrispettivo) in relazione alla quale effettuare
la richiesta di reso merce

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gestione_resi3.bmp](./assets/media/image749.png)

Nel dettaglio del documento verranno inoltre considerati i soli articoli
in relazione ai quali è effettivamente possibile richiedere il reso
merce.

**ATTENZIONE!** Non è possibile effettuare richieste di reso merce in
relazione ad articoli di tipo "Gift Card"

Allo stesso modo non verranno visualizzati, o quantomeno saranno ridotti
in termini di quantità, tutti gli articoli per i quali esiste già una
richiesta di reso fatta a partire dalla medesima fattura (o dal medesimo
corrispettivo)

Inoltre a differenza della fattura di origine, dove eventuali articoli a
taglie sono raggruppati in un'unica riga, **nella richiesta di reso
merce verrà visualizzata una riga per ogni singola taglia** dando quindi
all'utente la possibilità di selezionare in maniera puntuale lo
specifico articolo ed eventualmente anche la specifica taglia in
relazione alla quale richiedere il reso.

L'utente dovrà quindi selezionare, utilizzando per questo l'apposito
check, l'articolo o gli articoli per i quali effettuare la richiesta di
reso merce, indicando per ciascuno di essi l'esatta quantità (**che
ovviamente non potrà essere nulla, negativa o maggiore a quella presente
in fattura**) ed eventualmente una specifica nota (di riga e/o di
corpo).

**ATTENZIONE!** La nota di riga è gestita solo per i siti Ecommerce
collegati a Mexal. Quella di corpo è disponibile invece tanto per i siti
Ecommerce collegati a Mexal quanto per quelli collegati ad uno dei
gestionali Ho.Re.Ca.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gestione_resi6.bmp](./assets/media/image750.png)

**ATTENZIONE!** **i campi di input per l'inserimento della quantità e/o
della nota di riga verranno visualizzati solo dopo aver selezionato
l'articolo per il quale si intende effettuare una richiesta di reso
merce**.

E' inoltre possibile indicare selezionare anche uno specifico valore,
tra quelli proposti, per l'Aspetto Esteriore dei Beni (Ecommerce Mexal).

**ATTENZIONE!** **Il combo box di selezione per l'aspetto esteriore dei
beni è visualizzato solo ed esclusivamente nel caso in cui siano state
impostate delle specifiche descrizioni nella corrispondente tabella
Mexal (*Magazzino -- Tabelle Aziendali -- Aspetto Esteriore dei Beni*)**

Accettando quindi i termini e le condizioni di restituzione merce e
cliccando sul pulsante "**Conferma**" la richiesta di reso merce verrà
memorizzata nel database del sito nello stato **DA VERIFICARE**. (Le
condizioni di restituzione merce possono essere editate all'interno
della sezione Testi / Messaggi Sito del Wizard)

Contestualmente a questa fase verranno inviate due mail, una al cliente
e/o all'agente intestatario del documento di partenza (E-Mail di Invio
Reso) contente i dettagli della richiesta appena effettuata, e una
all'amministratore del sito (E-Mail di Informazioni di Invio Reso) per
notificargli l'acquisizione di questa nuova richiesta.

L'amministratore dovrà quindi accedere al Wizard del sito, portarsi
nella sezione "*Ordini -- Gestione Resi*", selezionare, tra le richieste
presenti in elenco quella in relazione alla quale ha appena ricevuto la
mail di notifica e visualizzarne il dettaglio, cliccando per questo sul
pulsante "**Visualizza Reso**".

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gestione_resi5.bmp](./assets/media/image741.png)

In questa fase, come precedentemente evidenziato, l'amministratore avrà
la possibilità di modificare le quantità (**che non potranno essere mai
superiori a quelle inserite dal cliente stesso in fase di creazione
della sua richiesta di reso**), le note e l'aspetto esteriore dei beni
e, soprattutto, avrà la possibilità di variare lo stato decidendo quindi
se approvare o meno la specifica richiesta.

In particolare per approvare la richiesta in oggetto, il suo stato dovrà
essere impostato sul valore **CONFERMATO**; nel caso in cui invece la
richiesta debba essere rifiutata il suo stato andrà impostato sul valore
**ANNULLATO**.

Il pulsante **Salva**, presente nella parte bassa di questa maschera,
consente di salvare in maniera definitiva le variazioni apportate alla
richiesta di reso merce e, nel caso, di inviare anche la mail di
"Conferma Reso" o quella di "Rifiuto Reso" per informare il cliente
della decisione presa in merito alla sua richiesta di reso merce.

A questo punto nel caso in cui la richiesta sia stata rifiutata, potrà
tranquillamente essere eliminata dal database del sito (pulsante
"Elimina Reso").

Nel caso in cui invece sia stata approvata il cliente potrà
visualizzarla alla pagina "Ordini" del sito nella sezione riservata ai
Resi.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gestione_resi8.bmp](./assets/media/image751.png)

Pur essendo stata approvata, la richiesta di reso merce si trova però
ancora solo sul database del sito, per cui sarà ora necessario inserirla
all'interno del gestionale in maniera tale da poterla effettivamente
elaborare.

Per far questo è sufficiente selezionarla tra quelle presenti in elenco
e cliccare sul pulsante "**Memorizza Reso**"
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_memorizza_reso.bmp](./assets/media/image752.png) ) che, come precedentemente evidenziato,
viene effettivamente visualizzato solo ed esclusivamente per richieste
in stato **CONFERMATO**

Cliccando su questo pulsante verrà infatti avviata una sincronizzazione
parziale (**non scalata dal monte sincronizzazioni previsto da
contratto**) a seguito della quale verrà registrato sul gestionale,
dipendentemente da quanto impostato nella maschera di Configurazione dei
Resi precedentemente esaminata, un documento **RC** o **NC**.

Infine una volta elaborato il documento all'interno del gestionale, ed
eventualmente trasformata la richiesta di reso (RC) in Nota d'Accredito
(NC) sarà sufficiente attendere la prossima sincronizzazione per
riportare tale variazione anche all'interno del sito.

Contestualmente alla sincronizzazione durante la quale viene riportata
sul sito la Nota d'Accredito, verrà anche inviata al cliente
un'ulteriore mail per informarlo dell'avvenuto accredito.

Ricevuta tale mail l'utente potrà quindi accedere nuovamente alla pagina
"Ordini" del sito e visualizzare, all'interno della sezione
"**Crediti**". il dettaglio della sua nota d'accredito.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gestione_resi9.bmp](./assets/media/image753.png)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gestione_resi10.bmp](./assets/media/image754.png)

> **NOTA BENE:** qualora in fase di sincronizzazione dovessero essere
> presenti delle richieste di reso merce in stato DA VERIFICARE, verrà
> inviata un'apposita mail di notifica all'amministratore del sito.

**ATTENZIONE! il dettaglio dei documenti di tipo NC (Note d'Accredito)
verrà visualizzato all'interno della pagina Ordine. Il dettaglio dei
documenti di tipo RC (Reso Merce) verrà invece visualizzato all'interno
della pagina Reso.**

In conseguenza di ciò le informazioni presenti nel dettaglio delle note
di accredito dipenderanno direttamente dal componente Ordine / Ordine
Custom e da come si è deciso di configurarlo.

Le informazioni presenti nel dettaglio dei documenti RC dipenderanno
invece direttamente dal componente Reso (RMA) / Reso Custom (RMA) e da
come si è deciso di configurarlo.

