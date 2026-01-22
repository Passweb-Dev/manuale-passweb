# FINDOMESTIC CON INCENTIVI STATALI



Nel caso in cui si sia deciso di attivare il modulo Findomestic che
prevede la possibilità di richiedere anche incentivi statali, per poter
completare in maniera corretta la configurazione del pagamento, oltre a
settare tutti i parametri presenti all'interno della sezione "Parametri
Gateway", sarà necessario anche marcare, mediante la creazione di
appositi Attributi, tutti gli articoli che possono effettivamente
usufruire di tali incentivi utilizzando, in questo senso, i **Codici
PRF** e i **Codici Finalità** forniti direttamente da Findomestic al
momento dell'adesione al servizio.

In sostanza dunque, a seconda della tipologia di prodotti venduti e del
tipo di incentivo di cui questi potranno usufruire, Findomestic
rilascerà all'esercente una serie di codici che dovranno essere inseriti
sui relativi articoli oltre che nella configurazione del pagamento
Passweb.

La presenza di questi codici sugli articoli in carrello e la corretta
configurazione del pagamento, attiveranno la possibilità, in checkout,
di richiedere il finanziamento Findomestic con il giusto incentivo
statale (coerente cioè con la tipologia di articoli in ordine)

In questo senso però è bene fare subito alcune considerazioni di
fondamentale importanza:

- **Passweb è in grado di gestire fino a 5 diverse tipologie di
  incentivi statali**

- **Nel caso in cui si dovessero gestire all'interno del proprio sito
  articoli che possono usufruire di diversi incentivi statali, potrebbe
  essere necessario attivare la gestione delle "Linee Articolo" in modo
  tale che questi prodotti possano poi generare ordini distinti**

> In questo senso infatti Findomestic non accetta ordini contenenti
> articoli sottoposti a due diverse tipologie di incentivo, per cui, pur
> avendo configurato tutto correttamente se dovessimo mettere in ordine
> contemporaneamente un "Articolo A" sottoposto ad "Incentivo 1" e un
> "Articolo B" sottoposto ad "Incentivo 2" l'unica possibilità che
> avremo, in relazione al pagamento Findomestic, sarà quella di
> richiedere un finanziamento standard con rateizzazione dell'importo ma
> comunque senza poter usufruire degli incentivi statali.
>
> Le "Linee Articolo" gestite da Passweb possono evitare questo tipo di
> problema proprio perché, partendo da un carrello con articoli
> appartenenti a due linee diverse, consentono di generare due ordini
> distinti (per i quali andranno compilati due distinti moduli di
> checkout).
>
> Per maggiori informazioni sulle Linee Articolo si veda anche quanto
> indicato nella corrispondente sezione di questo manuale ("*Catalogo --
> Linee Articolo*" e "*Configurazione Gestionale -- Mexal Parametri
> Configurazione Gestionale -- Mexal Attivazione Passweb -- Funzionalità
> Mexal Articoli -- Gestione Linee Articolo*")

Tenendo conto di quanto appena detto, nella sezione "**Parametri
Gateway**" della maschera di configurazione del pagamento Findomestic
sarà necessario impostare un valore per i seguenti parametri:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_findomestic.bmp](./assets/media/image94.png){width="5.779166666666667in"
height="3.4090277777777778in"}

- **Ambiente del Gateway:** permette di definire se utilizzare come
  ambiente del pagamento, l'ambiente di test (da utilizzare solo ed
  esclusivamente in fase di sviluppo del sito) oppure l'ambiente reale
  di produzione.

- **Identificativo Partner / Codice Venditore TVEI / Codice PRF:**
  codici di configurazione rilasciati all'esercente da Findomestic al
  momento dell'adesione al servizio

> **ATTENZIONE!** i parametri **Identificativo Partner / Codice
> Venditore TVEI / Codice PRF** sono esattamente gli stessi che si
> avrebbero anche con il modulo standard di Findomestic. Nello specifico
> il Codice PRF definito in questo campo verrà utilizzato nel momento in
> cui dovessimo avere nello stesso ordine articoli sottoposti a diverse
> tipologie di incentivi statali.
>
> In queste condizioni infatti, come precedentemente evidenziato,
> l'unica possibilità sarà quella di richiedere un finanziamento
> standard con rateizzazione dell'importo ma senza utilizzo di incentivi
> di alcun tipo

