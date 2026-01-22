# PAYPAL EXPRESS CHECKOUT -- ATTIVAZIONE ACCOUNT DI TEST



Una volta creato un account PayPal di test (per maggiori informazioni in
merito si vedano i precedenti capitoli di questo manuale) sarà poi
possibile prelevare direttamente dal sito developer i parametri
necessari per configurare la tipologia di pagamento "PayPal Express
Checkout" sul proprio sito Passweb collegandola all'ambiente Sandbox.

Nello specifico sarà quindi necessario portarsi, all'interno
dell'ambiente developer di PayPal, nella sezione "**Dashboard -- Sandbox
-- Accounts**"

selezionare un account di tipo Business, cliccare sul pulsante
raffigurante tre puntini posto in corrispondenza dell'account stesso, e
selezionare la voce "**View/edit account**"

![](./assets/media/image181.png)

La scheda "**API Credentials**", presente all'interno della maschera
così visualizzata, conterrà tutti i parametri necessari per collegare la
modalità di pagamento "PayPal Express Checkout" impostata sul proprio
sito Passweb a questo account di test.

![](./assets/media/image182.png)

Sarà quindi necessario copiare i valori presenti all'interno dei campi
**Username, Password** e **Signature** ed inserirli negli appositi campi
della maschera di configurazione del pagamento Passweb

![](./assets/media/image180.png)

**NOTA BENE**: in queste condizioni il parametro "Ambiente del Gateway"
deve ovviamente essere impostato sul valore "**Test**".

A questo punto sarà quindi possibile testare il corretto funzionamento
della modalità di pagamento in esame direttamente sul sito Passweb senza
impattare in alcun modo sul proprio account reale di PayPal.

