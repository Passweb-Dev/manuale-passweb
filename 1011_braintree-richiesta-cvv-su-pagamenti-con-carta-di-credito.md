# BRAINTREE -- RICHIESTA CVV SU PAGAMENTI CON CARTA DI CREDITO



Come evidenziato nei precedenti capitoli di questo manuale, nel momento
in cui si dovesse decidere di abilitare, tra le opzioni messe a
disposizione da Braintree, il pagamento mediante carta di credito sarà
poi possibile decidere anche di attivare o meno la richiesta del CVV
della carta come ulteriore misura di sicurezza.

Per far questo sarà però necessario agire direttamente dal Backoffice di
Braintree secondo quanto indicato al seguente link
<https://developer.paypal.com/braintree/articles/guides/fraud-tools/basic/avs-cvv-rules>

- Accedere quindi al backoffice del proprio account Braintree, cliccare
  sul menu delle impostazioni presente in testata (icona raffigurante
  una piccola rotellina) e selezionare la voce "**Fraud Management**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\braintree_cvv.bmp](./assets/media/image77.png)

- Cliccare sul link "**Options**" presente in corrispondenza della
  sezione CVV

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\braintree_cvv_2.bmp](./assets/media/image78.png)

- Selezionare quindi, tra le opzioni proposte, il / i criteri che
  dovranno essere applicati, in relazione al CVV, per rifiutare o meno
  la transazione.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\braintree_cvv_3.bmp](./assets/media/image79.png)

> Per ciascuna delle opzioni disponibili sarà poi possibile decidere se
> applicarla a tutte le transazioni o solo ad alcune

**ATTENZIONE!** Come indicato nella relativa documentazione ufficiale
(**cui si consiglia di fare sempre riferimento**), attivando questo tipo
di controllo le transazioni verranno poi rifiutate nel momento in cui
anche solo una delle regole attivate dovesse effettivamente non essere
soddisfatta

