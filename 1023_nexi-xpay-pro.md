# NEXI XPAY PRO



Questa modalità di pagamento online viene riconosciuta e gestita da
tutte le banche appoggiate al gateway di pagamento **Nexi** **XPay**.

**ATTENZIONE!** **Il gateway di Nexi mette a disposizione diverse
modalità di pagamento (XPay Pro, Xpay Easy, XPay Web ...) si consiglia
quindi di verificare attentamente che la modalità di pagamento attivata
sia effettivamente una di quelle disponibili per il proprio sito
Passweb**

Per poter attivare questa specifica modalità di pagamento in Passweb
sarà necessario:

1.  Codificare all'interno della Tabella Pagamenti del gestionale uno
    specifico pagamento al quale poter poi agganciare il pagamento on
    line in oggetto assegnandogli, ad esempio, la descrizione Nexi XPay

2.  Effettuare una sincronizzazione sito -- gestionale in modo tale da
    rendere disponibile questo nuovo pagamento anche in Passweb
    all'interno della maschera **"Lista dei Metodi di Pagamento"**
    precedentemente esaminata.

3.  Attivare questa nuova modalità di pagamento secondo quanto descritto
    nel capitolo *"Configurazione Modalità di Pagamento"* di questo
    manuale.

4.  Impostare in maniera corretta i parametri specifici per questa
    particolare modalità di pagamento.

In particolare per poter eseguire quest'ultimo passaggio sarà necessario
selezionare il pagamento in oggetto all'interno della maschera **"Lista
dei Metodi di Pagamento"** e cliccare sul pulsante "**Modifica
Pagamento**", presente nella barra degli strumenti.

Verrà quindi visualizzata la maschera di configurazione e
personalizzazione del pagamento, all'interno della quale sarà necessario
impostare, oltre ai parametri classici di configurazione del pagamento,
anche quelli specifici del gateway attualmente considerato e presenti
all'interno della sezione "**Parametri Gateway**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\configurazione_carta_si.bmp](./assets/media/image121.png){width="5.565277777777778in"
height="3.825in"}

Nel caso specifico il parametro

- **Ambiente del Gateway:** permette di definire se utilizzare come
  ambiente del pagamento, l'ambiente di test (da utilizzare solo ed
  esclusivamente in fase di sviluppo del sito) oppure l'ambiente reale
  di produzione.

- **Soluzione**: consente di impostare la tipologia di pagamento che
  verrà poi utilizzata all'interno del gateway. E' possibile selezionare
  una delle seguenti opzioni:

  - **Pagamento Semplice / One Click:** in questo caso il gateway
    gestirà dei pagamenti online "tradizionali". In realtà in queste
    condizioni sarà poi possibile decidere se configurare il pagamento
    in maniera tale che l'utente debba ogni volta inserire i dati della
    propria carta di credito (sezione "**Pagamento Semplice**") oppure
    se configurarlo in maniera tale che l'utente abbia anche la
    possibilità di memorizzare le proprie carte così da poter concludere
    più rapidamente l'ordine senza dover ogni volta digitare tutti i
    dati (sezione "**Pagamento One Click**")

> **ATTENZIONE!** Per maggiori informazioni in merito alla
> configurazione dei pagamenti Semplici e One Click si vedano i
> successivi capitoli ("*Pagamenti Semplici*" e "*Pagamenti One Click*")
> di questo manuale

- **Pagamento Ricorrente**: selezionando questa opzione sarà invece
  possibile gestire all'interno di Nexi dei pagamenti ricorrenti (es.
  per servizi in abbonamento)

> **ATTENZIONE!** per maggiori informazioni relativamente a come vengono
> gestiti i pagamenti ricorrenti nell'integrazione Passweb -- Nexi si
> veda quanto indicato nel successivo capitolo ("*Pagamenti
> Ricorrenti*") di questo manuale

