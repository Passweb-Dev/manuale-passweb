# SINCRONIZZAZIONE LANCIATA DA PASSWEB



Operando direttamente all'interno del Wizard di Passweb e, nello
specifico, dalla maschera "**Parametri Sincronizzazione**", accessibile
dalla voce di menu **"Configurazione - Sincronizzazione",** è possibile
gestire "**Sincronizzazioni Totali**", "**Sincronizzazioni per
Variati**" e "**Sincronizzazioni Parziali**".

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsanti_sincronizzazione.bmp](./assets/media/image182.png){width="5.954861111111111in"
height="3.532638888888889in"}

In particolare **le Sincronizzazioni Totali e quelle Parziali potranno
essere lanciate solo ed esclusivamente in maniera manuale** cliccando
per questo sui relativi pulsanti (**Sincronizzazione Totale** e
**Sincronizzazione Parziale**)

Per quel che riguarda invece le **Sincronizzazioni per Variati**, queste
potranno essere schedulate a precisi intervalli di tempo oppure
lanciate, anch'esse, in maniera manuale (pulsante **Sincronizzazione
Standard**).

Nel caso in cui si desideri schedulare questo tipo di operazione
occorrerà quindi indicare, per prima cosa, con che frequenza dovrà
essere effettuata.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sincronizzazione_variati_1.bmp](./assets/media/image183.png){width="5.954861111111111in"
height="3.532638888888889in"}

E' possibile decidere di eseguire quest'operazione ogni N giorni e in
corrispondenza di specifici giorni della settimana, indicando
eventualmente, anche l'esatto intervallo orario entro cui dover operare.

I giorni selezionati con il relativo segno di spunta sono i giorni
ammessi; pertanto se si volesse ad esempio evitare di lanciare
sincronizzazioni il fine settimana occorrerà togliere il segno di spunta
in corrispondenza dei giorni "Sabato" e "Domenica".

**NOTA BENE**: il controllo sui giorni della settimana viene effettuato
unicamente dal servizio di sincronizzazione automatica. Nulla vieta
all'utente di poter avviare una sincronizzazione manuale in qualsiasi
momento.

**NOTA BENE**: è possibile schedulare solo ed esclusivamente le
Sincronizzazioni per Variati.

**ATTENZIONE! Le Sincronizzazioni Parziali avvengono con un processo
separato da quello utilizzato per gestire le Sincronizzazioni Totali o
per Variati per cui è possibile eseguire una Sincronizzazione Parziale
contemporaneamente ad una Totale o per Variati. Non è invece possibile
eseguire contemporaneamente una Sincronizzazione Totale ed una per
Variati**

Gli altri parametri presenti all'interno della sezione "**Generali**",
variabili in relazione al fatto di considerare siti collegati a Mexal o
ad uno dei gestionali Ho.Re.Ca., consentono rispettivamente di:

- **E-Mail**: consente di specificare uno o più indirizzi di posta
  elettronica (eventualmente separati dal carattere ';') cui dovrà
  essere inviata, ad operazione terminata, una notifica contenente
  l'esito della sincronizzazione (ovviamente questa funzionalità sarà
  attivata solamente nel caso in cui si sia deciso di attivare la
  gestione delle mail, indicando per questo un indirizzo di posta valido
  alla pagina "Posta/SMS" del Wizard).

- **Tipo di sincronizzazione --** **presente solo nel caso di siti
  Ecommerce collegati ad uno dei gestionali Ho.Re.Ca.:** consente di
  impostare il tipo di sincronizzazione che dovrà essere eseguita
  durante le sincronizzazioni schedulate.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\horeca_tipo_sincronizzazione.bmp](./assets/media/image184.png){width="5.675in"
height="3.4090277777777778in"}

> E' possibile selezionare uno dei seguenti valori:

- **Totale:** selezionando questa opzione ogni sincronizzazione
  schedulata sarà una sincronizzazione Totale. Verranno quindi importati
  tutti gli articoli correttamente marcati all'interno del gestionale,
  tutti i clienti e verranno anche eseguite eventuali operazioni di
  cancellazione in relazione ad articoli non più presenti sul gestionale
  e/o marcati per non essere più gestiti all'interno del sito.

> Per quel che riguarda le risorse articolo, in queste condizioni
> verranno importate eventuali immagini relative ai soli prodotti
> "nuovi" che non sono cioè ancora presenti nel database Passweb.

