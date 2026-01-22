# SPECIFICHE CUSTOM -- GOOGLE / FACEBOOK -- PUBBLICAZIONI VIA CSV



Come evidenziato nei precedenti capitoli di questo manuale le Specifiche
Custom create per Google e Facebook possono tranquillamente essere
utilizzate sia con pubblicazioni via API che con pubblicazioni via CSV.

Ora, se nel caso della pubblicazione via API il discorso è abbastanza
semplice da comprendere, nel senso che i dati da inviare agli endpoint
Google devono essere gestiti in formato JSON e la struttura delle
specifiche custom dovrà essere quindi ricreata esattamente come indicato
nella relativa documentazione, nel caso di pubblicazioni via CSV il
discorso è leggermente diverso.

Le specifiche custom che andremo a creare dovranno infatti essere
inserite all'interno del file csv utilizzando una ben precisa sintassi
sia per l'intestazione della colonna in cui verrà inserita la specifica,
sia per i valori che dovranno poi essere inseriti nelle diverse righe
del file

Come per la pubblicazione via API dunque, anche in questo caso il punto
di partenza dovrà essere sempre la documentazione fornita dalla
piattaforma terza, documentazione questa in cui sarà indicato
esattamente, per ogni singola specifica, come questa dovrà essere
inserita all'interno del file sia a livello di intestazione che a
livello di singoli valori.

Nel caso di Google Merchant, ad esempio, la documentazione a cui fare
riferimento relativamente alla pubblicazione via csv, è quella presente
al seguente indirizzo

<https://developers.google.com/shopping-content/reference/rest/v2.1/products>

e, come si può facilmente notare, **nomi e sintassi richiesti dalle
varie specifiche sono ovviamente diversi da quelli richiesti nel caso di
pubblicazioni via API.**

Lo strumento messo a disposizione da Passweb per creare queste
specifiche è invece sempre lo stesso, ossia il JSON Builder presente
all'interno della sezione "**Struttura Specifica Custom**" esaminato nel
precedente capitolo di questo manuale.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\json_builder_specifiche_custom.bmp](./assets/media/image328.png){width="5.350694444444445in"
height="3.623611111111111in"}

Il punto fondamentale sarà quindi quello di capire esattamente quale
struttura dati dovremo utilizzare all'interno di questo JSON Builder per
fare in modo che la specifica custom che andremo a creare venga poi
inserita all'interno del file csv con la sintassi corretta.

In questo senso, analizzando la documentazione messa a disposizione da
Google possiamo osservare che le varie specifiche sono gestite,
sostanzialmente, in tre modi diversi:

- **come attributi semplici**

- **come valori multipli separati da ,**

- **come attributi con un certo numero di sotto attributi**

In realtà esistono anche altri tipi di sintassi, come ad esempio quella
utilizzata per le categorie merceologiche che però rientrano già tra le
specifiche standard gestite automaticamente da Passweb.

Detto ciò vediamo quali sono le strutture dati che dovremo andare a
creare all'interno del JSON Builder per poter gestire, nel caso di
pubblicazioni via CSV, ciascuna delle tre tipologie di specifiche sopra
indicate.

##### SPECIFICHE GESTITE COME ATTRIBUTI SEMPLICI

E' il caso più semplice.

In queste condizioni infatti il nome della specifica dovrà essere
esattamente quello che viene inserito come intestazione nella colonna
del file csv deputata a gestire la specifica in esame.

I valori della specifica saranno invece valori singoli da inserire nelle
diverse righe del file senza dover utilizzare particolari sintassi

**Esempio**: '*material'*

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\csv_specifica_custom_semplice_1.bmp](./assets/media/image348.png){width="5.467361111111111in"
height="3.8118055555555554in"}

Per poter gestire specifiche custom di questo tipo, nel JSON Builder
dovremo quindi creare **un solo nodo con valore semplice utilizzando
come "nome proprietà" il nome stesso della specifica**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\csv_specifica_custom_semplice_2.bmp](./assets/media/image349.png){width="5.350694444444445in"
height="3.623611111111111in"}

L'unica cosa a cui prestare attenzione, in queste condizioni, sono i
valori ammessi dalla specifica che possono essere, come nel caso in
esame, stringhe di qualsiasi tipo (con l'unica limitazione imposta dal
numero massimo di caratteri utilizzabili) oppure, per determinate
specifiche, devono essere necessariamente dei valori ben precisi.

Nel momento in cui l'esigenza dovesse essere, ad esempio, quella di
inviare a Google informazioni sull'altezza del prodotto, la specifica da
utilizzare dovrebbe essere *product_height*

