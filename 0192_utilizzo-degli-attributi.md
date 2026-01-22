# UTILIZZO DEGLI ATTRIBUTI



Una volta creato l'insieme di Attributi che andranno poi a comporre i
vari Temi ed assegnato loro un valore di Default il passo successivo
sarà quello di utilizzare questi stessi Attributi all'interno del sito
in maniera tale da rendere determinati elementi (colori e/o immagini)
variabili in relazione allo specifico Tema che verrà poi applicato.

In questo senso, ad esempio, **in corrispondenza di ogni singolo campo
dello Style Editor utilizzabile per gestire dei colori verrà
visualizzato oltre al pulsante utilizzabile per richiamare la tavolozza
grafica all'interno della quale poter selezionare visivamente lo
specifico colore desiderato, anche una combo box contenente l'elenco di
tutti gli Attributi precedentemente creati**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\temi_9_res.bmp](./assets/media/image334.png){width="4.435416666666667in"
height="2.3680555555555554in"}

Nel momento in cui si dovesse dunque decidere di utilizzare anziché uno
specifico codice colore uno degli Attributi presenti in elenco, la
corrispondente proprietà CSS verrà valorizzata con il relativo
segnaposto, segnaposto questo che in fase di visualizzazione della
pagina verrà poi sostituito con il codice colore assegnato all'Attributo
in questione nel Tema correntemente applicato al sito.

**ATTENZIONE!** In queste condizioni per non compromettere la corretta
visualizzazione del sito sarà necessario utilizzare Attributi il cui
valore è stato effettivamente impostato su di un codice colore
(esadecimale o rgb) valido.

**NOTA BENE:** nel caso in cui la combo box per la selezione degli
Attributi fosse impostata sul valore "Personalizzato" non verrà
utilizzato alcun Attributo e sarà quindi necessario indicare lo
specifico codice colore (che non varierà quindi al variare del Tema)
mediante la relativa tavolozza grafica.

**Allo stesso modo è possibile utilizzare gli Attributi di un Tema per
gestire anche le Immagini di sfondo dei vari elementi.**

Sempre nello Style Editor infatti, all'interno della sezione "Sfondi" è
presente il pulsante "**Aggiungi da Tema**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\temi_10_res.bmp](./assets/media/image335.png){width="4.435416666666667in"
height="2.2819444444444446in"}

mediante il quale poter accedere all'elenco di Attributi attualmente
gestiti.

Selezionando quindi un Attributo di tipo Immagine, come sfondo
dell'elemento in oggetto verrà utilizzata l'immagine associata
all'Attributo stesso nel Tema correntemente applicato al sito.

Oltre ai colori e alle Immagini di sfondo gestibili da Style Editor, gli
Attributi potranno essere utilizzati (sempre secondo la stessa logica)
anche:

- nei **Componenti di tipo Immagine**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\temi_11_res.bmp](./assets/media/image336.png){width="5.086111111111111in"
height="3.061111111111111in"}

> In questo caso al di sotto del pulsante "Seleziona la Risorsa"
> utilizzabile per individuare la specifica immagine da inserire
> all'interno della pagina web, è presente il campo **"Attributi Temi"**
> mediante il quale poter decidere di utilizzare uno degli Attributi
> (ovviamente di tipo Immagine) precedentemente creati in maniera tale
> da rendere il componente stesso variabile in relazione allo specifico
> Tema che verrà poi applicato al sito

- in quelle tipologie di componenti che prevedono parametri di
  configurazione con la possibilità di impostare delle immagini

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\temi_12_res.bmp](./assets/media/image337.png){width="5.086111111111111in"
height="3.079861111111111in"}

> Un esempio in tal senso è rappresentato dal componente "Rating Review"
> che ha come parametri di configurazione le immagini che dovranno da
> utilizzare per rappresentare le stelline che l'utente dovrà poi
> selezionare per esprimere un voto.

- nella sezione **CSS dei layout**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\temi_14_res.bmp](./assets/media/image338.png){width="5.092361111111111in"
height="2.4479166666666665in"}

> Come per il componente HTML anche in questo caso sarà sufficiente
> posizionare il cursore nella posizione in cui si desidera inserire
> l'Attributo, cliccare sul pulsante "Aggiungi Attributo Tema" presente
> immediatamente al di sotto dell'editor di codice e selezionare
> l'Attributo desiderato dal relativo elenco

