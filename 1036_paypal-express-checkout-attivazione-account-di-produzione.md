# PAYPAL EXPRESS CHECKOUT -- ATTIVAZIONE ACCOUNT DI PRODUZIONE



Una volta verificato il corretto funzionamento della modalità di
pagamento "PayPal Express Checkout" sul proprio ambiente Sandbox sarà
necessario cambiare la configurazione di questa modalità di pagamento
collegandola al proprio account di produzione.

**ATTENZIONE**: **i parametri "Username" "Password" e "Signature"
utilizzati per l'account di test e prelevati dall'ambiente developer di
PayPal sono validi solo ed esclusivamente per l'account definito
sull'ambiente Sandbox. Per abilitare pagamenti reali vanno impostati i
parametri collegati al proprio account reale di PayPal**

Per fare questo quindi sufficiente impostare nella maschera di
configurazione del pagamento Passweb i parametri **API Username, API
Password e API Signature** collegati al proprio account di produzione di
PayPal, parametri questi reperibili non più all'interno dell'ambiente
developer ma operando direttamente su paypal.com all'interno del proprio
account.

Nello specifico sarà quindi necessario:

1.  accedere su paypal.com al proprio account e portarsi poi nella
    sezione "**Il mio Conto -- Profilo -- Strumenti di Vendita**"

2.  cliccare sul pulsante "**Aggiorna**" presente in corrispondenza
    della voce "**Accesso API**" presente nella sezione **"Vendite
    online"**

3.  cliccare sul pulsante "**Richiedi Credenziali API**" presente in
    corrispondenza dell' "**Opzione 2**"

4.  nella maschera "**Richiedi Credenziali API**" selezionare l'opzione
    **"Richiedi una firma API"**.

5.  cliccando infine sul pulsante "**Accetto e invio**", presente nella
    maschera sopra riportata l'utente verrà ricondotto alla pagina
    "**Vedi o rimuovi firma API**" da cui poter prelevare i parametri
    necessari per poter configurare il pagamento "PayPal Express
    Checkout" definito all'interno del sito e-commerce sul proprio
    account PayPal di produzione.

6.  Per completare la configurazione sarà quindi sufficiente copiare il
    valore di questi parametri all'interno dei corrispondenti campi
    presenti nella maschera di configurazione del pagamento Passweb

**NOTA BENE**: in queste condizioni il parametro "Ambiente del Gateway"
deve ovviamente essere impostato sul valore "**Produzione**".

