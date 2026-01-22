# INSTALLAZIONE DI GA4 CON GOOGLE TAG MANAGER



Il processo di installazione di Google Analytics 4 mediante GTM passa
attraverso due step fondamentali:

1.  Creazione e attivazione di una proprietà GA4 (operazione da eseguire
    in Google Analytics)

2.  Installazione di GTM e collegamento con la proprietà GA4

Per maggiori informazioni relativamente allo step 1 si rimanda a quanto
indicato all'interno del capitolo "*Google Analytics -- Google analytics
4 -- Creazione e attivazione di una proprietà GA4*" di questo manuale o
alla specifica documentazione presente in rete.

Una volta completato lo step 1 e creata quindi la proprietà GA4 e il
relativo Stream di Dati, il passo successivo è quello che prevede di
creare con GTM i tag di monitoraggio da installare sul sito web.

In questo senso sarà dunque necessario:

1.  Accedere quindi all'interfaccia di amministrazione di GTM, portarsi
    nella dashboard di gestione del Contenitore su cui si desidera
    operare e cliccare sul pulsante "**Aggiungi un uovo Tag**"

![Videate\\gtm_15b.bmp](./assets/media/image36.png){width="5.586111111111111in"
height="3.4458333333333333in"}

2.  Cliccare sul pulsante "**Scegli un tipo di tag per iniziare
    l'installazione**" presente all'interno del box "**Configurazione
    Tag**"

![Videate\\gtm_ecommerce_avanzato_10.bmp](./assets/media/image37.png){width="5.33125in"
height="3.3569444444444443in"}

3.  Selezionare tra quelli proposti il tag relativo alla configurazione
    di GA4 "**Google Analytics: configurazione GA4"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ga4_10.bmp](./assets/media/image38.png){width="5.184722222222222in"
height="3.477777777777778in"}

> Nella successiva maschera di configurazione del tag impostare
> all'interno del relativo campo l' **ID Misurazione** (G-XXXXXXXXXX)
> della proprietà GA4 relativo allo Stream di Dati precedentemente
> creato in Analytics (volendo si potrebbe pensare di creare anche
> un'apposita constante da inserire in questo campo esattamente allo
> stesso modo di quanto fatto per l'ID Monitoraggio UA che si utilizzava
> in Universal Analytics)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ga4_11.bmp](./assets/media/image39.png){width="5.184722222222222in"
height="3.477777777777778in"}

> Accertarsi inoltre di aver selezionato il flag "**Invia un evento di
> visualizzazione pagina quando viene caricata questa configurazione**"
> come evidenziato nella figura sopra riportata, in modo tale da
> tracciare automaticamente le visualizzazioni di pagina

4.  Completata la configurazione del Tag sarà ora necessario decidere
    dove questo stesso Tag dovrà essere attivato. Cliccare quindi sul
    pulsante "**Scegli un attivatore per attivare questo tag**"

![Videate\\ga4_12.bmp](./assets/media/image40.png){width="5.184722222222222in"
height="3.477777777777778in"}

> e selezionare tra gli attivatori proposti l'opzione "**All Pages /
> Visualizzazione di pagina**"

![Videate\\gtm_35B.bmp](./assets/media/image41.png){width="5.598611111111111in"
height="3.248611111111111in"}

> In questo modo, il tag di Google Analytics che stiamo configurando
> verrà attivato al caricamento di una qualsiasi pagina del nostro sito.

5.  Assegnare un nome al Tag (es. "**Configurazione GA4**") che stiamo
    creando e cliccare sul pulsante "**Salva**" presente nella parte
    alta della maschera per confermare la sua creazione

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ga4_13.bmp](./assets/media/image42.png){width="5.184722222222222in"
height="3.477777777777778in"}

6.  Verificare in modalità **Anteprima** il corretto funzionamento del
    Tag (per maggiori informazioni in merito si veda anche quanto
    indicato nel capitolo "*Google Tag Manager -- Implementazione e
    attivazione di Google Tag manager --* *Fase 3 -- Anteprima di
    pubblicazione del contenitore*")

> **ATTENZIONE!** Come già evidenziato a questo punto il Tag è stato
> creato ma fintanto che non verrà pubblicata la nuova versione del
> contenitore le modifiche effettuate non verranno riportate in
> produzione e sul sito non sarà quindi ancora attivo nessun tipo di
> tracciamento

7.  Cliccare sul pulsante "**Salva**" presente nella parte alta della
    maschera per creare e salvare il Tag appena configurato

![Videate\\gtm_35c.bmp](./assets/media/image43.png){width="5.592361111111111in"
height="3.254861111111111in"}

8.  Una volta verificato che tutto funzioni correttamente l'ultimo
    passaggio sarà ovviamente quello di pubblicare il Contenitore. In
    questo senso sarà quindi sufficiente cliccare sul pulsante
    "**Invia**" presente nella parte alta della maschera

![Videate\\gtm_35d.bmp](./assets/media/image44.png){width="5.592361111111111in"
height="3.1590277777777778in"}

> assegnare un nome e una descrizione alla versione del Tag che andremo
> a pubblicare e, infine, avviare la pubblicazione cliccando sul
> pulsante "**Pubblica**"

![Videate\\gtm_35e.bmp](./assets/media/image45.png){width="5.547916666666667in"
height="3.407638888888889in"}

> Da questo momento in avanti la nuova versione del Contenitore (con i
> relativi Tag) sarà effettivamente attiva sul sito e da questo momento
> in avanti dovrebbero quindi iniziare ad arrivare alla nostra proprietà
> di Universal Analytics i relativi dati di tracciamento

**ATTENZIONE! Questo tag consente di tracciare in Analytics solo ed
esclusivamente le informazioni di base secondo quella che è la specifica
configurazione attivata nella corrispondente proprietà GA4. In queste
condizioni non verrà ancora tracciato nessune evento ecommerce**

