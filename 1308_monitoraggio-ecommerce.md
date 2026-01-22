# MONITORAGGIO ECOMMERCE



Come evidenziato nei precedenti capitoli di questo manuale in GA4 il
processo di attivazione e gestione del tracciamento ecommerce è stato,
sotto certi punti di vista, semplificato nel senso che essendo il data
model del nuovo sistema di tracciamento incentrato interamente sugli
eventi non è più necessario attivare determinate configurazioni a
livello di account Analytics per poter gestire anche il monitoraggio
ecommerce ma, molto più semplicemente, è sufficiente tracciare anche
quelli che sono i diversi eventi ecommerce esattamente allo stesso modo
in cui dovranno essere tracciati tutti gli altri eventi di interesse per
il proprio sito.

**ATTENZIONE!** in GA4, gli eventi ecommerce rientrano tra quelli
definiti come "**Eventi Consigliati**", non sono quindi raccolti da
Google in maniera automatica ne possono essere collezionati con
l'attivazione di un semplice check come si fa invece per gli "Eventi di
misurazione avanzata". Sotto questo punto di vista dunque anche in GA4
sarà necessario implementare (direttamente all'interno del sito o
mediante GTM) il codice necessario per inviare a GA4 gli eventi
ecommerce da tracciare assieme ai relativi parametri.

In questo senso dunque, nel momento in cui l'esigenza dovesse essere
quella di attivare il tracciamento degli eventi ecommerce, sfruttando
l'integrazione diretta Passweb -- Analytics, sarà necessario portarsi
alla pagina "**Sito -- Preferenze**" del Wizard (tab "**Tracciamento
Dati**") e verificare di aver correttamente impostato correttamente i
seguenti parametri:

- **Google Analytics Ricerca sul sito**

- **Google Analytics -- Eventi Articolo**

- **Google Analytics -- Eventi Carrello e Wishlist**

- **Google Analytics -- Eventi Checkout**

- **Google Analytics -- Eventi Utente**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sito_preferenze_eventi_ecommerce.bmp](./assets/media/image19.png)

Ciascuno dei parametri indicati consente infatti a Passweb, se
opportunamente abilitato, di attivare il codice necessario per inviare
alla corrispondente proprietà GA4 determinati eventi ecommerce come ad
esempio la visualizzazione di una lista di articoli, l'aggiunta o la
rimozione di articoli dal carrello, il completamento di un ordine ecc...

**ATTENZIONE!** per attivare un tracciamento ecommerce completo è
necessario abilitare tutti i parametri sopra indicati. Nel momento in
cui alcuni di essi non dovessero essere abilitati gli eventi
corrispondenti non verranno inviati ad Analytics e non faranno quindi
parte del sistema di tracciamento ecommerce attivo sul proprio sito

Nei successivi capitoli di questo manuale verranno analizzati nei
dettagli tutti gli eventi ecommerce attualmente gestiti da Passweb (e
che rientrano tra gli "Eventi Consigliati" da Google).

Nel momento in cui l'esigenza dovesse essere invece quella di gestire il
tracciamento Ecommerce mediante GTM è possibile fare riferimento a
quanto indicato nel relativo capitolo di questo manuale (*"Google Tag
Manager -- Implementare Google Analytics con GTM -- GTM e GA4"*) e,
soprattutto, alla documentazione specifica di GTM (che come noto è un
tool google esterno e indipendente da Passweb)

