# PARAMETRI DI INTEGRAZIONE



Per poter completare l'integrazione tra il proprio sito Ecommerce e la
piattaforma di pagamento Klarna è necessario disporre di appositi dati
da inserire tra i parametri di configurazione del pagamento Passweb.

Per ottenere queste chiavi sarà necessario:

1.  Completare la creazione del proprio account Klarna

2.  Effettuare l'accesso alla piattaforma ( <https://www.klarna.com/it/>
    ) utilizzando l'account appena creato

3.  Portarsi quindi all'interno della sezione "**Impostazioni --
    Credenziali API** " selezionando l'apposita voce di menu posta sulla
    sinistra della pagina

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_klarna_1.bmp](./assets/media/image115.png)

> e cliccare poi sul pulsante "**Genera nuove credenziali API Klarna**"
> evidenziato in figura

4.  Cliccare quindi sul pulsante "**Crea Credenziali**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_klarna_2.bmp](./assets/media/image116.png)

> e copiare i dati presenti all'interno dei campi "**Nome Utente
> (UID)**" e "**Password**" evidenziati

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_klarna_3.bmp](./assets/media/image117.png)

> all'interno rispettivamente dei campi "**Username**" e "**Password**"
> presenti nella sezione "**Parametri del gateway**" della maschera di
> configurazione del pagamento Passweb

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_klarna_4.bmp](./assets/media/image118.png)

> **ATTENZIONE!** Come evidenziato nel corrispondente messaggio del back
> office di Klarna, una volta generata la password questa non sarà più
> accessibile. Si consiglia quindi di salvarla in una posizione sicura e
> accessibile nel momento in cui dovesse essere recuperata

Come evidenziato nel precedente capitolo di questo manuale, infine,
Klarna offre anche la possibilità di inserire tanto in Checkout quando
direttamente nelle singole pagine prodotto un simulatore del pagamento
che consente all'utente di verificare l'importo delle singole rate che
verranno poi generate a fronte di quel determinato acquisto.

Affinchè tale simulatore possa funzionare in maniera corretta è però
necessario configurare correttamente il parametro "**ID Simulatore**"
presente anche esso nella sezione "Parametri del gateway" della maschera
di configurazione del pagamento Passweb.

Per ottenere questo codice identificativo è necessario:

1.  Accedere al back office del proprio account Klarna, portarsi nella
    sezione "**On-site messaging**" cliccando sulla corrispondente voce
    di menu posta sulla sinistra della pagina e cliccare suk pulsante
    "**Continua**" evidenziato in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_klarna_5.bmp](./assets/media/image119.png)

2.  Una volta effettuato l'accesso alla sezione "Installazione" l'ID
    Simulatore sarà esattamente quello indicato in corrispondenza
    dell'attributo "data-client-id" presente nello script di
    installazione visualizzato all'interno del box "Aggiungi il tuo
    codice al sito"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_klarna_6.bmp](./assets/media/image120.png)

> Copiare quindi il valore evidenziato in figura ed inserirlo nel
> corrispondente parametro di configurazione del pagamento Passweb
>
> **ATTENZIONE!** Nel momento in cui il parametro in questione non
> dovesse essere valorizzato in maniera corretta il simulatore potrebbe
> non essere visualizzato né in fase di checkout né tanto meno nelle
> singole pagine prodotto

**NOTA BENE**: quanto indicato in questo manuale relativamente
all'utilizzo dell'applicazione di Back Office del gateway di pagamento
potrebbe non essere allineato con la corrente versione di tale software.
In tal senso si consiglia quindi di fare riferimento sempre alla
relativa manualistica di prodotto.