- **Variati**: selezionando questa opzione ogni sincronizzazione
  schedulata sarà una sincronizzazione per Variati. Verranno quindi
  importati solo ed esclusivamente gli articoli e i clienti che
  risulteranno essere stati variati, lato gestionale, rispetto
  all'ultima sincronizzazione terminata correttamente. NON verranno
  effettuate operazioni di cancellazione articoli e/o clienti.

> Per quel che riguarda invece le risorse articolo, indipendentemente
> dal fatto di aver impostato il parametro in esame sul valore "Totale"
> o "Variati", a seguito di ogni sincronizzazione schedulata verranno
> importate sempre le risorse (immagini e schede tecniche) relative a
> prodotti nuovi (e che non erano quindi già presenti in Passweb) mentre
> l'eventuale importazione delle risorse relative a prodotti già
> esportati, e quindi già presenti nel database di Passweb, dipenderà da
> come sono stati settati i due campi "**Tabella Articoli**" e
> "**Tabella Categorie Merceologiche**" presenti in corrispondenza del
> parametro "**Aggiornamento file da Gestionale (Variati)**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\horeca_aggiornamento_file_gestionale.bmp](./assets/media/image185.png){width="3.779166666666667in"
height="0.34444444444444444in"}

> Per maggiori informazioni in merito si vedano anche i successivi
> capitoli di questo manuale.

- **Pubblica articoli precancellati o annullati logicamente --**
  **presente solo nel caso di siti Ecommerce collegati a Mexal:**
  consente, se selezionato, di pubblicare normalmente all'interno del
  proprio sito anche articoli che, lato gestionale sono stati
  precancellati e/o annullati logicamente (e che hanno ancora comunque
  il campo "Trasferisici sul sito" impostato a S).

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\importa_precancellati.bmp](./assets/media/image186.png){width="5.954861111111111in"
height="3.532638888888889in"}

> Nel caso in cui il parametro in oggetto non dovesse essere
> selezionato, eventuali articoli precancellati e/o annullati
> logicamente (e che hanno ancora comunque il campo "Trasferisici sul
> sito" impostato a S) verranno invece spubblicati in fase di
> sincronizzazione (il campo "Pubblica" di tali articoli verrà posto
> automaticamente a N).
>
> **ATTENZIONE! In quest'ultimo caso gli articoli precancellati e quindi
> non pubblicati sul sito, saranno comunque articoli presenti sul
> database e verranno quindi conteggiati nel numero complessivo degli
> articoli previsti da contratto**
>
> Nel caso in cui l'esigenza dovesse essere quella di eliminare dal sito
> tali articoli in maniera definitiva sarà quindi necessario impostare,
> lato gestionale, il parametro "Trasferisici sul sito" a N.
>
> **ATTENZIONE!** Il parametro "**Pubblica articoli precancellati o
> annullati logicamente**" ha effetto, ovviamente, sia per le
> Sincronizzazioni Standard (per Variati) che per le Sincronizzazioni
> Totali

- **Importa Articoli non attivi --** **presente solo nel caso di siti
  Ecommerce collegati ad uno dei gestionali Ho.Re.Ca.:** consente, se
  selezionato, di importare e gestire sul sito anche articoli che, lato
  gestionale sono stati correttamente abilitati (parametro "**Abilita
  Passweb**" correttamente selezionato) ma che risultano attualmente
  "Non attivi" e che sono quindi fuori dall'intervallo definito dai due
  campi "**Inizio validità**" e "**Fine Validità**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\validita_articoli_horeca.bmp](./assets/media/image187.png){width="4.785416666666666in"
height="3.123611111111111in"}

> **ATTENZIONE!** L' "attivazione" di un articolo viene considerata ad
> ogni sincronizzazione
>
> Nel caso in cui si sia deciso di non importare gli articoli "non
> attivi" (parametro "Importa Articoli non attivi" non selezionato) e
> qualora, lato gestionale, dovesse essere impostato per determinati
> articoli un preciso intervallo di validità occorrerà considerare
> quanto segue:

- durante la prima sincronizzazione l'articolo marcato come "non attivo"
  non verrà importato all'interno del sito

- durante le successive sincronizzazioni la valutazione relativa alla
  "validità" dell'articolo verrà effettuata, se le sincronizzazione
  eseguita è una "sincronizzazione per variati", solo nel caso in cui
  l'articolo stesso risulti essere variato rispetto all'ultima
  sincronizzazione utile. Se la sincronizzazione eseguita è invece una
  "sincronizzazione totale" la valutazione relativa alla validità verrà
  comunque effettuata per tutti gli articoli

- nel caso in cui l'articolo in esame dovesse essere gestito sul sito (e
  quindi già presente all'interno del database di Passweb) e alla
  valutazione della "validità" l'articolo stesso dovesse risultare "non
  attivo" verrà rimosso anche dal database del sito

<!-- -->

- **Importa risorse articoli (solo se automatica e Mexal \>= v.851) --
  presente solo nel caso di siti Ecommerce collegati a Mexal** :
  consente di automatizzare la procedura di importazione delle risorse
  articolo.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\schedulazione_importa_risorse.bmp](./assets/media/image188.png){width="5.643055555555556in"
height="3.5in"}

