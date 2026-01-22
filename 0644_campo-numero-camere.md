# CAMPO NUMERO CAMERE



Consente all'utente che compila il form di indicare il numero di camere
che dovranno eventualmente essere prenotate

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\form_welcome_campo_numero_camere.bmp](./assets/media/image32.png)

**Tipologia di componente Passweb**: Campo Lista Valori

**PARAMETRI DI CONFIGURAZIONE DEL COMPONENTE**

**Id/Name** = numeroCamere

**Obbligatorio** = Si

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\form_welcome_campo_numero_camere_configurazione.bmp](./assets/media/image33.png)

I valori presenti all'interno della select dovranno essere coerenti,
ovviamente, con il numero di camere per cui è possibile chiedere
informazioni.

Supponendo dunque che il numero di camere prenotabili possa variare da 1
a 3, in fase di configurazione del componente, i valori da inserire
all'interno della sezione "**Gestione Valori**" dovranno essere 1,2 e 3

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\form_welcome_campo_numero_camere_configurazione_2.bmp](./assets/media/image34.png)

**ATTENZIONE!** per ogni camera gestita, andranno poi inseriti
all'interno del form altri campi necessari per consentire all'utente di
indicare:

- Il numero di adulti

- Il numero di bambini

- L'età di ciascun bambino

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\form_welcome_campo_numero_camere_2.bmp](./assets/media/image35.png)

Inoltre per fare in modo che i campi visualizzati all'interno del form
siano effettivamente coerenti con il numero di camere indicate
dall'utente, questi campi aggiuntivi dovranno essere configurati con
determinate condizioni di visibilità e di obbligatorietà (per maggiori
informazioni in merito si vedano anche i successi capitoli di questo
manuale)

I dati relativi al numero di camere, al numero di adulti, di bambini e
all'età di ciascun bambino verranno poi inseriti nel relativo campo
(**Camere**) presente nel dettaglio della richiesta inserita all'interno
del gestionale

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\form_welcome_campo_camere_3.bmp](./assets/media/image36.png)

