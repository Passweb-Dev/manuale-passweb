# ECOMMERCE



Come già evidenziato nel precedente capitolo di questo manuale, la
sezione "**Ecommerce**" visibile all'interno della maschera "**Dati
Account**" solo dopo aver configurato e salvato i parametri di
Configurazione, permette di decidere quali dati Ecommerce dovranno
essere trasferiti dal proprio sito ad ActiveCampaign

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ac_7.bmp](./assets/media/image7.png){width="5.486805555555556in"
height="3.4479166666666665in"}

In questo senso dunque il parametro:

- **Abilita Ordini**: consente, se impostato sull'opzione **Si**, di
  abilitare l'invio ad ActiveCampaign degli ordini effettuati
  all'interno del proprio sito Ecommerce.

> Attivando questo parametro dunque, nel momento in cui un utente andrà
> ad effettuare un ordine all'interno del sito, questo verrà inviato
> immediatamente anche ad ActiveCampaign e sarà inserito nella sezione
> Ecommerce del relativo contatto

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ac_8.bmp](./assets/media/image8.png){width="5.519444444444445in"
height="3.4611111111111112in"}

> Oltre ai dati specifici dell'ordine (articoli, totale merce ...)
> verranno inviati ad Active anche i seguenti dati:

- **Nome** dell'utente di fatturazione

- **Cognome** dell'utente di fatturazione

- **Email** dell'utente di fatturazione

> In particolare l'Email dell'utente verrà utilizzata da ActiveCampaign
> come campo chiave quindi nel momento in cui dovesse già essere
> presente sulla piattaforma un utente con quella stessa Email verrà
> agganciata la relativa anagrafica contatto e verranno aggiornati i
> suoi dati.
>
> Nel caso in cui non dovesse invece essere presente nessun utente con
> quell'indirizzo mail, verrà creata una nuova anagrafica utilizzando i
> dati inviati.

- **Abilita Carrelli Abbandonati**: consente, se selezionato, di
  abilitare l'invio a MailChimp dei dati relativi ai Carrelli
  Abbandonati.

> **ATTENZIONE!** verranno inviati ad ActiveCampaign i soli Carrelli
> abbondonati associati ad utenti registrati e dotati quindi di uno
> specifico indirizzo mail.
>
> **ATTENZIONE!** A differenza di quello che avviene per gli ordini **i
> carrelli abbandonati verranno inviati ad ActiveCampaign non all'atto
> della loro creazione ma al termine di ogni sincronizzazione Sito --
> Gestionale (Totale o per Variati).**
>
> Anche in questo caso:

- oltre ai dati dello specifico carrello abbandonato verrà inviato ad
  Active anche il **Nome**, il **Cognome** e **l'indirizzo Email**
  dell'utente che ha generato il carrello in questione.

- l'indirizzo mail verrà utilizzato come campo chiave per agganciare
  eventuali anagrafiche contatto già presenti sulla piattaforma

- nel caso in cui non dovesse essere presente nessuna anagrafica con
  l'indirizzo mail inviato, verrà creato un nuovo contatto

