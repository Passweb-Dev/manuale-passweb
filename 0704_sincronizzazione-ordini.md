# SINCRONIZZAZIONE ORDINI



Per quel che riguarda i documenti (ordini, preventivi, bolle, fatture
ecc...) è bene sottolineare come questi siano gestiti, a livello di
sincronizzazione, in maniera leggermente differente rispetto a quanto
precedentemente visto per i clienti, gli articoli, le particolarità o i
dati delle tabelle accessorie.

Nello specifico occorre infatti considerare le seguenti regole di base:

- **L'inserimento sul gestionale di nuovi ordini effettuati all'interno
  del sito non richiede, di base, nessun tipo di sincronizzazione**.

> L'unica condizione per poter effettuare questo tipo di operazione
> infatti, è che il gestionale sia correttamente esposto e contattabile
> via internet nel momento in cui il cliente effettua l'ordine sul sito.
> In queste condizioni l'inserimento del nuovo ordine (ed eventualmente
> della nuova anagrafica cliente) sul gestionale avverrà in maniera
> immediata e completamente automatica senza il bisogno di interventi da
> parte dell'amministratore del sito e soprattutto senza scalere le
> sincronizzazioni previste da contratto.

- **Nel caso in cui al momento della creazione del nuovo ordine il
  gestionale, per diverse ragioni, non sia contattabile, l'ordine
  resterà memorizzato sul database del sito e potrà essere inserito nel
  gestionale in maniera manuale lanciando una "Sincronizzazione
  Parziale".**

> Anche in questo caso non verranno sottratte sincronizzazioni a quelle
> previste da contratto. Si ricorda però che la Sincronizzazione
> Parziale si occupa unicamente di inserire nuovi ordini e o nuove
> anagrafiche cliente. A seguito di questa operazione non verrà quindi
> prelevato dal gestionale nessun altro tipo di dato.

- **Nel caso in cui siano state apportate delle variazioni, lato
  gestionale, a documenti gestiti sul web queste potranno essere
  correttamente riportate anche all'interno del sito solo ed
  esclusivamente a seguito di una Sincronizzazione per Variati o ad una
  Ricostruzione Totale**

##### MEXAL -- ESPORTAZIONE DI DOCUMENTI CREATI DA GESTIONALE

Sui documenti Mexal (**Ordini, Bolle, Fatture, Preventivi, Matrici**)
non è gestita, a differenza di quanto visto per articoli, clienti e
particolarità una data di ultima modifica.

**Ciò che determina dunque se un documento dovrà o meno essere esportato
e gestito su uno dei 9 diversi possibili siti collegati alla stessa
azienda Mexal, è esattamente quanto indicato all'interno della maschera
"Stato Anagrafiche" del relativo documento,** maschera questa
accessibile cliccando sul pulsante "**Stato**" o, in alternativa, con il
tasto funzione "S**hift + F11**" dopo aver posizionato il cursore sul
campo "**Documento**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\multi_sito_ec19.bmp](./assets/media/image198.png)

In particolare:

- Lo slot **Attivo** determina se il relativo documento dovrà o meno
  essere gestito anche all'interno del sito.

> Ovviamente **per documenti nati all'interno di uno dei 9 siti**
> collegati alla stessa azienda Mexal, questo slot sarà impostato di
> default sul **valore S** mentre **per documenti nati all'interno del
> gestionale** sarà impostato di default sul **valore N**.
>
> In ogni caso l'utente avrà sempre la possibilità di variare
> manualmente questo valore a seconda del fatto di voler rendere
> disponibile o meno uno specifico documento anche sul web.

- Lo slot **NumSitoWeb** consente invece di specificare su quale dei 9
  diversi possibili siti collegati alla stessa azienda Mexal dovrà
  eventualmente essere esportato il documento in esame.