> Selezionando questo parametro infatti **a seguito di ogni
> sincronizzazione schedulata** verrà eseguita automaticamente anche la
> procedura di importazione risorse utilizzando, come data di ultima
> importazione, quella indicata all'interno dell'apposito campo (data
> questa che verrà poi aggiornata automaticamente al termine della
> procedura stessa)
>
> **ATTENZIONE!** Il parametro in esame avrà effetto solo ed
> esclusivamente per versioni Mexal maggiori o uguali alla 2023H (v.851)
>
> Nel momento in cui si dovesse decidere di flaggare questo parametro si
> consiglia sempre di verificare attentamente di non aver attivato, lato
> gestionale, procedure automatiche (es. sprix) che possano in qualche
> modo variare la data di ultima modifica di un'immagine prodotto senza
> che questa stessa immagine venga effettivamente sostituita.
>
> In caso contrario infatti potrebbero configurarsi situazioni in cui a
> seguito di una sincronizzazione automatica verrebbero reimportate
> immagini e/o risorse articolo che di fatto sono già presenti
> all'interno del sito allungando quindi inutilmente i tempi di
> sincronizzazione

Infine, il parametro "**Aggiornamento descrizioni in ... dal
Gestionale**" consente di indicare quali tabelle accessorie (Mexal o
Ho.Re.Ca.) dovranno essere prese in considerazione in fase di
sincronizzazione (per Variati o Totale) al fine di aggiornare la
descrizione, nella lingua indicata, dei relativi campi.

**ATTENZIONE!** Per le tabelle indicate verranno aggiornate solo ed
esclusivamente le descrizioni dei campi **nella lingua principale
dell'installazione gestionale**, lingua questa che può essere dichiarata
alla pagina "**Configurazione Gestionale**" del Wizard agendo sul
parametro "**Lingua Installazione**"

![Videate\\leggimi_32.bmp](./assets/media/image189.png){width="5.8180555555555555in"
height="3.5256944444444445in"}

Eventuali descrizioni, per i campi delle tabelle indicate, in lingue
diverse dalla lingua principale dell'installazione gestionale, non
verranno modificate in fase di sincronizzazione e, eventualmente,
dovranno quindi essere aggiornate operando direttamente all'interno del
Wizard in maniera manuale o, laddove possibile, in maniera massiva
mediante export / import di file csv

**ATTENZIONE!** Le tabelle indicate in corrispondenza di questo
parametro variano in relazione al fatto di considerare un sito collegato
a Mexal oppure ad uno dei gestionali Ho.Re.Ca.

[SITI ECOMMERCE COLLEGATI A MEXAL]{.underline}

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\mexal_aggiornamento_descrizioni.bmp](./assets/media/image190.png){width="6.928472222222222in"
height="1.3506944444444444in"}

[SITI ECOMMERCE COLLEGATI AD UNO DEI GESTIONALI HO.RE.CA.]{.underline}

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\horeca_aggiornamento_descrizioni.bmp](./assets/media/image191.png){width="5.727083333333334in"
height="0.7986111111111112in"}

Per maggiori informazioni relativamente a ciascuna delle tabelle
indicate all'interno di questa sezione si vedano i successivi capitoli
di questo manuale

##### TABELLA CATEGORIE MERCEOLOGICHE

