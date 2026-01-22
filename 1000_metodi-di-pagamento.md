# METODI DI PAGAMENTO



La sezione **"Pagamenti"** consente di selezionare, tra tutte quelle
presenti all'interno del gestionale, le diverse possibili modalità di
pagamento che verranno poi proposte al cliente che acquista sul web.

All'interno di questa pagina verrà quindi visualizzata la maschera
**"Lista dei Metodi di Pagamento"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\lista_modalita_pagamento.bmp](./assets/media/image1.png){width="5.850694444444445in"
height="3.545138888888889in"}

in cui verranno elencate tutte le modalità di pagamento codificate e
gestite all'interno della relativa tabella gestionale.

Il campo di ricerca attivabile cliccando sulla lente di ingrandimento,
presente in testata di ogni singola colonna, consente di filtrare i dati
in griglia sulla base dei valori presenti all'interno della colonna
stessa.

Una volta impostato un filtro di ricerca, per poterlo poi eliminare sarà
sufficiente cliccare sull'icona raffigurante una piccola lente di
ingrandimento con un -- all'interno (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_elimina_filtro.bmp](./assets/media/image2.png){width="7.777777777777778e-2in"
height="9.722222222222222e-2in"} ) che comparirà in testata alla colonna
in corrispondenza della quale è stato impostato il filtro stesso.

Infine è anche possibile ordinare, in maniera crescente e/o decrescente,
gli elementi in griglia cliccando semplicemente sull'icona raffigurante
due piccole frecce posta anch' essa in testata ad ogni singola colonna
della griglia (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_ordinamento_griglia.bmp](./assets/media/image3.png){width="0.12361111111111112in"
height="0.14930555555555555in"} )

**NOTA BENE:** per maggiori informazioni relative alla codifica ed alla
gestione dei pagamenti all'interno del gestionale si rimanda
all'apposita sezione del manuale di prodotto

**NOTA BENE:** nel caso in cui vengano apportate delle variazioni alla
tabella dei pagamenti all'interno del gestionale sarà poi necessario
lanciare una sincronizzazione manuale o attendere la prossima
sincronizzazione automatica in modo tale da riportare tali variazioni
anche all'interno del sito web.

Nel caso in cui dunque il pagamento desiderato compaia all'interno del
gestionale ma non ancora all'interno della maschera "Lista dei Metodi di
Pagamento" sopra evidenziata, sarà necessaria una sincronizzazione per
consentire a Passweb di importare anche le nuove modalità di pagamento.

**In ogni caso sarà possibile gestire ed attivare all'interno del sito
web unicamente una delle modalità di pagamento definite all'interno
dell'apposita tabella del gestionale.**

Il fatto di avere a disposizione all'interno della maschera sopra
evidenziata tutte le modalità di pagamento codificate e gestite
all'interno del gestionale, non significa però che tutte queste modalità
debbano necessariamente essere attivate anche all'interno del sito
e-commerce. Per ognuna di esse sarà infatti possibile decidere se
attivarla o meno anche all'interno del sito.

Per attivare una delle modalità di pagamento presenti in elenco e
renderla quindi disponibile ai vari clienti del sito web è sufficiente
selezionarla e cliccare poi sul pulsante **"Attiva Pagamento"** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_attiva_pagamento.bmp](./assets/media/image4.png){width="0.6298611111111111in"
height="0.16875in"} ) presente nella barra degli strumenti.

Allo stesso modo per disattivare una delle modalità precedentemente
attivate, è sufficiente selezionarla e cliccare poi sul pulsante
**"Disattiva Pagamento"** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_disattiva_pagamento.bmp](./assets/media/image5.png){width="0.6881944444444444in"
height="0.16875in"} ) presente nella barra degli strumenti.

**NOTA BENE:** all'interno del sito e-commerce i clienti potranno
scegliere unicamente tra le modalità di pagamento opportunamente
attivate o, eventualmente, il loro pagamento abituale.

**ATTENZIONE!** relativamente alla prenotazione di servizi/trattamenti
via web (Ecommerce Ho.Re.Ca.) verranno visualizzate, tra quelle attive,
le sole modalità di pagamento on line con carta di credito. **Le
modalità di pagamento NON con carta di credito, non verranno quindi mai
proposte in fase di prenotazione di un servizio/trattamento via web**

Il fatto di poter disporre o meno tra le varie scelte anche del proprio
pagamento abituale, dipende invece da quanto impostato per il parametro
"**Gestione del Pagamento Abituale"** all'interno della maschera
"Configurazione Ordini" di Passweb.

**NOTA BENE:** nel caso in cui il cliente abbia associato un pagamento
abituale, e si sia deciso di gestire anche questa modalità di pagamento,
il pagamento abituale risulterà essere la scelta di default.

**ATTENZIONE! Nel caso in cui l'utente non possa procedere alla conferma
dell'ordine a causa di un errata configurazione del sito, nello
specifico a causa dell'assenza di una qualche modalità di pagamento
effettivamente selezionabile, Passweb provvederà ad inviare
automaticamente all'amministratore del sito un'apposita mail di
notifica.**

A default i pagamenti presenti all'interno dei questa pagina assumeranno
la tipologia **"Pagamento del gestionale"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pagamenti_mexal.bmp](./assets/media/image6.png){width="5.8180555555555555in"
height="3.5256944444444445in"}

E' possibile personalizzare alcuni parametri di questi pagamenti,
modificandone l'etichetta identificativa o definendo ad esempio dei
costi aggiuntivi per lo specifico pagamento, e, soprattutto, è possibile
variarne la tipologia, **operazione questa indispensabile nel caso in
cui si voglia definire una modalità di pagamento on line tramite carta
di credito**.

In questo senso Passweb gestisce attualmente diverse possibili modalità
di pagamento on line mediante carta di credito.

Nello specifico sono gestiti i seguenti circuiti/gateway di pagamento:

1.  \@POS

2.  Afone paiment

3.  Axepta pHey

4.  Banca Sella

5.  BNL e-POSitivitiy

6.  Braintree

7.  CommerceWeb

8.  Findomestic -- Rateizzazione del pagamento

9.  NPG Consorzio Triveneto

10. Klarna -- Rateizzazione del pagamento

11. Nexi XPay

12. Numera NPGW

13. PagoLight -- Rateizzazione del pagamento

14. PayPal

15. PayPal Checkout

16. PayPal Express Checkout

17. PayWay di Sinergia

18. Raiffeisen

19. Safer Pay

20. Sardexnet

21. Satispay

22. Scalapay -- Rateizzazione del pagamento

23. Sia VPOS

24. Soisy -- per richiesta di finanziamenti online (obsoleto)

25. Stripe

26. SumUp

27. T.P@Y.SM

28. Unicredit PagoOnline Imprese

29. Unicredit PagoOnline (Obsoleto)

**NOTA BENE:** per maggiori informazioni relativamente all'attivazione e
alla gestione di una delle varie modalità di pagamento mediante carta di
credito si rimanda ai successivi capitoli di questo manuale.

Una volta impostato e configurato un pagamento on line, la relativa
tipologia verrà visualizzata in corrispondenza della colonna "**Metodo
di Pagamento**" presente all'interno della maschera "Lista dei metodi di
Pagamento".

