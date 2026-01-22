# CONSENT MODE



Un altro aspetto di fondamentale importanza da prendere in
considerazione in fase di attivazione e configurazione del proprio
sistema di tracciamento mediante GA4 è l'utilizzo, ormai
imprescindibile, della Consent Mode.

Dal punto di vista tecnico la Consent Mode è un API aperta sviluppata da
Google per offrire maggiore flessibilità nell'utilizzo dei suoi prodotti
(Google Analytics, Google Ads, Tag Manager ...) lavorando in
collaborazione con le piattaforme di gestione del consenso dei cookie, i
cosiddetti Consent Management Platform o CMP (tanto per capirci i vari
Cookiebot, Iubenda, OneTrust ...).

Grazie alla Consent Mode sarà possibile recuperare informazioni
fondamentali per quel che riguarda sia l'analisi statistica che
l'efficacia delle campagne di marketing digitale anche nel momento in
cui gli utenti dovessero avere negato il consenso all'installazione dei
cookie, il tutto ovviamente, sempre nel pieno rispetto di quanto
previsto dal GDPR.

Le informazioni che verranno inviate ai sistemi di Google (Analytics,
AdWords ...) nel momento in cui la Consent Mode dovesse essere
implementata in maniera corretta e l'utente dovesse aver negato,
mediante l'apposito banner offerto dalla piattaforma di CMP in uso al
sito, l'installazione dei cookie, saranno infatti in forma aggregata e
non identificativa il che, da una parte, consente di rispettare le
volontà dell'utente e il GDPR e dall'altra parte consente comunque di
poter dare in pasto ai sistemi di intelligenza artificiale e di
modellazione dei dati di Google informazioni utili per recuperare dati
statistici e conversioni che altrimenti andrebbero perse in maniera
definitiva.

Inoltre i tag e gli script di Google che utilizzano la Consent Mode
potranno modificare immediatamente il loro comportamento se l'utente
dovesse decidere di cambiare i propri consensi in un secondo momento e
tutto questo potrà avvenire anche in maniera completamente automatica
grazie all'integrazione tra la Consent Mode e la piattaforma di CMP in
uso al sito. Generalmente infatti sarà proprio questa piattaforma che,
utilizzando l'API della Consent Mode, andrà ad aggiornare
automaticamente lo stato dei consensi in base alle scelte effettuate
dall'utente nel banner di gestione dei Cookie.

Una cosa di fondamentale importanza che emerge subito da questi primi
concetti è quindi che **la Consent Mode non è un sistema di cookie
management, non sostituisce strumenti di gestione dei cookie come
Iubenda, CookieBot, OneTrust ...** **strumenti questi che dovranno
quindi essere ancora assolutamente utilizzati** sia perché si integrano
con la Consent Mode rendendo tutto il sistema più semplice da gestire
(come detto saranno loro infatti ad aggiornare automaticamente lo stato
del consenso degli utenti attivando o disattivando tag e script di
Google) sia perché, al momento, la Consent Mode funziona solo sui tag e
sugli script di Google.

Tanto per fare un esempio la Consent Mode è totalmente inefficace sui
pixel di Facebook che dovranno quindi continuare ad essere bloccati in
maniera preventiva dal sistema principale (CMP) di gestione dei cookie.

Chiarito questo primo aspetto di fondamentale importanza vediamo ora in
maniera un po' più tecnica come lavora la Consent Mode e come rende
effettivamente possibile quanto appena visto.

In questo senso va detto che per regolare il comportamento dei Tag e/o
degli script di tracciamento, Google ha introdotto **specifiche
tipologie di consenso** che gestiscono i cookie rilasciati da questi
stessi servizi:

Tali consensi sono:

- **ad_storage**

- **ad_user_data**

- **ad_personalization**

- **analytics_storage**

- **functionality_storage**

- **personalization_storage**

- **security_storage**

vediamoli nel dettaglio:

**[ad_storage]{.underline}**

**Controlla il comportamento dei cookie per finalità pubblicitarie,
inclusa la misurazione delle conversioni presenti sul sito**.

Corrisponde al "**Consenso Marketing**" presente nel cookie banner della
CMP in uso al sito

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\CMP_consenso_marketing.bmp](./assets/media/image7.png){width="2.9555555555555557in"
height="2.395138888888889in"}

A seconda della scelta effettuata dall'utente in merito a questa
specifica tipologia di consenso, il tag o lo script in uso al sito andrà
quindi ad utilizzare normalmente i cookie di marketing (nel caso di
consenso fornito) oppure (nel caso di consenso negato) potrà comunque ad
attribuire conversioni tramite appositi segnali (ping) inviati ai server
di Google utilizzando i suoi sistemi di modellazione dei dati e di
intelligenza artificiale.

