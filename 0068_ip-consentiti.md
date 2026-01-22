# IP CONSENTITI



La sezione "**IP Consentiti**", accessibile dalla relativa voce del menu
"**Sito** - **Preferenze**", consente di specificare un elenco di
indirizzi IP cui sarà consentito l'accesso al sito, specificando anche
se tale accesso potrà avvenire solo sul front end, solo sul back end
(Wizard) o su entrambe le parti dell'applicazione.

![](./assets/media/image355.png)

**ATTENZIONE! Nel momento in cui dovesse essere inserito anche un solo
indirizzo IP all'interno di questa maschera, l'accesso al front end /
back end del sito sarà inibito a tutti gli indirizzi IP tranne quelli
indicati in maniera specifica all'interno di questa stessa maschera**

Come per gli IP bannati, anche in questo caso se si dovesse tentare di
accedere al front end / back end del sito con un indirizzo IP non
consentito verrà ritornato un errore 403

**ATTENZIONE!** Per ovvie ragioni lo stesso indirizzo IP non potrà
essere inserito contemporaneamente nella lista degli IP Consentiti e in
quella degli IP Bannati

Per aggiungere un nuovo indirizzo IP alla white list è sufficiente
cliccare sul pulsante "**Aggiungi IP**" (
![](./assets/media/image356.png) ) presente nella contestuale barra degli strumenti e
inserire l'indirizzo desiderato all'interno del corrispondente campo
**IP**

![](./assets/media/image357.png)

Il parametro "**Applicazione**" consente invece di specificare se per
l'indirizzo IP indicato l'accesso potrà essere consentito solamente al
Back-end (Wizard) del sito, solamente al Front end oppure ad entrambe le
parti dell'applicazione.

**ATTENZIONE!** l'esposizione dell'interfaccia amministrativa (Wizard)
del sito sul perimetro della rete pubblica aumenta, ovviamente,
l'esposizione del sito stesso a possibili attacchi di tipo "forza bruta"
atti ad individuare credenziali di accesso deboli. In questo senso,
anche se Passweb tende comunque a proteggere l'accesso alla parte
amministrativa mediante meccanismo di autenticazione a due fattori, è
sempre consigliabile utilizzare credenziali di accesso sufficientemente
complesse e, laddove possibile, limitare anche l'accesso al back end ai
soli indirizzi IP effettivamente autorizzati a questo tipo di
operazioni.

Gli altri pulsanti presenti nella barra degli strumenti consentono
rispettivamente di:

**Modifica IP** (
![](./assets/media/image358.png) ): consente di modificare l'indirizzo IP
attualmente selezionato in elenco

**Elimina IP** (
![](./assets/media/image359.png) ): consente di eliminare dalla white
list l'indirizzo IP attualmente selezionato in elenco.

Una volta impostato l'elenco di IP Consentiti, per rendere effettive le
impostazioni sarà necessario cliccare sul pulsante "**Applica le nuove
impostazioni**" posto nella parte bassa della maschera

**ATTENZIONE!** Il salvataggio delle impostazioni e l'applicazione della
lista di IP Consentiti comporta il riciclo e conseguentemente il riavvio
del sito

