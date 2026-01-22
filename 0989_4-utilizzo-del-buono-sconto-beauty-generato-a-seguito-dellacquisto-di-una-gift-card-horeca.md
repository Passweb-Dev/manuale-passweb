# 4 -- UTILIZZO DEL BUONO SCONTO BEAUTY GENERATO A SEGUITO DELL'ACQUISTO DI UNA GIFT CARD HORECA



Per poter utilizzare, all'interno del sito, i Codici delle Gift Card di
tipo HoReCa generati a seguito dell'acquisto di Trattamenti e/o
Ricariche Promozionali, usufruendo così dei relativi Buoni Sconti
Beauty, sarà necessario verificare, innanzitutto, di aver correttamente
abilitato, in fase di prenotazione dei Trattamenti, anche lo step
relativo al pagamento di questi stessi Trattamenti accertandosi quindi
di non aver attivato il parametro "**Nascondi Step pagamento**" presente
nella maschera di configurazione del componente "**Prenotazione Custom
(Reservation)**"

![](./assets/media/image354.png)

In queste condizioni infatti portandosi, in fase di prenotazione di un
Trattamento, nello Step relativo al pagamento troveremo anche il campo
"**Buono Sconto**"

![](./assets/media/image355.png)

e sarà proprio all'interno di questo campo che l'utente dovrà andare ad
inserire il Codice Gift Card che gli consentirà, eventualmente, di
usufruire del relativo Buono Sconto.

Una volta inserito il codice all'interno del campo evidenziato in
figura, cliccando sul pulsante "**Applica**" verranno infatti avviati
tutta una serie di controlli necessari per validare il codice in
questione.

Nello specifico:

- verrà effettuata una chiamata al server Beauty (che dovrà quindi
  essere correttamente contattabile) per verificare se esiste
  effettivamente un Buono Sconto con codice a barre uguale a quello
  inserito dall'utente nel campo sopra evidenziato

- nel momento in cui il primo controllo dia esito positivo e quindi nel
  caso in cui il Buono Sconto esista, verrà verificato se alla data
  odierna tale buono sconto è ancora valido

- nel caso in cui il Buono Sconto dovesse risultare ancora valido verrà
  controllata la tipologia dell'articolo ad esso legato. Se l'articolo
  dovesse essere un prodotto di tipo "Ricarica Promozione" non dovranno
  essere soddisfatte particolari condizioni (un Buono Sconto generato da
  una Ricarica Promozione è infatti spendibile su di un qualsiasi
  Trattamento gestito all'interno del sito). Se invece l'articolo
  collegato ad un Buono Sconto dovesse essere un Trattamento verrà
  verificato che il codice del Trattamento che si sta prenotando sia
  effettivamente lo stesso di quello legato al Buono Sconto che si sta
  tentando di utilizzare

Nel momento in cui uno dei controlli indicati dovesse dare esito
negativo, il Codice Gift Card non potrà essere validato e verrà quindi
visualizzato un apposito messaggio di errore

![](./assets/media/image356.png)

modificabile alla sezione "Testi/Messaggi" del sito (componente
"**Prenotazione Custom (Reservation)**" campo "**Errore Validità Buono
Sconto**").

Nel momento in cui tutti i controlli indicati dovessero invece dare
esito positivo, il Codice Gift Card verrà correttamente validato e verrà
conseguentemente applicato il relativo sconto.

![](./assets/media/image357.png)

**ATTENZIONE!** Se l'importo dell'eventuale Buono Sconto applicato
dovesse essere tale da coprire interamente l'acquisto del Trattamento
verrà nascosta la sezione relativa alla selezione della modalità di
pagamento e la prenotazione potrà quindi essere conclusa con importo
nullo

![](./assets/media/image358.png)

![](./assets/media/image359.png)

Lato gestionale è possibile verificare l'effettiva applicazione di un
Buono Sconto alla prenotazione di un determinato Trattamento aprendo il
dettaglio del Trattamento stesso e richiamando poi, dal relativo menu
contestuale, la maschera relativa al "**Pagamento web**"

![](./assets/media/image360.png)

Il campo "**Buono Sconto**" evidenziato in figura conterrà l'eventuale
Buono applicato alla prenotazione in esame.

Per maggiori informazioni relativamente a come poter chiudere il giro
anche all'interno del gestionale fiscalizzando l'effettiva applicazione
del Buono Sconto si rimanda alla relativa documentazione di Beauty.

