# GESTIONE VALUTE



La pagina **"Gestione Valute"** **accessibile solo nel caso di siti
Ecommerce collegati a Mexal**, consente di specificare l'elenco delle
valute gestite all'interno del sito ed in cui potranno dunque essere
visualizzati i prezzi dei vari articoli.

All'interno di questa pagina verrà quindi visualizzata la maschera,
**"Gestione delle Valute"**, qui di seguito riportata

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gestione_valute.bmp](./assets/media/image164.png){width="5.629861111111111in"
height="3.467361111111111in"}

in cui poter definire l'elenco delle valute gestite.

Nella maschera sopra evidenziata la List Box sulla sinistra contiene
l'elenco di tutte le valute che è possibile gestire all'interno del
proprio sito web; la List Box sulla destra contiene invece l'elenco
delle valute effettivamente gestite.

**NOTA BENE:** l'elenco di tutte le valute che è possibile attivare e
gestire all'interno del proprio sito web (List Box sinistra) viene
prelevato direttamente dalla "Tabella Valute" di Mexal**.**

**NOTA BENE:** i coefficienti di conversione tra le varie valute sono
prelevati direttamente dalla "Tabella Cambi Valute" di Mexal

Per poter dunque inserire una specifica valuta nell'elenco delle valute
gestite è sufficiente selezionarla dall'elenco di sinistra, inserirla
nel riquadro di destra cliccando sulla piccola freccia rivolta verso
destra e cliccare infine sul pulsante "Salva" presente nella parte bassa
della maschera.

Allo stesso modo, per eliminare dall'elenco delle valute gestite una
specifica valuta, è sufficiente selezionarla dall'elenco di destra
reinserirla nel riquadro di sinistra cliccando sulla piccola freccia
rivolta verso sinistra e ancora una volta cliccare sul pulsante "Salva"
presente nella parte bassa della maschera.

Nel caso in cui la valuta che si intende gestire ed attivare all'interno
del sito non sia presente nell'elenco di tutte le possibili valute (List
Box sinistra), occorrerà per prima cosa codificarla all'interno del
gestionale aggiungendola a quelle presenti nella **"Tabella Valute"** di
Mexal (*"Azienda -- Parametri di Base -- Tabella Valute"*).

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\tabella_valute_Mexal.bmp](./assets/media/image165.png){width="2.7465277777777777in"
height="2.00625in"}

**NOTA BENE:** affinché la valuta venga esportata correttamente su
Passweb è necessario specificare in questa tabella la corretta dicitura
ISO della valuta (si può fare riferimento alla tabella ISO consultabile
all'indirizzo: http://it.wikipedia.org/wiki/ISO_4217)

Successivamente, dopo aver codificato in Mexal la nuova valuta,
occorrerà riportare, anche all'interno del sito web, la variazione
appena effettuata sul gestionale.

Per poter far questo sarà sufficiente lanciare una sincronizzazione
manuale dal menu *"Configurazione --Sincronizzazione"* di Passweb oppure
attendere la prossima sincronizzazione automatica.

Al termine di questa operazione la nuova valuta comparirà nell'elenco di
tutte le possibili valute (List Box sinistra) e potrà quindi essere
selezionata ed inserita nell'elenco delle valute effettivamente gestite
all'interno del sito.

**ATTENZIONE!** Per maggiori informazioni relativamente alle modalità di
determinazione del paese di provenienza dell'utente che naviga il sito,
e alla conseguente applicazione automatica di una determinata valuta, si
veda anche quanto indicato all'interno dei capitoli e "*Sito- Gestione
Lingue del sito*" e *"Configurazione Gestionale -- Parametri Paese
Lingua e Valuta -- Gestione Listini*" di questo manuale.

Nel caso in cui non fosse gestita e disponibile la valuta del paese di
appartenenza dell'utente attualmente collegato al sito verrà utilizzata
la valuta del paese di default. Nel caso in cui anche la valuta del
paese di default non fosse tra le valute gestite verrà allora utilizzata
la valuta indicata nel campo **"Valuta di Riferimento"**

**NOTA BENE:** come valuta di riferimento può essere selezionata
solamente una tra le valute gestite all'interno del sito.

In ogni caso l'utente potrà sempre avere la possibilità di variare la
valuta in cui vengono visualizzati i prezzi degli articoli. E' infatti
possibile inserire all'interno del sito il componente e-commerce
**"Cambio Valuta"** grazie al quale verrà messa a disposizione
dell'utente una combo box per selezionare, tra quelle effettivamente
gestite, la specifica valuta in cui visualizzare i prezzi degli articoli
(vedi anche sezione *"Live Editing -- Lista Componenti E-commerce --
Componente Cambio Valuta"* di questo manuale).

**Considerata la forte integrazione con il gestionale, Passweb assegna
sempre una priorità più elevata alle specifiche impostazioni di Mexal.**

Nel caso in cui dunque l'utente attualmente connesso al sito sia già un
cliente Mexal che ha nelle sue condizioni commerciali una specifica
valuta, e nel caso in cui tale valuta sia tra quelle effettivamente
gestite all'interno del sito, dopo che l'utente ha effettuato il login e
si è quindi fatto riconoscere dall'applicazione gli importi verranno
automaticamente, ed indipendentemente da tutto il resto, convertiti ed
espressi nella valuta corretta.

**NOTA BENE:** se l\'utente è già un cliente Mexal ed ha nelle sue
condizioni commerciali una delle valute gestite sul sito, dopo aver
effettuato il login, ed essersi quindi fatto riconoscere
dall'applicazione, gli importi verranno opportunamente convertiti e
visualizzati nella valuta corretta**.**

Nel caso in cui invece l'utente attualmente connesso al sito, e già
cliente Mexal, abbia nelle sue condizioni commerciali una valuta non
gestita all'interno del sito, per esso verrà utilizzata la valuta del
suo paese di appartenenza oppure la valuta indicata nel campo "Valuta di
Riferimento".

**NOTA BENE:** è fortemente consigliato abilitare e gestire all'interno
del sito tutte le valute effettivamente abilitate e gestite in
Mexal**.**

Per quel che riguarda infine i nuovi utenti (non ancora clienti Mexal)
nel caso in cui dovesse essere effettuato da uno di essi un nuovo ordine
in valuta, alla successiva sincronizzazione in Mexal:

- Verrà inserito il relativo documento (OC / OX) nella stessa valuta
  visualizzata ed utilizzata all\'interno del sito;

- Verrà creata la nuova anagrafica del cliente con, nelle sue condizioni
  commerciali, la stessa valuta visualizzata ed utilizzata all\'interno
  del sito.

