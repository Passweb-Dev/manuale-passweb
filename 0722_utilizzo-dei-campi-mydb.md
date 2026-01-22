# UTILIZZO DEI CAMPI MYDB



Una volta creati i campi MyDB secondo quanto descritto nei precedenti
capitoli di questo manuale, per poterli poi utilizzare all'interno del
sito sarà sufficiente creare appositi Attributi Articolo / Cliente /
Ordine **di tipo Mexal** mappati proprio su questi stessi campi

In fase di creazione di un nuovo Attributo Articolo / Cliente / Ordine
infatti, impostando il parametro "**Sorgente Dati**" sul valore
"**Mexal**" troveremo poi, tra i valori selezionabili in corrispondenza
del parametro "**Campo Mexal**", anche i campo MyDB precedentemente
creati.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\utilizzo_campi_mydb.bmp](./assets/media/image258.png)

Supponendo quindi di voler pubblicare l'informazione presente in un
campo MyDB utilizzato per estendere l'anagrafica articoli, sarà
sufficiente creare un nuovo Attributo Articolo di tipo Mexal
selezionando in corrispondenza del parametro "**Campo Mexal**", tra
tutti i valori disponibili, quello corrispondente al campo MyDB
desiderato.

L'Attributo in esame potrà poi essere utilizzato all'interno del sito
come un qualsiasi altro Attributo Articolo.

Per maggiori informazioni relativamente alla creazione e alla gestione
degli Attributi Articolo si veda anche quanto indicato all'interno del
capitolo "*Catalogo -- Attributi Articolo*" di questo manuale.

Per quel che riguarda invece la creazione e la gestione di Attributi
Utente e di Attributi Ordine si veda quanto indicato rispettivamente
all'interno dei capitoli "*Utenti -- Siti Ecommerce -- Utenti Sito --
Utenti -- Gestione Utenti - Attributi*" e "*Ordini -- Ordini -- Gestione
Attributi*" di questo manuale.

Per quel che riguarda poi la valorizzazione di questi Attributi mappati
con campi MyDB occorre sottolineare che:

- In fase di **sincronizzazione da Mexal verso Passweb** verranno letti
  e riportati sul sito i valori dei campi MyDB legati agli Attributi
  Articolo e Cliente attualmente gestiti.

> Inoltre, nel momento in cui il campo MyDB legato ad un determinato
> attributo dovesse essere **Riportabile,** verrà letto e riportato sul
> sito il corrispondente valore anche per tutti i documenti che, alla
> sincronizzazione, risultino essere variati

- In fase di **sincronizzazione da Passweb verso Mexal** occorre invece
  ricordare che:

  - potranno essere modificati i valori dei campi MyDB relativi ad
    anagrafiche Clienti / Fornitori e collegati, ovviamente, ad
    Attributi Cliente effettivamente utilizzati all'interno del sito

  - nel caso in cui alla pagina "**Ordini -- Configurazione Ordini**"
    del Wizard siano stati impostati a **SI** i campi "**Valorizza
    sempre le Videate Riportabili di Testat**a" e "**Valorizza sempre le
    Videate Riportabili di Riga**" allora, in fase di inserimento di un
    nuovo ordine verranno memorizzati, rispettivamente in Testata e in
    Riga di quello stesso documento, i campi MyDB corrispondenti agli
    Attributi Cliente e Articolo legati all'utente intestatario e agli
    articoli coinvolti nell'ordine.

  - in fase di modifica ordine o in caso di reso verranno modificati i
    valori degli Attributi Ordine di Testata e di Riga relativi ai campi
    MyDB gestiti sul sito.

