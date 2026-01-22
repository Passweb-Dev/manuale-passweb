# BRAINTREE -- GOOGLE PAY



Come evidenziato nei precedenti capitoli di questo manuale, nel momento
in cui si dovesse decidere di abilitare, tra le opzioni messe a
disposizione da Braintree, il pagamento mediante Google Pay non sarà
sufficiente attivare l'apposito flag all'interno di Passweb ma, affinché
tutto possa funzionare in maniera adeguata, sarà necessario configurare
correttamente il pagamento Google Pay anche all'interno del backoffice
di Braintree secondo quanto indicato al seguente link
<https://developer.paypal.com/braintree/docs/guides/google-pay/configuration/javascript/v3>

Nello specifico sarà dunque necessario:

- Accedere al proprio account Braintree, aprire il menu delle
  impostazioni (icona raffigurante una piccola rotellina posta in
  testata) e selezionare la voce "Processing"

![](./assets/media/image85.png)

- All'interno della sezione Payment Methods attivare l'interruttore
  presente in corrispondenza della sezione "**Google Pay**" e, se
  richiesto, approvare i relativi termini e condizioni

![](./assets/media/image90.png)

**ATTENZIONE!** si ricorda che in ambiente di produzione sarà necessario
impostare, nei parametri di configurazione Passweb anche il **Google
Merchant ID (Google Pay)** ossia l'ID Google relativo all'account di
produzione, su cui verranno poi dirottati i pagamenti

In fase di test con account Sandbox il Google Merchant ID non è
necessario e il relativo campo può anche essere lasciato vuoto

