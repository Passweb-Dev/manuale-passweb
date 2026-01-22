# IMPLEMENTARE GOOGLE ANALYTICS CON GTM



**ATTENZIONE! Implementare correttamente il tracciamento ecommerce di
Google Analytics mediante Google Tag Manager richiede una certa
dimestichezza con script, oggetti javascript e funzionalità avanzate di
tracciamento di web analytics.**

Si ricorda inoltre che i tracciamenti "nativi" di Google Tag Manager
potrebbero non essere completamente supportati da Passweb, che ha una
sua struttura del dataLayer, e potrebbero quindi portare ad un
monitoraggio non corretto dei vari eventi. **Per la creazione dei tag,
degli attivatori e delle relative variabili in Google Tag Manager si
consiglia di seguire le indicazioni contenute all'interno di questo
manuale"**

Nei successivi capitoli vedremo quindi come poter attivare il
tracciamento di Google Analytics mediante GTM sia a livello base
(facendo riferimento cioè al solo tracciamento della pagine visitate)
che a livello ecommerce

**ATTENZIONE! in ogni caso è assolutamente sconsigliato il fatto di
gestire un sistema di tracciamento in modalità mista** dove alcuni
eventi sono tracciati direttamente dal sito e altri mediante Tag
Manager. In questi casi infatti si perderebbe facilmente il controllo di
cosa viene eseguito prima e dopo (soprattutto nell'ottica di gestione
della Consent Mode) e si potrebbe quini incorrere, molto facilmente, in
errori di tracciamento