Nel momento in cui si dovesse utilizzare l'italiano come "Lingua
dell'installazione", selezionando questo parametro in fase di
sincronizzazione verranno aggiornate, con i valori presenti all'interno
del gestionale, le descrizioni in italiano relative **a tutte le
Categorie Merceologiche**, andando quindi a sovrascrivere eventuali
valori inseriti per questi stessi campi direttamente all'interno del
Wizard di Passweb.

Verrà di conseguenza aggiornato anche **il nome di tutte le pagine di
tipo Catalogo** (corrispondenti a tali categorie merceologiche) oltre
**alle etichette di tutti i menu generati sulla base di tali
categorie**.

Nel caso in cui il parametro non venga selezionato le descrizioni in
italiano presenti all'interno di questa tabella non verranno aggiornate,
mantenendo quindi eventuali personalizzazioni effettuate dall'utente.

**Eventuali descrizioni in lingua diversa dall'italiano non verranno mai
aggiornate alla sincronizzazione e potranno quindi essere personalizzate
o variate unicamente in Passweb, all'interno della corrispondente
sezione.**

##### TABELLA CATEGORIE ABBINATI -- SOLO SITI COLLEGATI A MEXAL

Nel momento in cui si dovesse utilizzare l'italiano come "Lingua
dell'installazione", selezionando questo parametro verranno poi
aggiornate in fase di sincronizzazione, con i valori presenti
all'interno del gestionale, le descrizioni in italiano relative a tutte
le **Categorie di Abbinati** gestite all'interno del sito.

Nel caso in cui il parametro non venga selezionato le descrizioni in
italiano presenti all'interno di questa tabella non verranno aggiornate,
mantenendo quindi eventuali personalizzazioni effettuate dall'utente.

**Eventuali descrizioni in lingua non verranno mai aggiornate alla
sincronizzazione e potranno quindi essere personalizzate o variate
unicamente in Passweb, all'interno della corrispondente sezione.**

##### TABELLA CATEGORIE STATISTICHE CLIENTE -- SOLO SITI COLLEGATI A MEXAL

Nel momento in cui si dovesse utilizzare l'italiano come "Lingua
dell'installazione", selezionando questo parametro verranno poi
aggiornate in fase di sincronizzazione, con i valori presenti
all'interno del gestionale, le descrizioni in italiano relative a tutte
le **Categorie Statistiche** utente gestite all'interno del sito.

Nel caso in cui il parametro non venga selezionato le descrizioni in
italiano presenti all'interno di questa tabella non verranno aggiornate,
mantenendo quindi eventuali personalizzazioni effettuate dall'utente.

**Eventuali descrizioni in lingua non verranno mai aggiornate alla
sincronizzazione e potranno quindi essere personalizzate o variate
unicamente in Passweb, all'interno della corrispondente sezione.**

##### TABELLA NATURA ARTICOLO

Nel momento in cui si dovesse utilizzare l'italiano come "Lingua
dell'installazione", selezionando questo parametro verranno poi
aggiornate in fase di sincronizzazione, con i valori presenti
all'interno del gestionale, le descrizioni in italiano relative a tutte
le **Nature** gestite all'interno del sito.

Nel caso in cui il parametro non venga selezionato le descrizioni in
italiano presenti all'interno di questa tabella non verranno aggiornate,
mantenendo quindi eventuali personalizzazioni effettuate dall'utente.

**Eventuali descrizioni in lingua non verranno mai aggiornate alla
sincronizzazione e potranno quindi essere personalizzate o variate
unicamente in Passweb, all'interno della corrispondente sezione.**

##### TABELLA TAGLIE -- SOLO SITI COLLEGATI A MEXAL 

Nel momento in cui si dovesse utilizzare l'italiano come "Lingua
dell'installazione", selezionando questo parametro verranno poi
aggiornate in fase di sincronizzazione, con i valori presenti
all'interno del gestionale, le descrizioni in italiano relative **agli
elementi di ogni serie di** **Taglie/Colori** gestita all'interno del
sito.

Nel caso in cui il parametro non venga selezionato le descrizioni in
italiano presenti all'interno di questa tabella non verranno aggiornate,
mantenendo quindi eventuali personalizzazioni effettuate dall'utente.