> Ovviamente nel caso in cui il documento sia stato generato a partire
> da uno dei 9 siti collegati alla stessa azienda Mexal il campo in
> esame sarà già valorizzato a default con il numero del relativo sito.
> In ogni caso l'utente avrà sempre la possibilità di variare
> manualmente questo valore e di decidere quindi su quale dei 9 siti
> esportare il documento
>
> **ATTENZIONE! In ogni caso ciascun documento potrà essere esportato e
> gestito solo ed esclusivamente in un sito alla volta. Non è quindi
> possibile esportare lo stesso documento su due siti differenti (seppur
> collegati alla stessa azienda)**
>
> Va detto anche che, lato gestionale, il numero di sito rappresenta, in
> relazione alla possibilità di fusione di due o più documenti diversi,
> un elemento di rottura (allo stesso modo ad, esempio dell'intestatario
> del documento o del pagamento adottato).
>
> **In altri termini quindi non è possibile fondere tra loro in un unico
> documento, singoli documenti associati a siti differenti oppure
> documenti associati ad uno specifico sito con documenti non associati
> ad alcun sito.**

- Lo slot **Variato** indica se sono state apportate o meno variazioni
  al documento in oggetto. Tale flag è gestito in automatico
  dall'applicativo ed è sufficiente effettuare un semplice F10 sul
  documento per passare il suo valore da N a S.

**Nota Bene:** nel caso in cui l'esigenza sia quella di modificare in
blocco questi parametri per un numero elevato di documenti si consiglia
di agire via sprix attraverso le variabili \_**MMMRA\$, \_MMMRV\$** e
**\_MMIDPASSWEB**

Ogni volta che viene eseguita una sincronizzazione con uno dei 9 siti
collegati alla stessa azienda Mexal, indipendentemente dal fatto che sia
una Ricostruzione Totale o una Sincronizzazione per Variati, verranno
dunque processati tutti i documenti (ordini, bolle, fatture ...) per i
quali il flag Attivo sopra evidenziato è impostato a S e che hanno,
ovviamente, nel campo NumSitoWeb il numero del sito con cui si sta
effettuando la sincronizzazione.

Tra questi verranno poi esportati e/o aggiornati sul sito solo ed
esclusivamente quei documenti per cui anche il flag Variato risulta
impostato sul valore S.

Supponiamo ora di aver attivato il nostro sito Ecommerce e di aver
correttamente esportato da Mexal articoli e soprattutto clienti.

Generalmente in queste condizioni potrebbe anche essere necessario
importare all'interno del sito la situazione ordini pregressa dei
clienti Mexal che si è deciso di gestire su quello stesso sito.

Come detto infatti un ordine effettuato e gestito interamente da Mexal
non viene esportato, a default, per cui il relativo intestatario,
sebbene in grado di accedere al sito, non avrà comunque alcuna
possibilità di visualizzarlo all'interno della propria sezione "Stato
Ordini", almeno fintanto che l'operatore Mexal non decida
volontariamente di esportarlo.

In questo senso la procedura da seguire per poter esportare e gestire
all'interno del sito web anche gli ordini generati direttamente in Mexal
(attraverso l'apposita maschera di Emissione/Revisione Documenti) sarà
esattamente la seguente:

1.  Richiamare, all'interno della maschera di Emissione/Revisione
    Documenti del gestionale, lo specifico documento generato da Mexal
    che si intende esportare all'interno del sito

2.  Portarsi sul campo **"Documento"** e cliccare sul pulsante **"Stato"
    (Shift + F11)** in maniera tale da accedere alla maschera "**Stato
    Anagrafiche**" precedentemente esaminata.

3.  Impostare il flag **ATTIVO** sul valore **S** (a default il valore è
    **'N'**)

4.  Indicare all'interno del campo **NumSitoWeb** il numero del sito
    verso cui si vuole esportare il documento (F2 su questo campo apre
    la maschera di selezione visuale dei siti).

5.  Lanciare una sincronizzazione (per variati o ricostruzione totale
    non fa differenza) o attendere la prossima sincronizzazione
    schedulata in modo tale da consentire a Passweb di leggere il nuovo
    valore dei parametri in oggetto e di poter così prelevare il
    relativo documento.

**NOTA BENE:** potranno essere esportati e conseguentemente visualizzati
sul sito solo ed esclusivamente quei documenti Mexal la cui data ricade
all'interno dell'intervallo temporale impostato attraverso il parametro
**"Periodo di Visualizzazione Documenti"** presente alla pagina
**"Gestione Ordini"** del Wizard .

Una volta esportato sul sito in maniera corretta un documento generato
da Mexal, questo stesso documento potrà essere visualizzato ed
eventualmente gestito dal relativo intestatario all'interno della
propria sezione "Stato Ordini".

Questo stesso documento, dipendentemente dalla sua tipologia, comparirà
anche all'interno di una delle maschere presenti nelle sezioni "Gestione
Ordini", "Gestione Resi" e/o "Gestione Matrici" del back end di Passweb.

**ATTENZIONE!!** Esportando un ordine da Mexal all'interno del sito
potrebbe verificarsi una situazione in cui all'interno di questo stesso
ordine siano presenti articoli non più gestiti sul sito.

**In queste condizioni modificando l'ordine in esame eventuali articoli
in esso contenuti e non gestiti all'interno del sito verrebbero
eliminati dall'ordine e tale variazione, alla successiva
sincronizzazione verrebbe anche riportata all'interno del gestionale**

Infine, per poter eliminare dal sito, ad esempio uno specifico ordine,
indipendentemente dal fatto che esso sia nato in Mexal o in Passweb,
sarà necessario:

1.  Richiamare, all'interno della maschera di Emissione/Revisione
    Documenti del gestionale, il documento in esame

2.  Portarsi sul campo **"Documento"** e cliccare sul pulsante **"Stato"
    (Shift + F11)** in maniera tale da accedere alla maschera "**Stato
    Anagrafiche**"

3.  Impostare il flag **ATTIVO** sul valore **N**, evitando così di
    esportarlo nuovamente alla prossima sincronizzazione

4.  Portarsi nella maschera **"Lista Ordini"** di Passweb, accessibile
    dal menu *"Ordini -- Gestione Ordini"*

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\lista_ordini.bmp](./assets/media/image199.png)