In sostanza Google la mette in questo modo. Diciamo che qualcuno visiti
il sito e produca una conversione. Se quell'utente, prima della
conversione, aveva fornito il consenso ai cookie di marketing, mediante
la corrispondente opzione presente nel pop-up fornito dalla piattaforma
CMP in uso al sito stesso, il tutto si svolgerà normalmente senza nessun
tipo di blocco e la conversione potrà essere correttamente registrata
senza dover ricorrere ad una qualsiasi modellazione dei dati.

Nel caso in cui l'utente dovesse invece aver negato il consenso
Marketing, il tag o lo script di tracciamento si adatterà a questa
scelta e, conseguentemente, non verranno quindi utilizzati da Google
Analytics cookie di marketing.

Nonostante ciò, dipendentemente dal fatto di utilizzare la Consent Mode
Base o Avanzata, potrebbe comunque essere ancora possibile inviare ad
Analytics dati di tracciamento e sulle conversioni, anche se,
ovviamente, ad un livello più aggregato (mediante specifici ping)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ga4_63.bmp](./assets/media/image8.png){width="3.6430555555555557in"
height="1.8215277777777779in"}

Lo stesso Google afferma che
(<https://blog.google/products/marketingplatform/360/conversion-modeling-through-consent-mode-google-ads/>
) grazie all'utilizzo della Consent Mode è possibile recuperare più del
70% delle conversioni provenienti dagli annunci Google Ads che
altrimenti andrebbero perse a causa delle scelte di consenso degli
utenti

**[ad_user_data / ad_personalization]{.underline}**

Permessi introdotti con la Consent Mode v2 (attiva a partire da Marzo
2024).

Come per ad_storage anche ad_user_data / ad_personalization sono
controllati dal consenso marketing presente nel cookie banner della CMP
in uso al sito

Nello specifico:

- **ad_user_data**: indica il consenso dell'utente **alla condivisione
  dei dati personali con Google per scopi pubblicitari**. Se l'utente
  concede questo consenso, i tag pubblicitari di Google possono
  utilizzare dati come ID utenti, email hashing, ecc., per il
  tracciamento e la misurazione avanzata delle conversioni. Se negato,
  viene disattivata la raccolta di dati utente personali usati in
  advertising, incluse funzionalità come "enhanced conversions"

- **ad_personalization**: indica il consenso dell'utente **all'utilizzo
  dei propri dati per finalità di personalizzazione pubblicitaria**, ad
  esempio remarketing o annunci basati sugli interessi Se l'utente
  concede questo consenso, Google può mostrare annunci personalizzati in
  base al comportamento, interessi e dati raccolti. In caso contrario,
  tali forme di targeting personalizzato saranno disattivate

**ATTENZIONE!** Come indicato nei cookie banner delle CMP generalmente
questi consensi sono legati al check "Marketing" per cui attivando il
relativo flag verranno automaticamente concessi tutti e 3 i consensi
ad_storage, ad_user_data e ad_personalization

**[analytics_storage]{.underline}**

**Controlla il comportamento dei cookie statistici**

Corrisponde al "**Consenso Misurazione**" presente nel cookie banner
della CMP in uso al sito

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\CMP_consenso_misurazione.bmp](./assets/media/image9.png){width="2.936111111111111in"
height="2.401388888888889in"}

In conseguenza di ciò nel momento in cui un utente dovesse accettare i
cookie analitici/statistici, questi verranno utilizzati normalmente e il
tracciamento verrà quindi eseguito in modalità "standard". In queste
condizioni verranno raccolti da Google Analytics tutti i dati di
tracciamento e sarà possibile, ad esempio, visualizzare le relative
visite al sito tanto nei report in tempo reale quanto nella Debug View
di GA4.

Nel momento in cui l'utente dovesse invece negare il consento
all'utilizzo dei cookie analitici non verrà installato ed utilizzato
alcun tipo di cookie correlato a Google Analytics. In queste condizioni
quindi non sarà possibile registrare "normalmente" la visita al sito da
parte dell'utente e non sarà possibile visualizzarla né nei report in
tempo reale né tanto meno nella Debug View di GA4

Tuttavia, anche in questo caso, dipendentemente dal fatto di aver
implementato la Consent Mode Avanzata o quella Base potranno comunque
essere inviati ai server di Google Analytics dei segnali (ping) privi di
cookie utili per la misurazione di base e per scopi di modellazione
futuri. Questi dati sono in forma aggregata e contengono solamente
informazioni su visitatori e pagine visitate, quindi non possono essere
usati, ad esempio, per scopi di retargeting.