Osservando la documentazione in merito a questa specifica

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\csv_specifica_custom_semplice_3.bmp](./assets/media/image350.png){width="5.467361111111111in"
height="3.8118055555555554in"}

possiamo notare che essa rientra effettivamente nel caso delle
specifiche gestite come attributi semplici per cui, lato Passweb dovrà
essere creata, come per '*material',* una struttura di un solo nodo di
tipo valore semplice utilizzando come 'nome proprietà' il nome della
specifica (ossia *product_height*).

In questo caso però i valori che tale specifica dovrà assumere non
possono essere stringhe di qualsiasi tipo ma dovranno avere
necessariamente una sintassi ben precisa del tipo

*Number + unit*

dove gli unici valori ammessi per '*unit*' sono '*cm'* o '*in'*

Ciò significa dunque che i valori che andremo ad inserire, per ogni
articolo, nell'Attributo utilizzato per mappare questa specifica non
potranno essere valori "a caso" ma dovranno avere esattamente la
sintassi richiesta.

In conseguenza di ciò se per un determinato articolo dovessimo
utilizzare come valore di questo attributo, ad esempio "*50 m*" o
'*20cm*', in fase di import dati da csv otterremo degli errori e il
prodotto potrebbe anche non essere pubblicato.

##### SPECIFICHE GESTITE CON VALORI MULTIPLI SEPARATI DA ,

**Esempio**: *excluded_destination*

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\csv_specifica_custom_valori_multipli.bmp](./assets/media/image351.png){width="5.467361111111111in"
height="3.8118055555555554in"}

Come nel caso precedente anche questo tipo di specifiche non hanno sotto
attributi per cui, a livello di intestazione, nel file csv andrà
utilizzato esattamente lo stesso nome della specifica, e lato Passweb,
dovremo creare **un solo nodo utilizzando** **come "nome proprietà" il
nome stesso della specifica**

Controllando però le informazioni di dettaglio relative alla specifica
in oggetto (informazioni queste a cui si può accedere cliccando sul nome
della specifica stessa)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\csv_specifica_custom_valori_multipli_2.bmp](./assets/media/image352.png){width="5.467361111111111in"
height="3.8118055555555554in"}

si potrà osservare non solo che la specifica in questione può accettare
solo determinati valori (indicati in "**Supported values**"), ma anche
che è possibile utilizzarne più di uno contemporaneamente a patto di
separarli con una ,

In queste condizioni quindi il tipo di nodo che dovremo andare a creare
su Passweb potrà variare in relazione a come dovremo poi gestire i
valori di questa specifica.

Se dovessimo comunque gestire un solo valore allora potremmo
tranquillamente utilizzare un nodo di tipo semplice.

Se invece dovessimo gestire situazioni in cui per determinati articoli
questa specifica potrebbe anche avere più di un valore allora la
struttura dati da creare in Passweb dovrà essere sì quella di un solo
nodo **ma di tipo "Array di Stringhe"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\csv_specifica_custom_valori_multipli_3.bmp](./assets/media/image353.png){width="5.350694444444445in"
height="3.623611111111111in"}

##### SPECIFICA GESTITE COME ATTRIBUTI CON SOTTO ATTRIBUTI 

**Esempio**: '*certification'*

Come indicato nella relativa documentazione

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\es_specifica_csv_certification_1.bmp](./assets/media/image354.png){width="5.467361111111111in"
height="3.441666666666667in"}

questo tipo di specifiche hanno un certo numero di sotto attributi.
Inoltre analizzando anche le informazioni di dettaglio relative alla
specifica in oggetto

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\csv_specifica_custom_sotto_attributi.bmp](./assets/media/image355.png){width="5.467361111111111in"
height="3.8118055555555554in"}

possiamo osservare che, in queste condizioni a livello di intestazione,
nel file csv deve essere utilizzata una sintassi di questo tipo

*nome_specifica(nome_sottoattributo1:nome_sottoattributo2:nome_sottoattributo3:
...:nome_sottoattributoN)*

che nel caso in esame si traduce in

***certification(certification_authority:certification_name:certification_code)***

Allo stesso modo anche i possibili valori della specifica dovranno
essere inserti con la sintassi

*valore_sottoattributo1:valore_sottoattributo2:valore_sottoattributo3:
... :valore_sottoattributoN*

Per ottenere questo tipo di risultato lato Passweb dovremo creare una
struttura dati costituita da un **Oggetto "semplice" cui assegnare il
nome della specifica con tante proprietà quanti sono i suoi sotto
attributi e assegnando anche a ciascuna proprietà il nome del relativo
sotto attributo**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\csv_specifica_custom_sotto_attributi_2.bmp](./assets/media/image356.png){width="5.350694444444445in"
height="3.623611111111111in"}

