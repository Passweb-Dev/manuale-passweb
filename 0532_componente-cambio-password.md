# COMPONENTE CAMBIO PASSWORD



Il componente "**Cambio Password**" può essere utilizzato all'interno di
una qualsiasi pagina generica (bianca) del sito

![](./assets/media/image8.png)

e consente di inserire all'interno di questa stessa pagina un modulo che
l'utente potrà utilizzare per reimpostare la propria password di accesso
al sito.

![](./assets/media/image9.png)

**Il componente "Cambio Password" diventa dunque di fondamentale
importanza nel momento in cui si dovesse decidere di gestire la
procedura di Recupero Credenziali non con l'invio di queste stesse
credenziali in chiaro all'interno della mail di recupero, ma bensì
mediante l'inserimento in questa stessa mail di un link (valido per sole
24 ore) che l'utente dovrà seguire per reimpostare la propria password
prima di poter effettuare nuovi accesi al sito.**

Cliccando quindi sul link presente nella mail di recupero credenziali
l'utente verrà automaticamente ricondotto ad una specifica pagina del
sito, in cui dovrà essere stato inserito necessariamente il componente
"Cambio Password" e in cui avrà quindi la possibilità di scegliere ed
impostare una nuova Password di accesso per il proprio Account.

**ATTENZIONE!** Una volta effettuato l'accesso alla pagina di Cambio
Password l'utente non potrà navigare in altre sezioni del sito prima di
aver impostato una nuova Password. Allo stesso modo il component di
Cambio Password verrà visualizzato all'interno della pagina solo nel
momento in cui questa stessa pagina dovesse essere raggiunta a partire
dal link presente nella mail di recupero credenziali.

Per attivare questa specifica gestione del recupero password sarà quindi
necessario:

- Inserire nel testo della mail di "Recupero Credenziali" (campo
  "**Testo Email Recupero Credenziali**" della maschera "*Configurazione
  Parametri degli Utenti -- Dati Email*") il segnaposto
  **{{VERIFYURL}}**

![](./assets/media/image10.png)

- Impostare, per tutte le Varianti Sito attualmente gestite, il
  parametro "**Pagina di Cambio Password**" presente nella maschera di
  configurazione della Variante stessa, sulla specifica pagina del sito
  all'interno della quale è stato inserito il componente "Cambio
  Password"

![](./assets/media/image11.png)

**ATTENZIONE!** Nel momento in cui una delle suddette condizioni non
dovesse essere soddisfatta la procedura di recupero credenziali con
l'invio del link per il cambio della Password potrebbe non funzionare in
maniera corretta

Per maggiori informazioni in merito alla procedura di recupero delle
credenziali di accesso al sito si veda anche la corrispondente sezione
di questo manuale ("*Utenti -- Siti Ecommerce -- Configurazione Utenti
Sito -- Configurazione Utenti -- Gestione delle credenziali*")

