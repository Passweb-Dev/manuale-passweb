# BRAINTREE -- APPLE PAY



Come evidenziato nei precedenti capitoli di questo manuale, nel momento
in cui si dovesse decidere di abilitare, tra le opzioni messe a
disposizione da Braintree, il pagamento mediante Apple Pay non sarà
sufficiente attivare l'apposito flag all'interno di Passweb ma, affinché
tutto possa funzionare in maniera adeguata, sarà necessario configurare
correttamente il pagamento Apple Pay anche all'interno del backoffice di
Braintree secondo quanto indicato al seguente link
<https://developer.paypal.com/braintree/docs/guides/apple-pay/configuration/javascript/v3>

**ATTENZIONE!** Per poter utilizzare Apple Pay è necessario disporre di
un' Account Apple developer correttamente funzionante. Si ricorda
inoltre che l'iscrizione ad un programma developer di Apple generalmente
richiede un contributo annuale (per maggiori informazioni in merito si
rimanda alla relativa documentazione disponibile sul portale
sviluppatori di Apple)

Come indicato anche nella documentazione ufficiale di Braintree per
poter testare in ambiente Sandbox sarà necessario essere autenticati in
un "**iTunes Connect sandbox tester account**" che dovrà essere
preventivamente cerato all'interno di un **Apple Developer Account**

Allo stesso modo ovviamente per poter concludere dei pagamenti in
ambiente di produzione sarà necessario in un Account iCloud reale

Per attivare tutto quanto richiesto si consiglia di fare sempre
riferimento alla documentazione (o direttamente al supporto) Braintree
e/o Apple disponibile, ad esempio ai seguenti link

<https://developer.paypal.com/braintree/docs/guides/apple-pay/configuration/javascript/v3>

<https://developer.apple.com/apple-pay/sandbox-testing/>

<https://developer.apple.com/documentation/passkit/apple_pay/setting_up_apple_pay>

<https://developer.apple.com/help/account/configure-app-capabilities/configure-apple-pay#create-a-merchant-identifier>

**ATTENZIONE!** si ricorda che l'opzione Apple Pay compaia
effettivamente tra le possibili opzioni di pagamento messe a
disposizione da Braintree è necessario che il sito sia protetto da un
certificato SSL e risponda dunque ad un indirizzo del tipo https://\...

E' bene ricordare inoltre che Apple Pay è disponibile solamente in
Safari su iOS versione 10+ e su macOS versione 10.12+

Nel momento in cui Apple Pay non dovesse essere supportata dal browser
utilizzato (ad esempio perché l'utente sta navigando con Chrome su
dispositivo Windows) l'opzione "Apple Pay" come possibile pagamento
messo a disposizione da Braintree non verrà ovviamente visualizzata

Una volta configurato tutto quanto richiesto nei vari ambienti Apple,
sarà poi necessario:

- Accedere al proprio account Braintree, aprire il menu delle
  impostazioni (icona raffigurante una piccola rotellina posta in
  testata) e selezionare la voce "Processing"

![](./assets/media/image85.png)

- All'interno della sezione Payment Methods attivare l'interruttore
  presente in corrispondenza della sezione "**Apple Pay**"

![](./assets/media/image88.png)

- Nella successiva maschera di configurazione seguire la procedura
  indicata per caricare un Apple Merchant Certificate correttamente
  generato (richiede l'accesso al proprio Apple Developer Account),
  indicare il dominio del proprio sito web e cliccare, infine, sul
  pulsante "**Done**"

![](./assets/media/image89.png)

