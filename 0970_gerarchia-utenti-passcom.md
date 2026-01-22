# GERARCHIA UTENTI PASSCOM



Nel caso in cui il sito sia collegato ad un'installazione Passcom (sia
essa presso la Web Farm di Passepartout, sia essa in locale presso il
cliente) è possibile creare un'intera gerarchia utenti in maniera
completamente automatica importandola direttamente dal gestionale.

Per poter far ciò occorre selezionare il parametro **"Crea gerarchia
Utenti del gestionale"** presente alla pagina Parametri
**Configurazione** dal menù del Wizard **"Configurazione"**

![](./assets/media/image265.png)

**NOTA BENE:** la maschera sopra evidenziata è visibile unicamente nel
caso in cui il sito sia collegato ad un'installazione Passcom.

Selezionando tale parametro verrà creata, alla successiva
sincronizzazione, la gerarchia automatica di Passweb per gli Utenti
Passcom prelevando tutto ciò che serve per realizzare tale gerarchia
(gruppi, utenti, legami "gruppo padre -- gruppo figlio" ecc ...)
direttamente dal gestionale.

**NOTA BENE:** la gerarchia automatica di Passweb per gli Utenti Passcom
è determinata unicamente dalle impostazioni del gestionale.

Scegliendo quindi di far generare in automatico all'applicazione questa
gerarchia per gli Utenti Passcom, Passweb si preoccuperà di prelevare
direttamente dal gestionale gli utenti abilitati ad accedere all'Area
Riservata del sito web, di creare appositi gruppi all'interno dei quali
andare a collocare, secondo specifiche regole di appartenenza, i vari
utenti e di stabilire i legami padre -- figlio tra ognuno di questi
gruppi.

I gruppi presenti all'interno di questa gerarchia e creati in automatico
da Passweb, sono quelli qui di seguito riportati:

- **Dottore Commercialista:** è il gruppo che racchiude al suo interno
  tutti gli Utenti Passcom di tipo COMMERCIALISTA, dunque, l'insieme di
  tutti gli utenti facenti parte di quel particolare gruppo definito
  all'interno di Passcom e con nome uguale a quello specificato nel
  campo **"Gruppo del gestionale dei Commercialisti"** presente nella
  pagina "Configurazione -- Parametri Configurazione" del Wizard (vedi
  anche sezione "Gerarchia Utenti" di questo manuale).

**NOTA BENE:** non è possibile eliminare dai gruppi sopra indicati gli
Utenti Passcom inseriti in automatico da Passweb e che verificano quindi
le relative regole di appartenenza.

**NOTA BENE:** i gruppi **Dottore Commercialista** e **Dipendenti**
nascono a default con i parametri "Comunicazione interna" e "Gestione
SMS" selezionati e conseguentemente con le relative funzionalità
abilitate.

- **Aziende Gestite:** è il gruppo che racchiude al suo interno tutti
  gli Utenti Passcom del sito di tipo AZIENDA, dunque, tutte le aziende
  dell'installazione il cui parametro **"Stato"** della maschera "*Dati
  Aziendali (F4 da "Anagrafica Azienda") -- Configurazione Moduli --
  Collegamento Sito Commercialista*" è stato impostato ad A (vedi anche
  sezione "Tipologia Utente" di questo manuale).

- **Aziende Liquidazione Mensile/Trimestrale:** è il gruppo che
  racchiude al suo interno tutti gli Utenti Passcom del sito di tipo
  AZIENDA, dunque, tutte le aziende dell'installazione il cui parametro
  **"Stato"** della maschera "*Dati Aziendali (F4 da "Anagrafica
  Azienda") -- Configurazione Moduli -- Collegamento Sito
  Commercialista*" è stato impostato ad A, e che hanno una gestione
  della liquidazione IVA Mensile/Trimestrale. Tale gestione deve essere
  attivata attraverso lo specifico parametro contabile all'interno del
  gestionale.

**NOTA BENE:** nel caso in cui all'interno del gestionale non siano
state definite aziende a liquidazione Mensile/Trimestrale all'interno
del sito non sarà creato il relativo gruppo.

- **Dipendenti:** è il gruppo che racchiude al suo interno tutti gli
  Utenti Passcom del sito di tipo DIPENDENTE, dunque, l'insieme di tutti
  gli utenti facenti parte di un qualsiasi gruppo utenti definito in
  Passcom e con nome diverso da quello specificato nel campo **"Gruppo
  del Gestionale dei Commercialisti"** presente nella pagina
  "Configurazione -- Parametri Configurazione" del Wizard.

Nel caso in cui il parametro **"Crea gerarchia Utenti Passcom"** non
venga selezionato, alla sincronizzazione, non verranno creati né i
gruppi automatici sopra evidenziati né tanto meno la relativa gerarchia
per gli Utenti Passcom. Verranno comunque importati gli Utenti Passcom
che, in questo caso però, non verranno ovviamente collocati in
automatico all'interno di nessuna gerarchia. In tal caso dunque sarà
necessario andare poi a collocare manualmente ogni singolo Utente
Passcom all'interno di una specifica gerarchia precedentemente creata.

**NOTA BENE:** è possibile inserire utenti Passcom in una qualsiasi
gerarchia diversa da quella generata in automatico da Passweb. Allo
stesso modo è perfettamente possibile inserire Utenti NON Passcom in uno
qualsiasi dei gruppi generati in automatico da Passweb e facenti parte
quindi della relativa gerarchia.