**Eventuali descrizioni in lingua non verranno mai aggiornate alla
sincronizzazione e potranno quindi essere personalizzate o variate
unicamente in Passweb, all'interno della corrispondente sezione.**

##### TABELLA CARTELLA ABBINAMENTI STRUTTURA -- SOLO SITI COLLEGATI A MEXAL

Nel momento in cui si dovesse utilizzare l'italiano come "Lingua
dell'installazione", selezionando questo parametro verranno poi
aggiornate in fase di sincronizzazione, con i valori presenti
all'interno del gestionale, le descrizioni in italiano relative **ai
vari elementi delle Cartelle Abbinamenti** associate a tutte le
strutture gestite all'interno del sito

**NOTA BENE**: tale aggiornamento è relativo ai soli elementi delle
Cartelle Abbinamenti di tipo "Statistico". Le descrizioni degli elementi
di tipo "Variante", in italiano o in lingua, verranno sempre aggiornate
alla sincronizzazione con i rispettivi valori presenti all'interno del
gestionale.

Nel caso in cui il parametro non venga selezionato le descrizioni in
italiano presenti all'interno di questa tabella non verranno aggiornate,
mantenendo quindi eventuali personalizzazioni effettuate dall'utente.

**Eventuali descrizioni in lingua non verranno mai aggiornate alla
sincronizzazione e potranno quindi essere personalizzate o variate
unicamente in Passweb, all'interno della corrispondente sezione.**

##### TABELLA CAUSALI DOCUMENTO -- SOLO SITI COLLEGATI A MEXAL

Nel momento in cui si dovesse utilizzare l'italiano come "Lingua
dell'installazione", selezionando questo parametro verranno poi
aggiornate in fase di sincronizzazione, con i valori presenti
all'interno del gestionale, le descrizioni in italiano relative **a
tutte le causali documento** gestite ed esportate all'interno del sito

Nel caso in cui il parametro non venga selezionato le descrizioni in
italiano presenti all'interno di questa tabella non verranno aggiornate,
mantenendo quindi eventuali personalizzazioni effettuate dall'utente.

**Eventuali descrizioni in lingua non verranno mai aggiornate alla
sincronizzazione e potranno quindi essere personalizzate o variate
unicamente in Passweb, all'interno della corrispondente sezione.**

##### TABELLA INSIEMI VALORI VARIANTE -- SOLO SITI COLLEGATI AD UN GESTIONALE HO.RE.CA.

Nel momento in cui si dovesse utilizzare l'italiano come "Lingua
dell'installazione", selezionando questo parametro verranno poi
aggiornate in fase di sincronizzazione, con i valori presenti
all'interno del gestionale, le descrizioni in italiano relative **ai
vari elementi degli Insiemi di Valori** associati a tutte le Varianti
Articolo gestite all'interno del sito

Nel caso in cui il parametro non venga selezionato le descrizioni in
italiano presenti all'interno di questa tabella non verranno aggiornate,
mantenendo quindi eventuali personalizzazioni effettuate dall'utente.

**Eventuali descrizioni in lingua non verranno mai aggiornate alla
sincronizzazione e potranno quindi essere personalizzate o variate
unicamente in Passweb, all'interno della corrispondente sezione.**

##### TABELLA ASPETTO ESTERIORE BENI -- SOLO SITI COLLEGATI A MEXAL

Nel momento in cui si dovesse utilizzare l'italiano come "Lingua
dell'installazione", selezionando questo parametro verranno poi
aggiornate in fase di sincronizzazione con i valori presenti all'interno
del gestionale, tutte le descrizioni in italiano relative all'aspetto
esteriore dei beni (utilizzate nella gestione dei resi merce).

Nel caso in cui il parametro in oggetto non venga selezionato le
descrizioni in italiano presenti all'interno di questa tabella non
verranno aggiornate, mantenendo quindi eventuali personalizzazioni
effettuate dall'utente.

**Eventuali descrizioni in lingua non verranno mai aggiornate alla
sincronizzazione e potranno quindi essere personalizzate o variate
unicamente in Passweb, all'interno della corrispondente sezione.**

##### TABELLA PAGAMENTI

Nel momento in cui si dovesse utilizzare l'italiano come "Lingua
dell'installazione", selezionando questo parametro verranno poi
aggiornate in fase di sincronizzazione, con i valori presenti
all'interno del gestionale, le descrizioni in italiano relative **alle
diverse tipologie di Pagamento.**

