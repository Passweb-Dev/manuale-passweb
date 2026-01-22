# CREAZIONE LEAD SU PUFFIN CRM



Come indicato all'interno dei precedenti capitoli di questo manuale, il
componente Form di Passweb può essere utilizzato anche per creare
anagrafiche di nuovi Lead che verranno poi memorizzate all'interno di
Puffin CRM.

Per far questo è necessario innanzitutto:

1.  Aver attivato correttamente l'integrazione tra Passweb e Puffin
    operando in questo senso all'interno della sezione "**Puffin CRM**"
    alla pagina "**Sito -- Preferenze**" del Wizard (tab
    "**Integrazioni**")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\puffin_crm_configurazione_2.bmp](./assets/media/image154.png)

> Per maggiori informazioni relativamente a come poter attivare questa
> integrazione si veda anche quanto indicato all'interno del capitolo
> "*Sito -- Preferenze -- Integrazioni -- Puffin CRM*" di questo manuale

2.  Aver abilitato il componente From al salvataggio dei dati
    all'interno di Puffin attivando, in questo senso, il parametro
    "**Crea Contatto in Puffin CRM**" presente nella maschera di
    configurazione del componente stesso

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\crea_anagrafica_puffin.bmp](./assets/media/image155.png)

Una volta verificate le due condizioni sopra indicate, inserendo poi
all'interno del Form uno dei seguenti componenti:

- **Campo di Testo**

- **Campo Radio**

- **Campo Lista di Checkbox**

- **Campo Lista Valori**

- **Campo Data**

- **Campo Area di Testo**

nella loro maschera di configurazione comparirà anche il parametro
"**Campo Puffin CRM**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\campo_puffin_crm.bmp](./assets/media/image156.png)

che consentirà di indicare, selezionandolo dal relativo menu a tendina,
lo specifico campo dell'anagrafica Lead di Puffin in cui dovrà essere
salvato il dato inserito dall'utente in fase di compilazione del From
sul sito Passweb.

Sono gestiti i seguenti campi dell'Anagrafica Lead di Puffin:

- **Alias azienda (utilizzato in fase di ricerca) -- SI**

- **Cap**

- **Cellulare**

- **Città**

- **Codice Ateco**

- **Codice fiscale**

- **Codice IBAN**

- **Codice SDI**

- **Cognome in caso di privato**

- **Email**

- **Email pec**

- **Fax**

- **Gestione persona fisica**

- **Gestione privato**

- **Identificativo Paese**

- **Identificativo provenienza**

- **Identificativo residenza fiscale**

- **Indirizzo**

- **Nome e cognome referente azienda**

- **Nome in caso di privato**

- **Nota di fine rapporto**

- **Note singole**

- **Numero dipendenti**

- **piva**

- **Prefisso internazionale cellulare**

- **Provincia**

- **Ragione sociale**

- **Sito web**

- **Telefono principale**

- **Telefono secondario**

- **Tipo azienda (azienda o privato)**

- **Valore del fatturato**

Oltre ai campi standard sopra evidenziati, potranno essere utilizzati
anche i Campi Custom appartenenti, in Puffin, a determinate "Strutture
di Campi Custom", strutture queste che, sempre all'interno di Puffin,
dovranno essere assegnate anche a specifici Utenti.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\puffin_campi_custom_6.bmp](./assets/media/image157.png)

Tali campi, come evidenziato in figura, saranno raggruppati nella select
presente in corrispondenza del parametro "Campo Puffin CRM" all'interno
di una determinata sezione la cui intestazione corrisponde con il nome
assegnato in Puffin alla loro struttura di appartenenza

**ATTENZIONE!** per maggiori informazioni in merito a come poter
abilitare i campi custom di Puffin si veda quanto indicato all'interno
del capitolo "*Sito -- Preferenze -- Integrazioni -- Puffin CRM -- Campi
Custom*" di questo manuale

Selezionando uno dei campi presenti nel menu a tendina verrà
visualizzata, immediatamente al di sotto del campo stesso, una piccola
legenda utile a comprendere la tipologia del campo Puffin selezionato e
quelle che dovranno quindi essere le impostazioni e le eventuali
limitazioni da settare, di conseguenza, sul campo Passweb per evitare
poi possibili errori in fase di salvataggio del form

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\legenda_campo_puffin_crm.bmp](./assets/media/image158.png)

