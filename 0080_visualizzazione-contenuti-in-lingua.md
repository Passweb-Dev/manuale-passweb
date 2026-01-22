# VISUALIZZAZIONE CONTENUTI IN LINGUA



**Nel caso di siti in multilingua l'utente che accede al sito potrà
visualizzare i testi delle pagine in una specifica lingua piuttosto che
nella lingua di default, dipendentemente da quella che è lingua
impostata per il suo browser oltre che, ovviamente, da quelle che sono
le lingue attualmente abilitate all'interno del sito.**

Supponendo dunque di aver realizzato il sito in due lingue, italiano ed
inglese, e di aver impostato come lingua di default l'italiano, nel
momento in cui un utente dovesse visitare il sito, gli verranno proposte
automaticamente le pagine in italiano o in inglese dipendentemente dalla
lingua attualmente impostata per il browser utilizzato per visitare il
sito.

Nello specifico se per il browser in questione è stata impostata la
lingua inglese il sito verrà aperto automaticamente in inglese, in tutti
gli altri casi (es. browser con lingua francese) il sito verrà aperto in
italiano

**In questo modo dunque anche se un utente dovesse spostarsi con il
proprio pc in un paese estero, continuerà a visualizzare il sito nella
sua lingua di riferimento.**

**ATTENZIONE!** Questo tipo di controllo viene eseguito solamente al
primo accesso al sito; ciò significa dunque che, l'utente potrebbe
comunque modificare manualmente in un qualsiasi istante (mediante
l'apposito componente Passweb) la lingua di visualizzazione del sito.

Per maggiori informazioni relativamente a come verificare ed
eventualmente modificare la lingua attualmente impostata per il proprio
browser si consiglia di fare riferimento alla manualistica dello
specifico browser.

Nel caso ad esempio di Google Chrome per gestire questo tipo di
impostazioni è necessario accedere per prima cosa al menu delle
impostazioni, selezionare la voce "**Mostra Impostazioni Avanzate**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\impostazioni_lingua_1.bmp](./assets/media/image427.png)

e successivamente cliccare sul pulsante "**Impostazioni della lingua ed
immissione**" presente nella sezione "**Lingue**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\impostazioni_lingua_2.bmp](./assets/media/image428.png)

In questo modo verrà infatti visualizzata la maschera "**Lingue**"
contenente l'elenco delle lingue attualmente gestibili per il proprio
browser

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\impostazioni_lingua_3.bmp](./assets/media/image429.png)

**ATTENZIONE! La lingua attualmente impostata per il proprio browser, e
che potrebbe determinare quindi la visualizzazione del sito Passweb in
una lingua piuttosto che in un\'altra, è la prima in elenco**

Come si può facilmente notare dalla figura sopra evidenziata la lingua
impostata per il proprio browser potrebbe essere generica -- es. Inglese
-- oppure potrebbe essere riferita anche ad uno specifico paese -- es.
Inglese (Stati Uniti) --.

Ora, mentre per la visualizzazione dei testi del sito il fatto di
utilizzare una lingua generica piuttosto che una lingua riferita ad uno
specifico paese non ha molta importanza, nel senso che il sito, posto di
aver ovviamente gestito la lingua inglese, verrà aperto in tale lingua
sia che il browser utilizzato per visitarlo sia impostato con la lingua
Inglese o con quella Inglese (Stati Uniti), questa stessa impostazione
potrebbe invece avere effetti diversi per quel che riguarda, ad esempio,
la geolocalizzazione delle valute, di eventuali gruppi di utenti
definiti proprio sulla base del paese di provenienza e per quel che
riguarda anche l'elenco dei paesi gestiti.

In questi casi infatti diventa di fondamentale importanza conoscere non
solo la lingua ma anche lo specifico paese di provenienza dell'utente.

In questo senso è quindi bene evidenziare che:

- nel caso in cui la lingua impostata per il browser utilizzato
  dall'utente faccia riferimento anche allo specifico paese -- es.
  Inglese (Stati Uniti) -- Passweb utilizzerà questa informazione per
  determinare la corretta valuta di gestione del sito, l'eventuale
  appartenenza dell'utente stesso ad uno dei gruppi definiti sulla base
  di specifici paesi oltre che per determinare se l'utente proviene o
  meno da uno dei paesi gestiti all'interno del sito.

- nel caso in cui la lingua impostata per il browser utilizzato
  dall'utente sia generica -- es. Inglese -- per determinare la corretta
  valuta di gestione, l'eventuale appartenenza dell'utente stesso ad uno
  dei gruppi definiti sulla base di specifici paesi oltre per
  determinare se l'utente proviene o meno da uno dei paesi gestiti
  all'interno del sito, Passweb utilizzerà l'indirizzo IP associato
  all'utente che sta navigando il sito stesso.

**ATTENZIONE! La corrispondenza Indirizzo IP -- Paese di provenienza è
determinata automaticamente da Passweb sulla base di un servizio
gratuito di tipo "light" la cui precisione potrebbe non essere quindi
garantita al 100% soprattutto in virtù di eventuali riassegnazioni degli
indirizzi IP da parte dei vari provider.**

Nel caso in cui l'esigenza dovesse quindi essere quella di ottenere una
maggiore precisione relativamente alla corrispondenza "Indirizzo IP --
Paese di provenienza" sarà necessario passare ad un servizio a
pagamento.