> Inoltre tra le informazioni inviate ad ActiveCampaign relativamente ai
> Carrelli Abbandonati sarà presente anche uno specifico url di recupero
> del Carrello.
>
> Cliccando su questo link, da inserire, ovviamente nelle relative mail
> di recupero, l'utente verrà quindi ricondotto al sito Passweb dove
> troverà il proprio carrello compilato in maniera completamente
> automatica con gli articoli precedentemente presenti all'interno del
> Carrello Abbandonato.
>
> In questo senso occorre ricordare anche che nel momento in cui il
> parametro " **Gestione Carrello al Login"** presente alla pagina
> "**Configurazione Catalogo**" del Wizard (sezione "**Gestione
> Carrello**") dovesse essere impostato sull'opzione **"Gestione
> Unificata" eventuali mail di recupero dei carrelli abbandonati
> (contenenti link per il recupero di un determinato carrello) non
> avrebbero molto senso.** Con la gestione unificata infatti l'ultimo
> carrello abbandonato da un determinato utente diventerà
> automaticamente il carrello attivo nel momento in cui l'utente stesso
> dovesse effettuare nuovamente l'accesso al sito.
>
> In queste condizioni dunque eventuali mail contenenti link di recupero
> di vecchi carrelli abbandonati porteranno l'utente sempre e comunque
> al carrello attivo in quel preciso momento, carrello questo che
> potrebbe anche contenere articoli diversi da quelli presenti nel
> momento in cui il vecchio carrello abbandonato era stato generato
>
> Per maggiori informazioni relativamente al parametro "Gestione
> Carrello al Login" si veda quanto indicato nel relativo capitolo di
> questo manuale ("*Catalogo -- Configurazione Parametri Catalogo --
> Catalogo Mexal / Ho.Re.Ca -- Gestione Carrello*")

In generale per quel che riguarda la creazione o meno di nuovi contatti
all'interno della piattaforma di ActiveCampaign a seguito della
creazione di un ordine o di un carrello abbandonato, è bene sottolineare
che **il campo che verrà utilizzato come chiave per determinare se
l'utente Passweb (che ha effettuato l'ordine o che ha prodotto il
carrello abbandonato) è già presente o meno su ActiveCampaign sarà,
ovviamente, l'indirizzo Email**.

In considerazione di ciò:

- Nel caso in cui l'indirizzo mail dell'utente Passweb, dovesse
  corrispondere a quello di uno dei contatti già presenti in
  ActiveCampaign, verrà agganciata la relativa anagrafica, verranno
  aggiornate le suoi informazioni e verranno aggiunti i dati Ecommerce
  relativi all'ordine appena effettuato o al carrello abbandonato da
  esso generato.

> **ATTENZIONE!** In questo caso potrebbero essere aggiornati nome e
> cognome dell'utente con i relativi dati presenti nell'ordine o nel
> carrello abbandonato inviato ad ActiveCampaign. **In ogni caso,
> l'appartenenza dell'utente ad eventuali liste definite su
> ActiveCampaign o le sue preferenze relative al fatto di aver accettato
> o meno di ricevere comunicazioni di carattere commerciale non saranno
> in alcun modo variate.**

- Nel caso in cui l'indirizzo mail dell'utente che ha effettuato
  l'ordine o che ha prodotto il carrello abbandonato non dovesse
  coincidere con nessuno dei contatti presenti su ActiveCampaign, verrà
  creata una nuova anagrafica con il Nome, il Cognome e la mail
  dell'utente Passweb. A questa nuova anagrafica verrà aggiunto
  automaticamente il tag "**Passweb Integration -- customer**" e
  verranno inserite ovviamente anche tutte le relative informazioni
  Ecommerce.

> In questo caso inoltre, **il nuovo contatto non verrà associato a
> nessuna delle Liste presenti su ActiveCampaign così come non verranno
> settate in alcun modo eventuali preferenze relative alla possibilità
> da parte sua di ricevere o meno comunicazioni di carattere
> commerciale.**
>
> Starà quindi a chi gestisce la piattaforma terza accertarsi del fatto
> che tale utente non venga poi coinvolto nell'invio di eventuali
> campagne di mail marketing.

**ATTENZIONE!** lato ecommerce l'integrazione tra Passweb ed
ActiveCampaign si limita ad inserire sulla piattaforma terza
informazioni relative ad ordini e carrelli abbandonati generati
all'interno del sito Ecommerce. **Eventuali automazioni a seguito delle
quali potranno o meno essere inviate determinate mail, l'invio di queste
stesse mail, così come eventuali segmentazioni o controlli relativi al
fatto che un utente possa o meno ricevere determinate tipologie di mail,
sono tutte cose che dovranno essere implementati e gestite direttamente
su ActiveCampaign**.

Per la stessa ragione nel momento in cui si dovessero verificare
problemi di qualsiasi tipo inerenti all'invio o alla ricezione di queste
mail sarà necessario rivolgersi direttamente all'assistenza di
ActiveCampaign.

