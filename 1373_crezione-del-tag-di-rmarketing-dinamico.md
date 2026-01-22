# CREZIONE DEL TAG DI RMARKETING DINAMICO



1.  Accedere al proprio Account di Google Tag Manager, portarsi nella
    dashboard di gestione del Contenitore su cui si desidera operare e
    cliccare sul pulsante "**Aggiungi un uovo Tag**"

![Videate\\gtm_15b.bmp](./assets/media/image36.png){width="5.586111111111111in"
height="3.4458333333333333in"}

2.  Cliccare sul pulsante "**Scegli un tipo di tag per iniziare
    l'installazione**" presente all'interno del box "**Configurazione
    Tag**"

![Videate\\gtm_ecommerce_avanzato_10.bmp](./assets/media/image37.png){width="5.33125in"
height="3.3569444444444443in"}

3.  Selezionare tra quelli proposti il tag "**Google Ads**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_remarketing_dinamico_3.bmp](./assets/media/image220.png){width="5.375694444444444in"
height="3.325in"}

> e tra le successive tipologie di Tag per Google Ads selezionare
> l'opzione "**Google Ads Remarketing**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_remarketing_dinamico_4.bmp](./assets/media/image221.png){width="5.375694444444444in"
height="3.325in"}

4.  Nella successiva maschera di configurazione del tag impostare i
    parametri richiesti come di seguito indicato

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_remarketing_dinamico_5.bmp](./assets/media/image222.png){width="5.375694444444444in"
height="3.325in"}

- **Conversion ID**: utilizzare il proprio ID Conversione di Google Ads

- **Send dynamic remarketing event data**: selezionato

- **Event Name**: {{Event}} -- variabile standard che verrà poi
  sostituita con il nome dell'evento che ha fatto scattare il Tag

- **Event Value:** {{GADS -- DLV remarketing_ads.value}} -- variabile di
  livello dati precedentemente creata

- **Event Items:** {{GADS -- DLV remarketing_ads.items}} -- variabile di
  livello dati precedentemente creata

5.  Una volta completata la configurazione del Tag dovremo ora andare ad
    impostare l'Attivatore mediante il quale decidere quando e come
    questo stesso Tag dovrà essere effettivamente attivato.

> Cliccare quindi sul pulsante "**Scegli un attivatore per attivare
> questo tag**" presente all'interno del box "**Attivazione**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_remarketing_dinamico_6.bmp](./assets/media/image223.png){width="5.375694444444444in"
height="3.325in"}

> e, successivamente, cliccare sul pulsante di creazione di un nuovo
> attivatore (il piccolo + posto nella parte alta della maschera)

![Videate\\gtm_ecommerce_avanzato_19.bmp](./assets/media/image60.png){width="5.33125in"
height="3.3569444444444443in"}

6.  Nella maschera di creazione del nuovo Attivatore cliccare su
    "**Scegli un tipo di trigger per iniziare l'installazione**"
    presente all'interno del box "**Configurazione attivatore**"

![Videate\\gtm_ecommerce_avanzato_20.bmp](./assets/media/image61.png){width="5.33125in"
height="3.3569444444444443in"}

> e selezionare, tra le opzioni proposte, "**Evento Personalizzato**"

![Videate\\gtm_ecommerce_avanzato_21.bmp](./assets/media/image62.png){width="5.33125in"
height="3.3569444444444443in"}

7.  Nella successiva maschera impostare i parametri di configurazione
    dell'attivatore come nella figura di seguito riportata

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_remarketing_dinamico_7.bmp](./assets/media/image224.png){width="5.375694444444444in"
height="3.325in"}

- **Nome Evento**: impostare su
  "***view_item_list\$\|view_item\$\|add_to_cart\$\|purchase\$***"

- **Utilizza Espressione Regolare**: selezionato

- **Questo attivatore si attiva su**: impostare sul "**Tutti gli eventi
  personalizzati**"

> L'utilizzo dell'espressione regolare consente di gestire un solo
> attivatore per tutti gli eventi di Remarketing Dinamico che dovranno
> effettivamente essere gestiti.
>
> Con la configurazione in oggetto dunque il Tag di Remarketing Dinamico
> verrà attivato in corrispondenza degli eventi di:

- view_item_list

- view_item

- add_to_cart

- purchase

8.  Assegnare un nome all'Attivatore (es. "**GADS - Remarketing
    Events**") e cliccare sul pulsante **Salva**

> **ATTENZIONE!** Volendo avremmo anche potuto creare preventivamente
> questo tipo di attivatore operando all'interno dell'apposita sezione
> di GTM per poi selezionarlo tra quelli proposti all'interno della
> maschera "Scegli un attivatore"

9.  Una volta completata anche la configurazione dell'Attivatore
    assegnare un nome al Tag che stiamo creando (es. **GADS --
    Remarketing Dinamico**) operando dall'apposito campo presente nella
    parte alta della maschera e, infine, salvare il Tag cliccando sul
    pulsante "**Salva**"

10. Verificare in modalità **Anteprima** il corretto funzionamento del
    Tag

11. Pubblicare il nuovo Tag e le modifiche apportate al Contenitore
