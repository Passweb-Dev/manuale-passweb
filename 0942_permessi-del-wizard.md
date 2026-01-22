# PERMESSI DEL WIZARD



La sezione "Permessi del Wizard", accessibile cliccando sul pulsante
"**Modifica Permessi**" della maschera "**Gestione Ruoli**"
precedentemente analizzata, consente di impostare le azioni che tutti
gli utenti appartenenti al Ruolo in esame potranno o non potranno
effettuare all'interno del Wizard.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\utentipassweb_modifica_ruolo.bmp](./assets/media/image13.png)

Per definire quindi uno specifico schema di permessi è sufficiente
selezionare/deselezionare all'interno della griglia sopra evidenziata la
funzionalità che si intende abilitare/disabilitare e successivamente
cliccare sul pulsante **"Salva"** presente nella parte bassa della
maschera.

Per ogni elemento presente in griglia (righe della tabella) è possibile
abilitare/disabilitare determinate funzionalità (colonne della tabella)
che possono variare in relazione alla specifica tipologia di elemento.

Ad esempio per quel che riguarda le funzionalità dell'applicazione
(Gestione dell'Account di Posta, Gestione Risorse ecc ..), è possibile
definire unicamente se la specifica funzionalità dovrà o meno essere
abilitata, mentre per quel che riguarda le classi di componenti, oltre a
definire se la tipologia di ruolo che si sta considerando possa essere
abilitata o meno a gestire la specifica classe, è possibile indicare
anche che tipo di azione potrà essere effettuata su quella classe
(Creazione, Modifica, Editing Grafico, Copia ecc ... ).

Ciascuna delle colonne presenti nella griglia consente quindi di
abilitare o disabilitare sui singoli elementi presenti in riga una certa
azione. In particolare:

- **Accesso:** consente di abilitare/disabilitare la gestione del
  corrispondente elemento di riga (funzionalità o classe di componente);

> **ATTENZIONE!** Nel caso in cui il flag Accesso non sia selezionato
> verrà disabilitata la gestione del relativo elemento (funzionalità o
> classe di componente) per cui eventuali altre azioni abilitate per lo
> stesso elemento non avranno alcun effetto.

- **Creazione:** consente di abilitare/disabilitare la possibilità di
  creare nuovi elementi (pagine o componenti);

- **Modifica:** consente di abilitare/disabilitare la possibilità di
  modificare i contenuti del relativo elemento di riga;

- **Eliminazione:** consente di abilitare/disabilitare la possibilità di
  eliminare il relativo elemento di riga;

- **Editing grafico:** consente di abilitare/disabilitare la possibilità
  di accedere alle proprietà grafiche del relativo elemento di riga;

- **Spostamento:** consente di abilitare/disabilitare la possibilità di
  spostare all'interno delle pagine il relativo elemento di riga;

- **Configurazione e Distribuzione:** consente di abilitare/disabilitare
  la possibilità di accedere alle proprietà del relativo elemento di
  riga per distribuire i componenti sulle pagine;

- **Copia e Scollega:** consente di abilitare/disabilitare la
  possibilità di effettuare la copia del relativo elemento di riga e di
  scollegarli dagli elementi ripetuti;

**NOTA BENE:** relativamente ai componenti presenti nella libreria di
Passweb, la griglia di permessi sopra evidenziata consente di definire
le azioni che possono essere abilitate/disabilitate a livello di classi
di componente. Per poter poi stabilire quale singolo componente possa o
meno essere gestito da una certa tipologia di utenza, occorre
necessariamente agire, in Live Editing, dalle proprietà di
configurazione dello specifico componente (vedi anche pagina "Modifica
Componenti - Proprietà" di questo manuale).

> I due pulsanti "**Seleziona Tutto**" e "**Deseleziona Tutto**"
> presenti nella parte alta della maschera consentono rispettivamente di
> selezionare e deselezionare in un colpo solo tutti i check presenti
> all'interno della maschera.
>
> Infine, l'icona raffigurante un piccolo check blu posta in
> corrispondenza di ogni colonna della voce "**LE -- Gestione
> Componenti**" consente di selezionare/deselezionare in un colpo solo
> tutti i check della relativa colonna, mantenendo, inoltre, lo schema
> di campi selezionati per la colonna "**Accesso**"

