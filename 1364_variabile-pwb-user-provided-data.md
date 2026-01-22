# VARIABILE "PWB -- USER PROVIDED DATA"



**Tipologia della variabile**: variabile di tipo User Provided Data

**Nome della variabile**: PWB -- User Provided Data

I dati utente catturati dal dataLayer di Passweb e disponibili in Tag
Manager grazie alle variabili di livello dati indicate nei precedenti
capitoli di questo manuale, a differenza di quanto avveniva per i dati
ecommerce, non possono essere passati a Google Analytics o a Google Ads
direttamente come parametri dei vari eventi.

In questo caso infatti dovrà essere creata una nuova tipologia di
variabile che raccoglie in sé tutti questi dati e che sarà poi quella
che dovrà essere effettivamente utilizzata in fase di configurazione dei
vari Tag di tracciamento per fare in modo che questi stessi Tag possano
inviare a Google Ads piuttosto che a Google Analytics oltre ai dati per
cui sono stati creati anche i dati utente raccolti all'interno di questa
nuova tipologia di variabile.

Di seguito viene quindi indicata la procedura da seguire per creare
questa nuova variabile:

Di seguito viene indicato il procedimento da seguire per poter creare la
variabile in questione:

1.  Accedere al pannello di amministrazione del proprio account GTM,
    sezione "**Variabili**" (menu di sinistra), e creare una nuova
    variabile cliccando sul pulsante "**Nuova**" presente in
    corrispondenza del box "**Variabili definite dall'utente**"

![Videate\\gtm_ecommerce_avanzato_1.bmp](./assets/media/image49.png)

2.  Cliccare sul pulsante "**Scegli un tipo di variabile per iniziare
    l'installazione**" presente in corrispondenza del box
    "**Configurazione Variabile**"

![Videate\\gtm_ecommerce_avanzato_2.bmp](./assets/media/image50.png)

> e selezionare, tra le varie proposte, l'opzione "**User-Provided
> Data**" (o "Dati Forniti dagli Utenti" a seconda della lingua
> impostata all'interno del proprio browser)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_var_user_provided_data.bmp](./assets/media/image202.png)

3.  Nella successiva maschera impostare i campi di configurazione della
    variabile come di seguito indicato

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gtm_var_user_provided_data_2.bmp](./assets/media/image203.png)

- **Type**: Manual Configuration

- **Email**: impostare sulla variabile {{UPD -- DLV
  user_data.sha256_email_address}}

- **Phone**: impostare sulla variabile {{UPD -- DLV
  user_data.sha256_phone_number}}

- **First Name**: impostare sulla variabile {{UPD -- DLV
  user_data.address.sha256_first_name}}

- **Last Name**: impostare sulla variabile {{UPD -- DLV
  user_data.address.sha256_last_name}}

- **Street**: impostare sulla variabile {{UPD -- DLV
  user_data.address.street}}

- **City**: impostare sulla variabile {{UPD -- DLV
  user_data.address.city}}

- **Region**: lasciare impostato sull'opzione "Not set"

- **Country**: impostare sulla variabile {{UPD -- DLV
  user_data.address.country}}

- **Postal Code**: impostare sulla variabile {{UPD -- DLV
  user_data.address.postal_code}}

