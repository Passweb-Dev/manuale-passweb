# TASSE



La sezione "**Tasse**", accessibile dalla voce di menu principale
"**Ordini**" consente all'amministratore del sito di:

- definire e gestire eventuali tasse addizionali (es. CONAI, RAEE
  ecc...) che dovranno poi essere applicate agli ordini effettuati
  all'interno del sito.

- gestire una specifica aliquota / esenzione IVA in relazione ad ogni
  singolo paese (diverso dall'Italia) in cui dovrà poi essere spedita la
  merce acquistata in maniera tale da soddisfare le normative vigenti in
  materia di **OSS (One Stop Shop)**, di **Cessioni intracomunitarie** e
  di **Esportazioni verso paesi extra UE** (per maggiori informazioni in
  merito si vedano anche i successivi capitoli di questo manuale).

Portandosi dunque all'interno di questa sezione verrà visualizzata la
maschera "**Tasse**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\lista_tasse.bmp](./assets/media/image436.png){width="5.811805555555556in"
height="3.532638888888889in"}

contenente l'elenco di tutte le tasse addizionali attualmente codificate
e gestite all'interno del sito.

Il campo di ricerca attivabile cliccando sulla lente di ingrandimento,
presente in testata di ogni singola colonna, consente di filtrare i dati
in griglia sulla base dei valori presenti all'interno della colonna
stessa.

Una volta impostato un filtro di ricerca, per poterlo poi eliminare sarà
sufficiente cliccare sull'icona raffigurante una piccola lente di
ingrandimento con un -- all'interno (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_elimina_filtro.bmp](./assets/media/image2.png){width="7.777777777777778e-2in"
height="9.722222222222222e-2in"} ) che comparirà in testata alla colonna
in corrispondenza della quale è stato impostato il filtro stesso.

Infine è anche possibile ordinare, in maniera crescente e/o decrescente,
gli elementi in griglia cliccando semplicemente sull'icona raffigurante
due piccole frecce posta anch' essa in testata ad ogni singola colonna
della griglia (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\icona_ordinamento_griglia.bmp](./assets/media/image3.png){width="0.12361111111111112in"
height="0.14930555555555555in"} )

I pulsanti presenti nella barra degli strumenti consentono
rispettivamente di:

**Attiva** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_attiva_tassa.bmp](./assets/media/image437.png){width="0.4548611111111111in"
height="0.175in"} ) **\\ Disattiva**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_disattiva_tassa.bmp](./assets/media/image438.png){width="0.5583333333333333in"
height="0.18194444444444444in"} ) **Tassa**: consente di
attivare\\disattivare la tassa addizionale attualmente selezionata in
elenco. Ovviamente potranno essere effettivamente applicate ai vari
ordini effettuati all'interno del sito, solo ed esclusivamente le tasse
addizionali opportunamente abilitate.

**ATTENZIONE!** per ottimizzare le prestazioni del sito i dati relativi
ad eventuali tasse addizionali sono gestiti a livello di sessione del
browser. In conseguenza di ciò eventuali variazioni apportate a livello
di attivazione / disattivazione di una determinata tassa possono
richiedere, prima di essere effettivamente visualizzate sul front end
del sito, la pulizia della cache del browser (compresi i cookie) oppure
l'apertura automatica (a seguito di un determinato periodo di
inattività) di una nuova sessione.

**Elimina Tassa**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_elimina_tassa.bmp](./assets/media/image439.png){width="0.48680555555555555in"
height="0.18194444444444444in"} ): consente di eliminare la tassa
addizionale attualmente selezionata in elenco

**Modifica Tassa**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_modifica_tassa.bmp](./assets/media/image440.png){width="0.5451388888888888in"
height="0.18194444444444444in"} ): consente di modificare i parametri di
configurazione della tassa addizionale attualmente selezionata in elenco

**Copia Tassa**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_copia_tassa.bmp](./assets/media/image441.png){width="0.44166666666666665in"
height="0.1625in"} ): consente di duplicare la tassa addizionale
attualmente selezionata in elenco.

**Aggiungi Tassa**
(![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_aggiungi_tassa.bmp](./assets/media/image442.png){width="0.5909722222222222in"
height="0.175in"} ): consente di definire una nuova tassa addizionale.
Cliccando su questo pulsante verrà quindi visualizzata la maschera
**"Nuova Tassa"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\nuova_tassa.bmp](./assets/media/image443.png){width="5.565277777777778in"
height="3.265972222222222in"}

all'interno della quale poter definire le caratteristiche della tassa
che si intende codificare.

Nello specifico il parametro:

- **Stato della Tassa:** consente di abilitare/disabilitare la tassa in
  esame rendendola quindi effettivamente utilizzabile o meno all'interno
  del sito (allo stesso modo di quanto avviene con i pulsante "**Attiva
  Tassa**" e "**Disattiva Tassa**" precedentemente esaminati).

- **Descrizione:** consente di definire, in tutte le lingue attualmente
  gestite, l'etichetta identificativa della tassa addizionale che si sta
  codificando. Tale etichetta verrà poi utilizzata e visualizzata
  all'interno del relativo componente "**Tasse**" come label relativa
  all'importo della tassa stessa

- **Tipologia Tassa:** consente di definire la tipologia di Tassa che si
  intende codificare. E' possibile indicare uno dei seguenti valori:

  - **Tassa Extra**: selezionando questa opzione sarà poi possibile
    definire e gestire una Tassa addizionale, diversa dall'Iva, da
    applicare ai singoli articoli in ordine (es. CONAI, RAEE ecc...)

  - **Iva**: selezionando questa opzione sarà poi possibile gestire, per
    gli utenti Privati e per le Aziende iscritte o non iscritte al VIES
    un'aliquota iva e/o un' esenzione IVA diversa in relazione allo
    specifico paese in cui dovrà poi essere spedita la merce.

> Questa particolare tipologia di Tassa permetterà quindi di soddisfare
> le normative di legge in materia di OSS (One Stop Shop) e/o Cessioni
> intra o extra comunitarie. Per maggiori informazioni in merito si
> rimanda a quanto indicato nei successivi capitoli di questo manuale

**ATTENZIONE!** I successivi parametri di configurazione presenti
all'interno di questa maschera variano in relazione all'opzione
selezionata per il campo "Tipologia Tassa" e quindi in base alla
specifica tipologia di Tassa che si andrà a gestire.

Per maggiori informazioni in merito ai parametri di configurazione delle
due diverse tipologie di Tasse gestibili in Passweb si vedano i
successivi capitoli di questo manuale