> selezionare il documento in esame ed eliminarlo cliccando sul apposito
> pulsante **"Elimina Ordine"** ( ) presente nella barra degli
> strumenti.

**NOTA BENE**: a differenza di quanto avviene per articoli e clienti la
sincronizzazione (sia essa per variati o una ricostruzione totale) non
elimina automaticamente nessun ordine per cui, per completare
l'operazione, è necessario che l'ordine in questione venga eliminato
manualmente anche dalla lista ordini presente nel back end di Passweb

##### HO.RE.CA. -- ESPORTAZIONE DI ORDINI/PRENOTAZIONI CREATI DA GESTIONALE

Nel caso di siti Ecommerce collegati ad uno dei gestionali Ho.Re.Ca.
l'operazione di esportazione ordini e/o prenotazioni dal sito sul
gestionale funziona in maniera leggermente diversa rispetto a quanto
visto nel caso di siti Ecommerce collegati a Mexal.

In queste condizioni occorre infatti considerare che al momento della
prima sincronizzazione Passweb non prenderà in considerazione nessuno
degli ordini e/o delle prenotazioni presenti in quello stesso momento
all'interno del gestionale, in modo tale da non dover importare, a
default, tutta la situazione pregressa di ordini e/o prenotazioni.

A partire dalla successiva sincronizzazione verranno invece prelevati ed
importati all'interno del sito, in maniera completamente automatica,
tutti gli ordini, le bolle, le fatture e/o le prenotazioni che risultino
essere variati rispetto all'ultima sincronizzazione terminata
correttamente, e la cui data ricada all'interno dell'intervallo
temporale impostato attraverso il parametro **"Periodo di
Visualizzazione Documenti"** presente alla pagina **"Gestione Ordini"**
del Wizard.

Nel caso in cui l'esigenza dovesse quindi essere quella di esportare
all'interno del sito tutti gli ordini e/o le prenotazioni attualmente
presenti sul gestionale, sarà necessario (dopo aver effettuato la prima
sincronizzazione) variare tutti questi documenti (lato gestionale) e
lanciare poi una nuova sincronizzazione.

**ATTENZIONE!** Nel caso in cui si vogliano esportare dal gestionale
verso il sito web dei documenti (ordini/bolle/fatture) in cui
l'indirizzo di spedizione codificato nel piede è quello di un punto
vendita gestito anche all'interno del sito, è necessario prestare
particolare attenzione al fatto che l'indirizzo presente nel piede del
documento coincida esattamente, in tutte le sue parti, con uno degli
indirizzi dei punti vendita codificati anche all'interno del sito.

In caso contrario non potendo individuare, all'interno di Passweb il
punto vendita desiderato, le relative informazioni andranno perse e non
saranno quindi visualizzate all'interno del sito.

