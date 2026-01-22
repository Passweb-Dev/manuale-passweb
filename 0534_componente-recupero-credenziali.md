# COMPONENTE RECUPERO CREDENZIALI



Il Componente **"Recupero Credenziali** può essere utilizzato
all'interno di una qualsiasi pagina

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_recupero_credenziali_res.bmp](./assets/media/image13.png)

e consente di inserire all'interno del proprio sito un modulo mediante
il quale un qualsiasi utente avrà la possibilità di resettare, nel caso
in cui le abbia perse, le proprie credenziali di accesso.

Tale Componente potrà essere inserito all'interno di una qualsiasi
pagina del sito indipendentemente dalla sua tipologia.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\recupero_credenziali_sito.bmp](./assets/media/image14.png)

L'utente dovrà semplicemente inserire, nel corrispondente campo,
l'indirizzo mail fornito in fase di registrazione e cliccare poi sul
pulsante "**Recupera**".

> **NOTA BENE:** il testo del pulsante "Recupera" così come i messaggi
> di successo e di errore relativi a questo componente, potranno essere
> modificati e personalizzati all'interno della corrispondente sezione
> "Gestione Testi/Messaggi Sito" del Wizard in corrispondenza del
> componente "Recupero Credenziali".

Alla richiesta di recupero credenziali, se l'indirizzo inserito è
corretto (ed è quindi effettivamente presente nel database di Passweb),
il sistema provvederà ad inviare all'utente una mail contenente la login
di accesso al sito e, soprattutto, un link di recupero su cui l'utente
stesso dovrà cliccare per poter poi impostare una nuova Password.

**ATTENZIONE!** per ragioni di privacy il link di recupero sarà visibile
solo nella mail inviata all'utente che lo ha richiesto. In conseguenza
di ciò nel log della mail di recupero password, consultabile all'interno
del Wizard (sezione "*Posta SMS -- Logging -- Mail*"), tale link sarà
oscurato e sostituito da una serie di XXXXXXXXXX

**Il link presente all'interno della mail ha validità di 24 ore,
trascorse le quali l'utente dovrà effettuare necessariamente una nuova
richiesta di recupero.**

Cliccando su questo link l'utente verrà ricondotto ad una specifica
pagina del sito, in cui dovrà essere stato inserito necessariamente il
componente "**Cambio Password**" e in cui avrà quindi la possibilità di
scegliere ed impostare una nuova Password di accesso per il proprio
Account.

**ATTENZIONE!** Una volta effettuato l'accesso alla pagina di Cambio
Password l'utente non potrà navigare in altre sezioni del sito prima di
aver impostato una nuova Password.

Per maggiori informazioni relativamente al componente "Cambio Password"
si veda anche la corrispondente sezione di questo manuale ("*Varianti
Sito Responsive -- Lista Componenti Interazione Utente -- Componente
Cambio Password*").

**ATTENZIONE! Affinché tutto il processo possa funzionare correttamente
è necessario che siano soddisfatte due condizioni di fondamentale
importanza**.

Nello specifico:

1.  Tutte le Varianti attualmente gestite devono avere impostata una
    specifica pagina di "Cambio Password".

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\varianti_cambio_password.bmp](./assets/media/image11.png)

> **ATTEZNIONE!** Nel caso in cui per una determinata Variante non fosse
> stata indicata, la "Pagina di Cambio Password", il componente
> "Recupero Credenziali" verrà mostrato sul Wizard notificando tale
> mancanza. **Sul front-end del sito invece il componente non verrà
> visualizzato fino a che non sia stata impostata la "Pagina di Cambio
> Password"**.
>
> Per maggiori informazioni in merito a come e dove impostare tale
> pagine si veda anche la corrispondente sezione di questo manuale
> ("*Varianti Sito Responsive -- Creazione e gestione di una Variante
> Responsiva*")

2.  Nel testo della mail di "Recupero Credenziali" (campo "**Testo Email
    Recupero Credenziali**" della maschera "**Configurazione Parametri
    degli Utenti -- Dati Email**") deve essere stato inserito
    necessariamente il segnaposto **{{VERIFYURL}}**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\segnaposto_link_cambio_password.bmp](./assets/media/image10.png)

> **ATTENZIONE!** Qualora nel testo della mail di recupero credenziali
> non sia stato inserito il segnaposto \"{{VERIFYURL}}\", al salvataggio
> questo verrà inserito automaticamente in fondo al testo.