Il campo "Email" evidenziato in figura, ad esempio, lato Puffin è un
campo di tipo stringa (**Tipo di Campo: stringa**) che ha abilitato un
controllo relativo al fatto che la stringa inserita rappresenti un
indirizzo mail (**Regole: email**) e tale campo verrà considerato come
obbligatorio, da Puffin, per la corretta creazione del Lead se il campo
Cellulare dovesse essere vuoto o, ovviamente, non gestito all'interno
del form (**Richiesto se cell = ''**)

In conseguenza di ciò, per evitare errori in fase di salvataggio dei
dati (e quindi in fase di conferma del form sul sito), il Campo Testo di
Passweb dovrà essere configurato impostando il parametro "**Tipo Valore
= Mail**" e il parametro "**Campo Obbligatorio**" su "**Si**" con
l'eventuale condizione di obbligatorietà legata al fatto che il campo
"Cellulare" presente nel form (e ovviamente mappato con il
corrispondente campo Puffin) sia uguale a stringa vuota

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\legenda_campo_puffin_crm_2.bmp](./assets/media/image159.png)

In questo modo, come è semplice comprendere, i controlli richiesti da
Puffin verranno applicati a monte da Passweb per cui, se soddisfatti, il
valore inserito dall'utente in fase di compilazione del form sarà già
corretto e non si avranno poi problemi, al salvataggio, in fase di
inserimento dell'anagrafica su Puffin.

Altre possibili configurazioni richieste dai campi Puffin potrebbero
essere del tipo di quelle riportate in tabella

+------------------------+------------------------+--------------------+
| **CONDIZIONI PUFFIN**  | **CONDIZIONI CAMPO     | **VALORI ACCETTATI |
|                        | PASSWEB**              | IN FASE DI         |
|                        |                        | COMPILAZIONE DEL   |
|                        |                        | FORM**             |
+========================+========================+====================+
| **Tipo di Campo**:     | **Componente da        | Qualsiasi stringa  |
| stringa                | utilizzare**: Campo di | alfanumerica       |
|                        | Testo                  |                    |
| **Regole**: text       |                        |                    |
|                        | **Tipo Valore** =      |                    |
|                        | Testo                  |                    |
+------------------------+------------------------+--------------------+
| **Tipo di Campo**:     | **Componente da        | Qualsiasi stringa  |
| stringa                | utilizzare**: Campo di | alfanumerica       |
|                        | Testo                  |                    |
| **Regole**: text -     |                        |                    |
| richiesto              | **Tipo Valore** =      |                    |
|                        | Testo                  |                    |
|                        |                        |                    |
|                        | **Campo Obbligatorio** |                    |
|                        | = Si                   |                    |
+------------------------+------------------------+--------------------+
| **Tipo di Campo**:     | **Componente da        | Indirizzo mail     |
| stringa                | utilizzare**: Campo di | formattato come    |
|                        | Testo                  | indirizzo@mail.it  |
| **Regole**: email      |                        |                    |
|                        | **Tipo Valore** = Mail |                    |
+------------------------+------------------------+--------------------+
| **Tipo di Campo**:     | **Componente da        | Numero intero      |
| numero                 | utilizzare**: Campo di | (compreso 0)       |
|                        | Testo                  |                    |
| **Regole**: intandzero |                        |                    |
|                        | **Tipo Valore** =      |                    |
|                        | Numerico               |                    |
+------------------------+------------------------+--------------------+
| **Tipo di Campo**:     | **Componente da        | Numero decimale    |
| numero_float           | utilizzare**: Campo di |                    |
|                        | Testo                  |                    |
| **Regole**: float      |                        |                    |
|                        | **Tipo Valore** =      |                    |
|                        | Decimale               |                    |
+------------------------+------------------------+--------------------+
| **Tipo di Campo**:     | **Componente da        | I valori           |
| stringa                | utilizzare**: Campo    | selezionabili      |
|                        | Radio, Campo Lista     | mediante il        |
| **Regole**: booleanSN: | Checkbox, Campo Lista  | componente         |
| S,N                    | Valori                 | utilizzato (e che  |
|                        |                        | verranno poi       |
|                        |                        | inseriti nel       |
|                        |                        | corrispondente     |
|                        |                        | campo Puffin)      |
|                        |                        | dovranno essere    |
|                        |                        | esclusivamente     |
|                        |                        | **S** oppure **N** |
+------------------------+------------------------+--------------------+
| **Tipo di Campo**:     | **Componente da        | I valori           |
| stringa                | utilizzare**: Campo    | selezionabili      |
|                        | Radio, Campo Lista     | mediante il        |
| **Regole**: booleanSN: | Checkbox, Campo Lista  | componente         |
| azienda,cliente        | Valori                 | utilizzato (e che  |
|                        |                        | verranno poi       |
|                        |                        | inseriti nel       |
|                        |                        | corrispondente     |
|                        |                        | campo Puffin)      |
|                        |                        | dovranno essere    |
|                        |                        | esclusivamente     |
|                        |                        | '**azienda'**      |
|                        |                        | oppure             |
|                        |                        | '**cliente'**      |
+------------------------+------------------------+--------------------+