Nel caso in cui il parametro non venga selezionato le descrizioni in
italiano presenti all'interno di questa tabella non verranno aggiornate,
mantenendo quindi eventuali personalizzazioni effettuate dall'utente.

**Eventuali descrizioni in lingua non verranno mai aggiornate alla
sincronizzazione e potranno quindi essere personalizzate o variate
unicamente in Passweb, all'interno della corrispondente sezione.**

##### TABELLA CATEGORIA STATISTICA ARTICOLO

Nel momento in cui si dovesse utilizzare l'italiano come "Lingua
dell'installazione", selezionando questo parametro verranno poi
aggiornate in fase di sincronizzazione, con i valori presenti
all'interno del gestionale, le descrizioni in italiano relative a tutte
le **Categorie Statistiche** gestite all'interno del sito.

Nel caso in cui il parametro non venga selezionato le descrizioni in
italiano presenti all'interno di questa tabella non verranno aggiornate,
mantenendo quindi eventuali personalizzazioni effettuate dall'utente.

**Eventuali descrizioni in lingua non verranno mai aggiornate alla
sincronizzazione e potranno quindi essere personalizzate o variate
unicamente in Passweb, all'interno della corrispondente sezione.**

**TABELLA SERIE TAGLIE -- SOLO SITI COLLEGATI A MEXAL**

Nel momento in cui si dovesse utilizzare l'italiano come "Lingua
dell'installazione", selezionando questo parametro verranno poi
aggiornate in fase di sincronizzazione, con i valori presenti
all'interno del gestionale, le descrizioni in italiano relative **alle
varie serie di Taglie/Colori** gestite all'interno del sito.

Nel caso in cui il parametro non venga selezionato le descrizioni in
italiano presenti all'interno di questa tabella non verranno aggiornate,
mantenendo quindi eventuali personalizzazioni effettuate dall'utente.

**Eventuali descrizioni in lingua non verranno mai aggiornate alla
sincronizzazione e potranno quindi essere personalizzate o variate
unicamente in Passweb, all'interno della corrispondente sezione.**

##### TABELLA CAMPI STRUTTURA -- SOLO SITI COLLEGATI A MEXAL

Nel momento in cui si dovesse utilizzare l'italiano come "Lingua
dell'installazione", selezionando questo parametro verranno poi
aggiornate in fase di sincronizzazione, con i valori presenti
all'interno del gestionale, le descrizioni in italiano relative **ai
campi di tutte le strutture gestite sul sito**

Nel caso in cui il parametro non venga selezionato le descrizioni in
italiano presenti all'interno di questa tabella non verranno aggiornate,
mantenendo quindi eventuali personalizzazioni effettuate dall'utente.

**Eventuali descrizioni in lingua non verranno mai aggiornate alla
sincronizzazione e potranno quindi essere personalizzate o variate
unicamente in Passweb all'interno della corrispondente sezione.**

##### TABELLA STRUTTURA VARIANTE -- SOLO SITI COLLEGATI AD UN GESTIONALE HORECA

Nel momento in cui si dovesse utilizzare l'italiano come "Lingua
dell'installazione", selezionando questo parametro verranno poi
aggiornate in fase di sincronizzazione, con i valori presenti
all'interno del gestionale, le descrizioni in italiano relative **ai
campi delle Varianti Articolo gestite sul sito**

Nel caso in cui il parametro non venga selezionato le descrizioni in
italiano presenti all'interno di questa tabella non verranno aggiornate,
mantenendo quindi eventuali personalizzazioni effettuate dall'utente.

**Eventuali descrizioni in lingua non verranno mai aggiornate alla
sincronizzazione e potranno quindi essere personalizzate o variate
unicamente in Passweb all'interno della corrispondente sezione.**

##### TABELLA LINEE ARTICOLO -- SOLO SITI COLLEGATI A MEXAL

Nel momento in cui si dovesse utilizzare l'italiano come "Lingua
dell'installazione", selezionando questo parametro verranno poi
aggiornate in fase di sincronizzazione, con i valori presenti
all'interno del gestionale, le descrizioni in italiano relative a tutte
le **Linee Articolo** gestite all'interno del sito.

