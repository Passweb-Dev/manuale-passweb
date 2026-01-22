# AGGIORNAMENTO ATTRIBUTI MEXAL



La procedura di **Aggiornamento Attributi,** disponibile solo per siti
Ecommerce collegati a Mexal, è quella particolare operazione che
permette a Passweb di avere la stessa struttura dati utilizzata anche
dal gestionale e di mantenere quindi perfettamente allineate le due base
dati. Tale operazione si può verificare in due diversi momenti:

- Alla prima sincronizzazione sito -- gestionale.

- Ogni qualvolta viene lanciata manualmente cliccando sul pulsante
  **"Aggiorna"** presente all'interno della sezione **"Aggiornamento
  Attributi Mexal"** della maschera "**Parametri Sincronizzazione**" di
  Passweb

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\aggiornamento_attributi.bmp](./assets/media/image175.png)

**ATTENZIONE!** E' grazie a questa operazione che verranno resi
disponibili all'interno di Passweb i campi di eventuali videate
aggiuntive articoli e/o clienti/fornitori

Sulla base di quanto appena detto dunque è abbastanza semplice
comprendere come **ogniqualvolta venga fatta una qualche modifica alla
base dati di Mexal (es. creazione di una nuova videata aggiuntiva,
aggiunta di un nuovo campo ad una videata aggiuntiva già utilizzata ecc.
...) sia poi necessario avviare questa procedura in maniera tale da
mantenere le due basi dati sempre allineate e da poter dunque disporre
in Passweb degli stessi campi disponibili anche all'interno di Mexal.**

**NOTA BENE**: l'operazione di **"Aggiornamento Attributi Mexal"**
consente di poter disporre in Passweb degli stessi campi disponibili
all'interno di Mexal. Starà poi all'utente in fase di realizzazione del
sito web decidere quali di questi campi utilizzare effettivamente.

**In ogni caso l'operazione di "Aggiornamento Attributi Mexal" opera
unicamente a livello di struttura dati preoccupandosi di mettere a
disposizione in Passweb certi campi Mexal ma non di prelevarne il
relativo valore (per questo sarà infatti necessario ricorrere alla
sincronizzazione)**

Supponendo dunque di aver creato in Mexal una nuova videata aggiuntiva
articoli con all'interno dei campi da utilizzare sul sito gli step da
seguire per poter rendere disponibili questi stessi campi, e per ogni
articolo i relativi valori, anche nel corrispondente sito ecommerce
saranno esattamente i seguenti:

1.  Creazione in Mexal dei nuovi campi della videata aggiuntiva articoli

2.  Valorizzazione in Mexal articolo per articolo dei campi della nuova
    videata aggiuntiva

3.  Esecuzione da Passweb della procedura di "**Aggiornamento
    Attributi**" (necessaria per allineare le due basi dati e rendere
    disponibili anche all'interno del sito i nuovi campi)

4.  Creazione, in Passweb, di nuovi Attributi Articolo di tipo Mexal
    mappati con i nuovi campi creati all'interno del gestionale e ora
    disponibili anche in Passweb.

5.  Inserimento dei nuovi campi nelle pagine del sito mediante il
    componente "Dati Articolo"

6.  Esecuzione della procedura di "Sincronizzazione" (necessaria per
    consentire a Passweb di leggere e conseguentemente visualizzare sul
    sito, per ogni articolo, i valori dei nuovi campi creati ai punti
    precedenti).

**NOTA BENE**: la procedura di **"Aggiornamento Attributi Mexal"** può
essere lanciata unicamente da Passweb e non influisce in alcun modo sui
parametri contrattuali relativi alle sincronizzazioni

Una volta lanciata la procedura di Aggiornamento Attribuiti l'esito
verrà notificato via mail all'indirizzo indicato in corrispondenza del
campo **E-mail** presente all'interno della sezione "**Parametri
aggiornamento attributi**" (pagina "Parametri di sincronizzazione" del
Wizard)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\parametri_aggiornamento_attributi.bmp](./assets/media/image176.png)

**ATTENZIONE!** nel caso in cui il campo E-mail evidenziato in figura
non dovesse essere valorizzato, la mail di notifica verrà inviata
all'indirizzo indicato in corrispondenza del campo E-mail presente alla
pagina "**Account e-mail SMS**" del Wizard (menu "*Posta / SMS --
Impostazioni -- Configurazione*")