**ATTENZIONE!** nel momento in cui la configurazione del componente
Passweb utilizzato per mappare uno dei campi Puffin gestiti non dovesse
essere coerente con i valori accettati da Puffin, alla conferma del form
(dipendentemente da quello che l'utente andrà effettivamente ad
inserire) potrebbero verificarsi degli errori e l'anagrafica Lead
potrebbe quindi non essere salvata in maniera corretta all'interno del
CRM

In tal senso alcuni campi sono gestiti in maniera leggermente diversa
dagli altri. Stiamo parlando, nello specifico, del campo:

- **Identificativo Paese** -- campo non obbligatorio utilizzato per la
  definizione della Nazione nell'indirizzo del Lead

- **Identificativo provenienza** -- campo obbligatorio utilizzato da
  Puffin per gestire il canale di provenienza del Lead (es. Pubblicità,
  Fiere ...)

- **Identificativo residenza fiscale** -- campo non obbligatorio
  utilizzato per la definizione della residenza fiscale (CEE, Extra
  Cee...) nell'indirizzo del Lead

I possibili valori assunti da questi campi sono infatti definiti da
specifiche liste presenti su Puffin e, per evitare errori in fase di
inserimento del Lead, il valore indicato dall'utente sul Form di Passweb
in corrispondenza di questi campi dovrà coincidere esattamente con uno
dei valori ammessi da Puffin.

In considerazione di ciò, **tali campi dovranno** **necessariamente
essere gestiti con un componente di tipo "Campo Lista Valori"**
configurato con le impostazioni di seguito indicate:

- **Tipo Valore**: Testo

- **Campo Puffin CRM**: Identificativo Paese / Identificativo
  provenienza / Identificativo residenza fiscale

- **Campo Obbligatorio**: Si (senza condizioni di obbligatorietà per
  Identificativo provenienza) / No (per Identificativo Paese /
  Identificativo residenza fiscale)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\puffin_identificativo_provenienza.bmp](./assets/media/image160.png)

Salvando il componente con le impostazioni indicate verranno
automaticamente prelevate da Puffin tutte le possibili opzioni di scelta
che saranno poi visualizzate sul front end del sito all'interno del
corrispondente menu a tendina, opzioni queste che, ora, potranno essere
visualizzate anche nella maschera di configurazione del componente
stesso.

Tornando infatti ad aprire la maschera di configurazione del componente
"Campo Lista Valori" utilizzato per mappare il campo "Identificativo
Provenienza" di Puffin, troveremo ora le diverse possibili opzioni di
scelta all'interno della sezione "**Gestione Valori**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\puffin_identificativo_provenienza_1.bmp](./assets/media/image161.png)

**ATTENZIONE!** per visualizzare le diverse possibili opzioni di scelta
del componente "Campo Lista Valori" utilizzato per mappare i campi
Puffin "Identificativo Paese / Identificativo Provenienza /
Identificativo residenza fiscale" è necessario settare le impostazioni
di configurazione come sopra indicato ed effettuare un primo salvataggio
del componente.

Sono gestiti allo stesso modo anche i Campi Custom di tipo

- **Elenco**

- **Pulsante Radio**

- **Casella Checkbox**

che dovranno quindi mappati con componenti Passweb della stessa
tipologia.

Nello specifico i campi custom di tipo "**Elenco**" dovranno essere
mappati con un componenti Passweb di tipo **"Campo Lista Valori",** i
campi custom di tipo "**Pulsante Radio** con componenti Passweb di tipo
"**Campo Radio**" e i campi custom di tipo "**Casella Checkbox**" con
componenti Passweb di tipo "**Campo Lista Checkbox**"

Anche in questo caso poi sarà necessario effettuare un primo salvataggio
del componente per consentire a Passweb di prelevare le diverse
possibili opzioni definite per questi campi direttamente su Puffin

**Va da sé, ovviamente, che i valori prelevati da Puffin non dovranno in
alcun modo essere modificati**, in caso contrario si potrebbero infatti
riscontrare problemi in fase di salvataggio del form e di creazione
della relativa anagrafica lead su Puffin.

