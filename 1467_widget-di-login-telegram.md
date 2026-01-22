# WIDGET DI LOGIN TELEGRAM



Una volta creato il Bot Telegram deputato all'invio dei messaggi e
impostata anche l'integrazione tra le due piattaforme, l'ultimo passo
sarà quello di inserire all'interno del sito il "**Widget di Login
Telegram"** in maniera tale da mettere gli utenti che lo desiderano
nelle condizioni di autorizzare l'esercente ad inviargli messaggi via
Telegram

Per configurare questo Widget è necessario accedere al seguente
indirizzo

<https://core.telegram.org/widgets/login>

e impostare i parametri di configurazione come di seguito indicato

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\telegram_widget_login.bmp](./assets/media/image26.png)

Nello specifico:

- **Bot Username**: all'interno di questo campo dovrà essere inserito lo
  Username assegnato al Bot Telegram deputato all'invio dei messaggi e
  impostato anche nei parametri di configurazione del Wizard
  relativamente all'integrazione tra le due piattaforme

> **ATTENZIONE!** per maggior informazioni relativamente alla procedura
> di creazione del Bot Telegram si veda quanto indicato nei precedenti
> capitoli di questo manuale

- **Authorization Type**: relativamente a questo parametro sarà
  necessario selezionare l'opzione "**Redirect to URL**" inserendo poi
  all'interno del successivo campo il seguente indirizzo

> ***https://www.urlsito.com/telegram/callbacklogin***
>
> dove, ovviamente, *www.urlsito.com* andrà sostituito con l'indirizzo
> del proprio sito web
>
> **ATTENZIONE!** l'url del sito dovrà essere inserito esattamente nel
> formato indicato, comprensivo quindi di protocollo https e di path
> finale */telegram/callbacklogin*

- **Request Access:** in corrispondenza di questo parametro sarà
  necessario accertarsi di aver selezionato il corrispondente check

Impostati tutti i parametri di configurazione, sarà necessario prelevare
lo snippet di codice presente in corrispondenza del campo "**Embed
Code**" e inserirlo all'interno del proprio sito utilizzando un
Componente HTML

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\telegram_widget_login_2.bmp](./assets/media/image27.png)

**ATTENZIONE! il Widget Login di Telegram deve essere reso visibile ai
soli utenti autenticati.**

Come è semplice comprendere infatti per poter inviare messaggi ad un
determinato utente è indispensabile poter collegare quello stesso utente
ad un ben preciso account Telegram e questo, ovviamente, potrà avvenire
grazie al Widget Telegram solo però se l'utente ha già effettuato anche
l'autenticazione al sito

**ATTENZIONE!** nel momento in cui il processo di connessione a Telegram
dovesse avvenire da parte di un utente che non ha ancora effettuato
l'autenticazione al sito, l'account Telegram collegato al numero di
cellulare inserito in fase di connessione non potrà essere collegato a
nessuno degli utenti Passweb e, in conseguenza di ciò, quell'account non
potrà mai ricevere alcun tipo di messaggio da parte del sito Ecommerce.

In questo senso quindi il consiglio potrebbe essere quello di inserire
il Widget nella pagina di "Profilo Utente" creando magari anche una
pagina e/o una sezione specifica del sito in cui fornire agli utenti
tutte le indicazioni relative a come poter iscriversi al Bot Telegram e
ricevere così i vari messaggi di notifica

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\telegram_widget_login_3.bmp](./assets/media/image28.png)

**ATTENZIONE!** nel momento in cui l'esigenza dovesse essere quella di
nascondere il Widget di Login Telegram agli utenti autenticati che
dovessero aver già effettuato l'iscrizione al relativo BOT, sarà
possibile utilizzare la classe CSS "**telegramconfigured**" che verrà
assegnata al tag body della pagina solo nel caso in cui l'utente
autenticato risulti essere già iscritto al Bot del sito.

Una volta inserito il Widget, nel momento in cui l'utente dovesse poi
cliccare sul relativo pulsante gli verrà visualizzata una maschera di
accesso a Telegram del tipo di quella evidenziata in figura

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\telegram_widget_login_4.bmp](./assets/media/image29.png)

L'utente dovrà quindi inserire il numero di cellulare collegato
all'account Telegram su cui verranno poi inviati i vari messaggi (numero
questo che potrebbe tranquillamente anche essere diverso da quello
presente nel suo profilo) e cliccare sul pulsante "**Avanti**"

In questo modo, all'account collegato al numero di cellulare indicato,
verrà inviato un messaggio di notifica da parte di Telegram relativo
alla richiesta di accesso appena effettuata con i due pulsanti
"**Rifiuta**" e "**Conferma**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\telegram_widget_login_5.bmp](./assets/media/image30.png)

Cliccando sul pulsante "**Conferma**" l'utente potrà quindi autorizzare
la ricezione di messaggi da parte del Bot.

Contemporaneamente sul sito verrà visualizzata anche un'ulteriore
maschera necessaria per accettare il trasferimento di dati (Nome,
Username e Foto del profilo) tra Passweb e Telegram.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\telegram_widget_login_6.bmp](./assets/media/image31.png)

Per portare a termine il processo di connessione, sarà quindi
sufficiente cliccare sul pulsante "**Accetta**"

A questo punto, se correttamente configurato, l'utente riceverà anche il
primo messaggio automatico (quello di Benvenuto) da parte del Bot del
sito.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\telegram_widget_login_7.bmp](./assets/media/image32.png)

