# OPZIONE DI OPT-OUT



Come indicato nei precedenti capitoli di questo manuale in determinate
configurazioni di Clerk (visitor auto) potrebbe essere necessario
inserire sul sito un'opzione di Opt-Out che consenta di bloccare, per
tutti gli utenti che dovessero esercitarla, qualsiasi tipo di
tracciamento e/o di modulo Clerk presente sul sito stesso.

Per poter implementare questa opzione sarà necessario, nello specifico:

- Creare un Attributo Cliente Passweb, di tipo Testo, che dovrà poi
  essere utilizzato per memorizzare questo tipo di consenso

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\privacy_clerk_optout.bmp](./assets/media/image70.png){width="5.6625in"
height="3.5194444444444444in"}

- Impostare il parametro "**Attributo OPT OUT**" presente nel tab
  "**Configurazione**" (sezione "**Parametri Store**") della maschera di
  configurazione dell'account Clerk sull' Attributo Cliente creato al
  punto precedente

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\privacy_clerk_optout_0.bmp](./assets/media/image71.png){width="5.467361111111111in"
height="3.623611111111111in"}

- Inserire nei form di Registrazione e Profilo Utente un componente
  "**Campo Checkbox**" mappato sull'Attributo Cliente di cui ai punti
  precedenti

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\privacy_clerk_optout_1.bmp](./assets/media/image72.png){width="3.967361111111111in"
height="3.1430555555555557in"}

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\privacy_clerk_optout_2.bmp](./assets/media/image73.png){width="5.6625in"
height="3.5194444444444444in"}

In questo modo per gli utenti non autenticati, così come per quelli
autenticati che non hanno esercitato questa specifica opzione, tutti i
moduli Clerk presenti sul sito continueranno a funzionare normalmente
secondo quelli che sono i vari parametri settati in fase di
configurazione dell'integrazione tra le due piattaforme.

Al contrario nel momento in cui un utente autenticato dovesse decidere
di esercitare questa opzione, lo script di configurazione di Clerk non
verrà più eseguito, il sistema di tracciamento non inveirà alcun dato
relativo alla sessione di navigazione alla piattaforma terza e eventuali
moduli Clerk presenti sul sito (Ricerca, Raccomandazioni, Chat ...)
verranno automaticamente disabilitati.

