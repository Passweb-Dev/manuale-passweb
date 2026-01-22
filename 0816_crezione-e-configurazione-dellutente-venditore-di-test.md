# CREZIONE E CONFIGURAZIONE DELL'UTENTE VENDITORE DI TEST



Come evidenziato nel precedente capitolo di questo manuale per poter
testare e verificare completamente il funzionamento dell'integrazione
tra il proprio sito Ecommerce e la piattaforma eBay è necessario
lavorare in ambiente Sandbox e disporre, innanzitutto, di un **Account
Venditore di Test** necessario per implementare l'integrazione tra
Passweb ed eBay e permetterci quindi di mettere in vendita determinati
articoli del sito Ecommerce sulla Sandbox di eBay

Per creare un utente Venditore di test è necessario agire ancora una
volta all'interno dell'ambiente di sviluppo di eBay
(<https://developer.ebay.com/signin>) utilizzando l'account creato nel
precedente capitolo di questo manuale.

![](./assets/media/image20.png)

Una volta effettuato l'accesso verrà visualizzata la maschera contente i
set di chiavi di configurazione precedentemente creati tanto per
l'ambiente Sandbox quanto per quello di Produzione.

Sarà quindi necessario cliccare sul pulsante "**Users Tokens**" presente
in corrispondenza della chiave "**App ID**" relativa all'ambiente
Sandbox

![](./assets/media/image21.png)

e, nella successiva maschera, cliccare poi sul pulsante "**Register a
new Sandbox User**" presente all'interno della sezione **"Get a User
Token Here"**

![](./assets/media/image22.png)

In questo modo verrà infatti visualizzato il form di registrazione
dell'utente di Test

![](./assets/media/image23.png)

Una volta inseriti i dati richiesti sarà sufficiente cliccare sul
pulsante "**Create User**" per completare il processo di registrazione e
creare così il nostro nuovo utente di test.

A questo punto sarà necessario **trasformare l'utente appena creato in
un utente di tipo Venditore** con tutte le caratteristiche necessarie
per poterlo effettivamente utilizzare nel processo di integrazione tra
il nostro sito Ecommerce e l'ambiente Sandbox di eBay.

Per far questo dovremo **però agire direttamente all'interno del back
end della Sandbox di eBay**.

Sarà quindi necessario accedere al seguente indirizzo
<https://signin.sandbox.ebay.com> utilizzando le credenziali dell'utente
di test creato al passo precedente.

![](./assets/media/image24.png)

Una volta effettuato l'accesso portarsi nella sezione relativa alle
impostazioni dell'account cliccando per questo sulla prima voce del menu
presente in testata e selezionando, nel relativo menu contestuale, la
voce **"Account Settings"**

![](./assets/media/image25.png)

Nella successiva maschera cliccare sulla voce "**Personal Information**"
presente nel menu posto nella parte sinistra della pagina

![](./assets/media/image26.png)

Cliccare quindi sul pulsante "**Edit**" in corrispondenza della voce
"**Account type**" presente all'interno della sezione "**Account
Information**"

![](./assets/media/image27.png)

In questo modo verremo automaticamente ricondotti all'ambiente Sandbox
di eBay del sito Italiano dove dovremo inserire nuovamente le
credenziali dell' utente di test (le stesse utilizzate in precedenza)

![](./assets/media/image28.png)

**ATTENZIONE!** per poter modificare la tipologia di account di un
utente della Sandbox è necessario partire dalla Sandbox di eBay relativa
al sito americano ( <https://signin.sandbox.ebay.com>), seguire la
procedura appena descritta ed essere ricondotti in automatico alla
Sandbox italiana.

Partendo direttamente dalla Sandbox relativa al sito Italiano, infatti,
non avremo poi modo di accedere alla sezione relativa alle "Informazioni
Utente" da cui poter modificare, come vedremo, la tipologia dell'Account

Una volta effettuato l'accesso verrà visualizzata la maschera
**"Modifica Tipo di account"**

![](./assets/media/image29.png)

all'interno della quale potremo finalmente impostare l'Account
dell'Utente di Test precedentemente creato come quello di un **Venditore
di tipo Business**, selezionando, come evidenziato in figura, la
relativa opzione e cliccando poi sul pulsante "Invia"

**ATTENZIONE! Affinchè il processo di integrazione tra il sito Ecommerce
e l'ambiente Sandbox di eBay possa andare a buon fine è indispensabile
che l'account relativo all'utente di test "Venditore" sia di tipo
Business**

Oltre alla tipologia è consigliabile impostare correttamente anche gli
indirizzi da associare all'Account appena creato.

Per fare questo è necessario collegarsi ancora una volta alla Sandbox
eBay del sito americano, effettuare l'accesso con le credenziali del
nostro utente di tipo Venditore, accedere alla sezione relativa alle
impostazioni dell'Account e cliccare, questa volta, sulla voce
"**Adresses"** presente nel menu posto nella parte sinistra della pagina

![](./assets/media/image30.png)

Dovremo quindi selezionare l'indirizzo da modificare e cliccare sul
relativo pulsante **Change**

![](./assets/media/image31.png)

Come nel caso precedente, anche questa volta, potremmo essere
(dipendentemente dalla tipologia di indirizzo che andremo a modificare)
automaticamente ricondotti alla Sandbox eBay del sito Italiano. Inserite
nuovamente le credenziali dell'utente Venditore ed effettuato l'accesso,
verrà, quindi visualizzata la maschera all'interno della quale poter
immettere le informazioni esatte relativamente all'indirizzo da
modificare

![](./assets/media/image32.png)