Nel caso in cui il parametro non venga selezionato le descrizioni in
italiano presenti all'interno di questa tabella non verranno aggiornate,
mantenendo quindi eventuali personalizzazioni effettuate dall'utente.

**Eventuali descrizioni in lingua non verranno mai aggiornate alla
sincronizzazione e potranno quindi essere personalizzate o variate
unicamente in Passweb, all'interno della corrispondente sezione.**

##### DESCRIZIONE DETTAGLIATA ARTICOLO -- SOLO SITI COLLEGATI A MEXAL 

Nel momento in cui si dovesse utilizzare l'italiano come "Lingua
dell'installazione", selezionando questo parametro verrà poi aggiornata
in fase di sincronizzazione, con il valore prelevato dal corrispondente
campo Mexal, la "**Descrizione Dettagliata**" (in Italiano) degli
articoli coinvolti nella sincronizzazione stessa.

Nel momento in cui il parametro in oggetto non dovesse essere
selezionato, per il campo "Descrizione Dettagliata" verrà invece
mantenuto il valore presente in Passweb indipendentemente da quanto
indicato all'interno di Mexal.

**I valori in lingua del campo "Descrizione Dettagliata" non verranno
mai aggiornati alla sincronizzazione e potranno quindi essere
personalizzati o variati unicamente in Passweb, all'interno della
corrispondente sezione del Wizard.**

Per maggiori informazioni in merito a come gestire il campo "Descrizione
Dettagliata" si veda anche quanto indicato all'interno della sezione
"*Catalogo -- Gestione Articoli -- Articoli -- Anagrafica Articolo /
Servizio -- Anagrafica Passweb -- Descrizioni*" di questo manuale.

##### AGGIORNAMENTO FILE DA GESTIONALE (VARAITI)

La sezione "**Aggiornamento File dal Gestionale (Variati)**"
**disponibile solo nel caso di siti Ecommerce collegati ad uno dei
gestionali Ho.Re.Ca.**, consente di decidere come dovrà comportarsi
l'applicazione in merito alle Risorse Articolo (Immagini e Schede
Tecniche) e alle Immagini delle Categorie Merceologiche inserite
all'interno del gestionale, nel momento in cui dovesse essere eseguita
una **Sincronizzazione automatica** (e indipendentemente dal fatto che
tale sincronizzazione automatica sia stata impostata come sincro totale
o solo per variati).

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\horeca_aggiornamento_file_gestionale.bmp](./assets/media/image185.png){width="3.779166666666667in"
height="0.34444444444444444in"}

Nello specifico i due parametri presenti all'interno di questa sezione
consentiranno rispettivamente di:

- **Tabella Articoli:** se selezionato, a seguito di ogni
  sincronizzazione automatica, per ogni singolo articolo che dovesse
  risultare effettivamente variato rispetto l'ultima sincronizzazione
  utile, verranno prelevate dal corrispondente gestionale Ho.Re.Ca. le
  risorse ad esso associate in corrispondenza dei campi **"Foto"** e
  **"Allegato"** della relativa anagrafica.

> **ATTENZIONE! In queste condizioni le risorse prelevate direttamente
> dal gestionale andranno a sovrascrivere le eventuali risorse caricate
> manualmente direttamente all'interno del Wizard del sito.**
>
> Ovviamente, nel momento in cui si dovesse decidere di importare ad
> ogni sincronizzazione anche le risorse grafiche dei relativi articoli,
> la procedura potrebbe impiegare più tempo.
>
> Volendo, quindi, è possibile decidere di non selezionare questo
> parametro, velocizzando la procedura di sincronizzazione e importando
> poi le sole risorse grafiche, quando necessario, mediante le relativa
> procedura di "Importazione Risorse".
>
> Per maggiori informazioni in merito si veda anche la sezione
> "*Sincronizzazione -- Importazione Risorse Articolo*" di questo
> manuale

- **Tabella Categorie Merceologiche:** se selezionato, a seguito di ogni
  Sincronizzazione automatica verranno prelevate dal gestionale
  Ho.Re.Ca. le immagini relative alle categorie merceologiche che
  risulteranno essere effettivamente variate rispetto l'ultima
  sincronizzazione utile

> Tali risorse andranno quindi, eventualmente a sovrascrivere quelle
> caricate manualmente direttamente all'interno del Wizard del sito