All'interno della sezione "**Parametri Incentivi Statali**" sarà invece
necessario impostare tutti i parametri richiesti in relazione alla
tipologia di incentivo (5 disponibili) che si desidera attivare.

Nello specifico:

- **Attributo Articolo Codice PRF**: consente di indicare,
  selezionandolo dal relativo menu a tendina, l'Attributo Articolo
  utilizzato per associare ai singoli prodotti il "**Codice PRF**"
  fornito direttamente da Findomestic

- **Attributo Articolo Codice Finalità:** consente di indicare,
  selezionandolo dal relativo menu a tendina, l'Attributo Articolo
  utilizzato per associare ai singoli prodotti il "**Codice Finalità**"
  fornito direttamente da Findomestic

- **Codice Finalità Articolo:** consente di indicare il "**Codice
  Finalità**" fornito direttamente da Findomestic e che dovrà essere
  applicato nel momento in cui dovessimo avere in ordine più articoli
  sottoposti allo stesso tipo di incentivo statale ma con singoli
  "Codici Finalità" differenti.

- **Testo Domanda Incentivi:** consente di specificare, in tutte le
  lingue attualmente gestite all'interno del sito, il testo della
  domanda che verrà visualizzata all'utente in relazione alla selezione
  del pagamento Findomestic che prevede anche l'utilizzo degli incentivi
  statali

- **Testo No Incentivi:** consente di specificare, in tutte le lingue
  attualmente gestite all'interno del sito, la label corrispondente alla
  scelta di effettuare la richiesta di finanziamento senza incentivi

- **Testo Incentivo Statale 1 / 2 / 3 / 4 / 5:** consente di
  specificare, in tutte le lingue attualmente gestite all'interno del
  sito, la label corrispondente all'incentivo che l'utente desidera
  attivare nella richiesta di finanziamento

- **Codice PRF -- Incentivo Statale** **1 / 2 / 3 / 4 / 5:** consente di
  impostare per ciascuna delle 5 tipologie di incentivi gestibili
  all'interno del proprio sito Passweb, il "**Codice PRF**" fornito
  direttamente da Findomestic e identificativo della specifica tipologia
  di incentivo statale

Per comprendere meglio come poter configurare tutto il sistema al fine
di inviare a Findomestic una richiesta di finanziamento con incentivi
statali consideriamo ora un semplice esempio

**[ESEMPIO]{.underline}**

