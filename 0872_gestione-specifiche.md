# GESTIONE SPECIFICHE



La sezione "**Gestione Specifiche**" consente di codificare delle
Specifiche Custom (personalizzate) che potranno poi essere gestite nelle
Inserzioni utilizzate per la pubblicazione dei prodotti sulle
piattaforme Prestashop e Magento e/o sui Marketplace di Google e
Facebook

Tali specifiche consentono di inserire nel tracciato record dei file
csv, piuttosto che nelle chiamate API prodotte da Passweb in fase di
pubblicazione articoli, campi personalizzati la cui struttura potrà
essere impostata in fase di codifica della specifica stessa e il cui
valore, volendo, potrà poi essere mappato e/o prelevato direttamente da
specifici Campi / Attributi Articolo.

Effettuando l'accesso a questa sezione del Wizard verrà visualizzata la
maschera "**Lista delle specifiche**" contenente l'elenco di tutte le
Specifiche Custom attualmente codificate.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\specifiche_custom_1.bmp](./assets/media/image321.png){width="5.350694444444445in"
height="3.623611111111111in"}

Per ciascuna delle specifiche presenti in elenco verrà indicato:

- Il nome assegnato alla specifica (colonna "**Descrizione**")

- Il metodo di pubblicazione in relazione al quale poter utilizzare la
  corrispondente Specifica (colonna "**Pubblicazione**")

- Il Marketplace sui cui poter utilizzare la corrispondente Specifica
  (colonna "**Marketplace**")

I pulsanti presenti nella relativa barra degli strumenti consentono
rispettivamente di:

- **Elimina Specifica** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_elimina_specifica_custom.bmp](./assets/media/image322.png){width="0.6166666666666667in"
  height="0.18194444444444444in"} ): consente di eliminare la specifica
  custom attualmente selezionata in elenco.

> **ATTENZIONE!** Eliminando una specifica custom la stessa verrà
> ovviamente eliminata in maniera automatica anche da tutte le
> Inserzioni in cui era stata eventualmente gestita

- **Modifica Specifica** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_modifica_specifica_custom.bmp](./assets/media/image323.png){width="0.6430555555555556in"
  height="0.18194444444444444in"} ): consente di modificare la specifica
  attualmente selezionata in elenco.

> **ATTENZIONE!** Nel caso di pubblicazione via CSV, la modifica di
> specifiche già in uso in determinate inserzioni potrebbe compromettere
> l'integrità dei dati presenti nei file prodotti a seguito della
> pubblicazione di articoli coinvolti in queste stesse inserzioni
> (questo soprattutto nel momento in cui la modalità adottata per la
> scrittura di questi file dovesse essere "In append").
>
> **Prima di modificare Tipologia e/o Tag di una Specifica si consiglia
> quindi di verificare che la stessa non sia già in uso in qualche
> Inserzione e, soprattutto, si consiglia di svuotare il repository
> utilizzato per la pubblicazione dei file csv.**

- **Aggiungi Specifica** (
  ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_aggiungi_specifica_custom.bmp](./assets/media/image324.png){width="0.6625in"
  height="0.175in"} ): consente di codificare una nuova Specifica
  Custom.

**ATTENZIONE!** la tipologia e la gestione delle Specifiche definite
all'interno di questa sezione potrà variare a seconda del Marketplace e
del metodo di pubblicazione in relazione al quale la specifica stessa
dovrà poi essere utilizzata.

In particolare:

- Per Prestashop/Magento sarà possibile creare specifiche custom che
  potranno poi essere utilizzate solo in pubblicazioni via CSV

- Per Google Merchant e Facebook Business Manager sarà possibile creare
  specifiche custom che potranno poi essere utilizzate sia in
  pubblicazioni via CSV che in pubblicazioni via API

Nei successivi capitoli di questo manuale vedremo quindi più nel
dettaglio come poter creare e gestire Specifiche Custom che dovranno poi
essere utilizzate su Prestashop / Magento piuttosto che su Google
Merchant o Facebook Business Manager

