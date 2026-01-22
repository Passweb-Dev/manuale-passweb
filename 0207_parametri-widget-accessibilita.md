# PARAMETRI WIDGET ACCESSIBILITA'



All'interno della sezione "**Parametri Widget Accessibilità**" è
possibile decidere di abilitare o meno il Widget di Passweb utile a
migliorare l'accessibilità del proprio sito.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gestione_varianti_parametri_widget_accessibilita.bmp](./assets/media/image30.png)

**ATTENZIONE! per visualizzare la sezione evidenziata in figura e poter
quindi gestire il Widget di Accessibilità è necessario aver abilitato,
per prima cosa, il corrispondente modulo all'interno di Passstore.**

Nello specifico il parametro:

**Abilita Widget di Accessibilità:** consente, se abilitato, di attivare
il Widget di Accessibilità sul front end del proprio sito

**Visualizzazione Pulsante Widget:** consente di indicare,
selezionandola dal relativo menu a tendina, la posizione in cui dovrà
essere visualizzato il pulsante per aprire / chiudere il Widget di
Accessibilità

**Tema Widget Accessibilità:** consente di impostare, selezionandolo dal
relativo menu a tendina, il tema (colori) da utilizzare per il proprio
Widget. E' possibile selezionare una delle seguenti opzioni:

- Blu

- Grigio

- Rosso

- Verde

- Viola

- Valore Personalizzato

Nel momento in cui il parametro in questione dovesse essere impostato
sull'opzione "**Valore Personalizzato**" verrà visualizzato anche un
ulteriore campo di input all'interno del quale poter indicare il nome
della classe CSS che dovrà poi essere utilizzata per customizzare il
Widget secondo le proprie specifiche esigenze

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gestione_varianti_parametri_widget_accessibilita_2.bmp](./assets/media/image31.png)

In questo senso la customizzazione del tema dovrà avvenire impostando in
maniera manuale le varie regole CSS operando, in questo senso ad
esempio, dal Layout di Sito (sezione CSS), e richiede ovviamente
specifiche conoscenze tecniche.

Nello specifico, una volta impostato il nome della classe custom sarà
poi possibile utilizzare questa stessa classe per andare a valorizzare,
secondo le specifiche esigenze del caso, le seguenti variabili CSS in
uso al tema del Widget:

- **\--pwbaccessibility-panel-bkcolor**: colore di background del
  pannello

- **\--pwbaccessibility-panel-textcolor**: colore del testo del pannello

- **\--pwbaccessibility-section-bkcolor**: colore di backgroud delle
  sezioni del pannello

- **\--pwbaccessibility-section-textcolor**: colore del testo delle
  sezioni del pannello

- **\--pwbaccessibility-btn-bkcolor**: colore di background dei bottoni

- **\--pwbaccessibility-btn-bkcolor-active**: colore di background dei
  bottoni selezionati

- **\--pwbaccessibility-btn-bkcolor-hover**: colore di background dei
  bottoni all\'hover

- **\--pwbaccessibility-btn-bordercolor**: colore del bordo dei bottoni

- **\--pwbaccessibility-btngroup-bkcolor-active**: colore di background
  dei bottoni raggruppati all\'hover (Dimensione del Fon, Altezza della
  linea, Spaziatura carattere)

Supponendo dunque di aver indicato come nome della classe personalizzata
il valore "custom-theme" e di voler impostare il colore di background
del pannello sul valore esadecimale " #4B3621" e il colore del testo sul
valore esadecimale " #4B3621" sarà necessario utilizzare la seguente
regola CSS

*#pwbaccessibility-widget.**custom-theme**{*

*\--pwbaccessibility-panel-bkcolor:#4B3621;*

*\--pwbaccessibility-btn-bkcolor:#214B4B;*

*}*

Per maggiori informazioni relativamente all'uso del Widget si veda anche
quanto indicato nel successivo capitolo di questo manuale

**ATTENZIONE!** **si ricorda che, di per sé, il solo Widget di
accessibilità non è sufficiente a mette il sito a norma, dal punto di
vista legale, rispetto a quanto richiesto, a partire da Giugno 2025,
dalla corrispondente normativa europea (EU Accessibility Act -
<https://eur-lex.europa.eu/legal-content/IT/TXT/?uri=CELEX%3A32019L0882>
--).**

**Si ricorda inoltre che la messa a norma del sito rispetto all'EU
Accessibility Act è un onere che rimane in capo al proprietario del sito
e che Passepartout non ha, in questo senso, alcun tipo di
responsabilità.**

In tal senso per portare il sito a norma, evitando quindi possibili
sanzioni, è necessario avviare un processo di audit del proprio sito
volto a verificare il rispetto di tutto quanto richiesto dal EU
Accessibility Act, la messa a norma di eventuali non conformità e la
successiva redazione di una dichiarazione di accessibilità da pubblicare
poi all'interno del sito stesso.

**ATTENZIONE!** Per maggiori informazioni relativamente a questo tipo di
processo è possibile chiedere maggiori informazioni rivolgendosi
direttamente all'assistenza Passepartout