**[functionality_storage]{.underline}**

**Controlla il comportamento dei cookie utilizzati per l'archiviazione
di informazioni che supportano le funzionalità del sito web** (es. le
impostazioni relative alla lingua)

Corrisponde al "**Consenso Funzionalità**" presente nel cookie banner
della CMP in uso al sito

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\CMP_consenso_funzionalita.bmp](./assets/media/image10.png){width="2.936111111111111in"
height="2.401388888888889in"}

**[personalization_storage]{.underline}**

**Controlla il comportamento dei cookie utilizzati per l'archiviazione
di informazioni relative alla personalizzazione** (es. i consigli sui
video). Non riguarda l'advertising

Corrisponde al "**Consenso Esperienza**" presente nel cookie banner
della CMP in uso al sito

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\CMP_consenso_esperienza.bmp](./assets/media/image11.png){width="2.936111111111111in"
height="2.395138888888889in"}

**[security_storage]{.underline}**

**Controlla il comportamento dei cookie utilizzati per l'archiviazione
di informazioni relative alla sicurezza,** (es. la funzionalità di
autenticazione, la prevenzione delle frodi e altre protezioni per gli
utenti).

In genere questo consenso rientra come parte della categoria
**Necessari** delle varie CMP (quindi pre-abilitata e non
disattivabile), proprio perché senza questi cookie il sito potrebbe non
funzionare correttamente dal punto di vista della sicurezza

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\CMP_consenso_necessari.bmp](./assets/media/image12.png){width="2.942361111111111in"
height="2.3881944444444443in"}

**ATTENZIONE!** sulla base di quanto detto, di fatto i consensi che
regolano l'utilizzo dei cookie da parte di Google Analytics sono
ad_storage e analytics_storage (che corrispondono rispettivamente ai
flag "Marketing" e "Misurazione" presenti nel cookie banner della CMP in
uso al sito)

In generale dunque, quando gli utenti concedono il consenso, i tag e gli
script di Google funzioneranno normalmente. Quando invece gli utenti
negano il consenso, i tag e gli script Google associati non andranno a
memorizzare e ad utilizzare nessun tipo di cookie. Anche in queste
condizioni (cookie non memorizzati), l'attività dell'utente sul sito
potrebbe comunque causare l'invio ai server di Google di appositi
segnali (ping) utili a comunicare lo stato del consenso e il
comportamento dell'utente:

Nello specifico i ping inviati ai sistemi di Google, nel momento in cui
l'utente non dovesse concedere i consensi (e nel caso in cui si sia
deciso di implementare la Consent Mode Avanzata) saranno di tre tipi
diversi:

- **Stato del consenso**: vengono inviati da ogni pagina visitata
  dall'utente in cui è implementata la modalità di consenso. Comunicano
  lo stato del consenso espresso dall'utente in merito all'utilizzo
  delle varie categorie di cookie. Questo stesso ping verrà tramesso,
  ovviamente, anche nel caso in cui il consenso prestato dall'utente
  dovesse essere modificato in maniera tale da aggiornare immediatamente
  i sistemi di Google in merito alla scelta effettuata.

- **Conversioni**: vengono inviati per indicare che si è verificata una
  conversione

- **Google Analytics**: vengono inviati da ogni pagina del sito in cui è
  stato implementato Google Analytics, registrando tutte le visite e gli
  eventi.

Tali ping possono includere:

- Informazioni funzionali (come le intestazioni aggiunte passivamente
  dal browser) :

- Timestamp

- User Agent

- Referrer, vale a dire in che modo l\'utente è approdato sul tuo sito
  web

- Informazioni aggregate/non identificative:

- Un'indicazione relativa al fatto che la pagina corrente o una pagina
  precedente nella navigazione dell'utente possa includere o meno,
  nell'URL, informazioni sui click degli annunci (es. GCLID / DCLID)

- Informazioni booleane sullo stato del consenso

- Numero casuale per ogni caricamento di pagina.

Di seguito alcuni indirizzi dove poter trovare documentazione ufficiale
di Google relativamente Consent Mode

<https://developers.google.com/tag-platform/devguides/privacy>

<https://developers.google.com/tag-platform/devguides/consent#gtag.js>

<https://www.iubenda.com/it/help/27154-google-consent-mode>

<https://support.cookiebot.com/hc/en-us/articles/360016047000-Cookiebot-and-Google-Consent-Mode>