Supponiamo di vendere all'interno del nostro sito due diverse tipologie
di articoli, mobili e articoli di climatizzazione, sottoposti a due
diverse tipologie di incentivi (ad esempio per la ristrutturazione
edilizia, e per l'efficienza energetica)

In queste condizioni dopo aver sottoscritto il contratto, Findomestic
invierà all'esercente, tra gli altri, una serie di codici necessari per
configurare la propria piattaforma del tipo di quelli qui di seguito
riportati:

**Codice PRF Incentivo ristrutturazione** = 50190 -- E' il codice
identificativo della specifica tipologia di incentivo statale. Andrà
quindi inserito, ad esempio, all'interno del campo Passweb "**Codice PRF
-- Incentivo Statale 1**"

**Codice PRF Incentivo energetico** = 20222 -- E' il codice
identificativo della specifica tipologia di incentivo statale. Andrà
quindi inserito, ad esempio, all'interno del campo Passweb "**Codice PRF
-- Incentivo Statale 2**"

**Codice Finalità generica**: 123 -- E' il Codice Finalità generico che
dovrà essere passato a Findomestic nel momento in cui dovessimo avere in
ordine più articoli con singoli codici finalità diversi ma che rientrano
tutti nell'ambito dei mobili e che possono quindi essere sottoposti allo
stesso incentivo di ristrutturazione (quello con Codice PRF 50190).
Andrà quindi inserito all'interno del campo Passweb "**Codice Finalità
Articolo**"

**Codice PRF Articolo** = 50190 -- Questo codice andrà inserito come
valore dell'attributo indicato all'interno del campo Passweb
"**Attributo Articolo Codice PRF**". Ogni articolo gestito all'interno
del sito che potrà essere sottoposto all'incentivo di ristrutturazione
dovrà quindi avere, per l'attributo indicato, questo esatto valore

**Codici Finalità Articolo (mobili):** Questo codice andrà inserito, per
tutti gli articoli della categoria mobili, come valore dell'attributo
indicato all'interno del campo Passweb "**Attributo Articolo Codice
Finalità**". All'interno della categoria "mobili" potremo quindi avere
diverse tipologie di articoli che possono essere tutte sottoposte
all'incentivo di ristrutturazione. A seconda della specifica tipologia
ogni articolo dovrà quindi avere per l'attributo indicato il suo
specifico "Codice finalità". Un possibile schema potrebbe essere il
seguente

- Codice finalità per Salotto: 123

- Codice Finalità per Sala da pranzo:456

- Codice Finalità per Letti / Materassi: 789

- ...

**Codici Finalità Articolo (articoli di climatizzazione):** Questo
codice andrà inserito, per tutti gli articoli della categoria
"cilmatizzazione", come valore dell'attributo indicato all'interno del
campo Passweb "**Attributo Articolo Codice Finalità**". All'interno
della categoria "cilmatizzazione" potremo quindi avere diverse tipologie
di articoli che possono essere tutte sottoposte all'incentivo per
l'efficienza energetica. A seconda della specifica tipologia ogni
articolo dovrà quindi avere per l'attributo indicato il suo specifico
"Codice finalità". Un possibile schema potrebbe essere il seguente

- Codice Finalità per Climatizzatori: 222

- Codice Finalità per Stufe a Pellet:333

- ...

Supponiamo ora di configurare tre distinti prodotti venduti all'interno
del sito come di seguito indicato

+----------------------+-----------------------+-----------------------+
| **ARTICOLO A -- cat. | **ARTICOLO B -- cat.  | **ARTICOLO C -- cat.  |
| Mobili**             | Mobili**              | Climatizzazione**     |
+======================+=======================+=======================+
| Codice PRF Articolo  | Codice PRF Articolo = | Codice PRF Articolo = |
| = 50190              | 50190                 | 20222                 |
|                      |                       |                       |
| Codice Finalità      | Codice Finalità       | Codice Finalità       |
| Articolo = 123       | Articolo = 456        | Articolo = 222        |
+----------------------+-----------------------+-----------------------+

Dovendo gestire due diverse tipologie di incentivi il pagamento
Findomestic dovrà essere configurato come nella figura di seguito
riportata

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\findomestic_incentivi_2.bmp](./assets/media/image98.png){width="5.779166666666667in"
height="3.4090277777777778in"}

In queste ipotesi potrebbero configurarsi tre diverse possibili
situazioni di acquisto:

**[CASO 1]{.underline}**

Viene inserito in ordine un solo prodotto di una specifica tipologia, ad
esempio l' **ARTICOLO C**.

In questo caso alla pagina di checkout l'utente avrebbe, in
corrispondenza del pagamento Findomestic, la possibilità di richiedere
il finanziamento con o senza l'incentivo statale relativo all'efficienza
energetica.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\findomestic_incentivi_3.bmp](./assets/media/image99.png){width="5.104166666666667in"
height="3.279166666666667in"}

**[CASO 2]{.underline}**

Vengono inseriti in ordine **contemporaneamente gli ARTICOLI A e B**
entrambi appartenenti alla categoria dei mobili.

In questo caso alla pagina di checkout l'utente avrebbe, in
corrispondenza del pagamento Findomestic, la possibilità di richiedere
il finanziamento con o senza l'incentivo statale relativo alla
ristrutturazione edilizia.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\findomestic_incentivi_4.bmp](./assets/media/image100.png){width="5.104166666666667in"
height="3.279166666666667in"}

**[CASO 3]{.underline}**

Vengono inseriti in ordine **contemporaneamente gli ARTICOLI A e C**
appartenenti a categorie sottoposte a diverse tipologie di incentivi.

In questo caso alla pagina di checkout l'utente avrebbe, in
corrispondenza del pagamento Findomestic, la possibilità di richiedere
un finanziamento standard con rateizzazione dell'importo ma senza
utilizzo di alcun tipo di incentivo.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\findomestic_incentivi_5.bmp](./assets/media/image101.png){width="5.104166666666667in"
height="3.279166666666667in"}

**ATTENZIONE!** Lo stesso risultato lo avremmo anche nel momento in cui
in ordine dovessero esserci solo articoli non sottoposti ad alcun tipo
di incentivo, oppure una situazione mista di articoli sottoposti ad un
certo incentivo e articoli non sottoposti a nessun incentivo

In questo caso per fare in modo che l'utente possa comunque richiedere
il finanziamento con il corretto incentivo dovremmo per forza di cose
ricorrere, laddove possibile, alla funzionalità di Passweb relativa alle
**Linee Articolo**

