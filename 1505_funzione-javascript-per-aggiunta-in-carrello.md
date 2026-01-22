# FUNZIONE JAVASCRIPT PER AGGIUNTA IN CARRELLO



Nel caso in cui si volesse personalizzare e/o automatizzare in qualche
modo la procedura nativa di aggiunta articoli in carrello è possibile
utilizzare la seguente funzione javascript.

Nello specifico:

**Site.cart.addProduct(...)**

che richiede in input i seguenti parametri.

- **\_code**: codice articolo. Se il codice indicato non è presente sul
  database di Passweb viene restituito un messaggio di errore con il
  testo indicato sul Wizard in "Gestione Testi/Messaggi del Sito" in
  corrispondenza della voce "Errore articolo non presente" relativa al
  componente Form.

- **\_quantity**: quantità articolo. Per gestire al meglio i separatori
  dei decimali, il parametro è di tipo stringa. Se la quantità indicata
  non è un decimale superiore a zero viene restituito un messaggio di
  errore con il testo indicato sul Wizard in "Gestione Testi/Messaggi
  del Sito" in corrispondenza della voce "Errore quantità non valida"
  relativa al componente Form.

- **\_size**: taglia articolo. Se il codice articolo fa riferimento ad
  un articolo a taglie è necessario indicare la descrizione in lingua
  della taglia. In mancanza di tale indicazione viene restituito un
  messaggio di errore con il testo indicato sul Wizard in "Gestione
  Testi/Messaggi del Sito" in corrispondenza della voce "Errore taglia
  non indicata" relativa al componente Form. Se la taglia specificata
  non è presente sul database di Passweb viene restituito un messaggio
  di errore con il testo indicato sul Wizard in "Gestione Testi/Messaggi
  del Sito" in corrispondenza della voce "Errore taglia non valida"
  relativa al componente Form. Se l'articolo non è a taglie, il
  parametro può essere valorizzato a NULL e comunque qualsiasi valore
  indicato non viene preso in considerazione.

- **\_discount**: sconto da applicare all'articolo. La valorizzazione di
  tale parametro viene presa in considerazione solo se sul sito si è
  autenticato un agente abilitato alla modifica dello sconto. Se il
  parametro viene valorizzato a NULL verrà applicato all'articolo
  l'eventuale sconto impostato sul gestionale. Se il valore indicato non
  è uno sconto valido viene restituito un messaggio di errore con il
  testo indicato sul Wizard in "Gestione Testi/Messaggi del Sito" in
  corrispondenza della voce "Errore sconto non valido" relativa al
  componente Form.

- **\_price**: prezzo da applicare all'articolo. La valorizzazione di
  tale parametro viene presa in considerazione solo se sul sito si è
  autenticato un agente abilitato alla modifica del prezzo. Se il
  parametro viene valorizzato a NULL verrà applicato all'articolo il
  prezzo impostato sul gestionale. Se il valore indicato non è un prezzo
  valido viene restituito un messaggio di errore con il testo indicato
  sul Wizard in "Gestione Testi/Messaggi del Sito" in corrispondenza
  della voce "Errore prezzo non valido" relativa al componente Form.

- **\_callbackAddProduct**: funzione di callback, per la gestione del
  risultato della funzione.

- **\_checkUserLogged**: controllo se l'utente è loggato. La
  valorizzazione a TRUE abilita il controllo se l'utente che effettua la
  chiamata è loggato o meno. Se il parametro viene valorizzato a NULL
  oppure a FALSE non verrà considerato il controllo sull'utente loggato.
  Se il controllo è abilitato e l'utente non è loggato viene restituito
  un messaggio di errore con il testo indicato sul Wizard in "Gestione
  Testi/Messaggi del Sito" in corrispondenza della voce "Utente non
  loggato" relativa al componente Aggiunti al Carrello.

La funzione in output restituisce un oggetto che può essere gestito
dalla funzione di callback e che ha i seguenti campi.

- **data.errore**: valore booleano che indica se la funzione è stata
  eseguita correttamente. Il valore FALSE indica che non ci sono stati
  errori, altrimenti TRUE.

- **data.messaggio**: testo del messaggio di errore, nel caso in cui non
  ci siano stati errori il messaggio sarà vuoto.

- **data.codiceErrore**: codice numerico dell'errore, nel caso in cui
  non ci siano stati errori il codice è uguale a 0.

Elenco dei codici di errore

- **1**: utente non loggato

- **2**: articolo non presente

- **3**: quantità indicata non corretta

- **4**: taglia non indicata

- **5**: taglia indicata non corretta

- **6**: sconto indicato non valido

- **7**: prezzo indicato non valido

Nel caso in cui valori indicati nei parametri siano corretti, l'articolo
verrà aggiunto in carrello.

La modalità di inserimento in carrello segue quanto indicato sul Wizard
in "Catalogo 🡪 Configurazione Parametri Catalogo" in relazione alla voce
"Modalità di inserimento in carrello".

Nel caso in cui per questo campo sia stata impostata l'opzione "Modifica
riga articolo", se l'articolo che si vuole aggiungere in carrello è già
presente, verranno sommate le relative quantità.

**[Esempi:]{.underline}**

Site.cart.addProduct('PRESINA','4',null,null,null,callbackAddProduct,null);

Viene aggiunto al carrello l'articolo con codice PRESINA in quantità 4.

Site.cart.addProduct('MAGLIA','1','M',null,null,callbackAddProduct,null);

Viene aggiunto al carrello l'articolo con codice MAGLIA in quantità 1 e
taglia M.

Site.cart.addProduct('TEGAME','2',null,'10+20',null,callbackAddProduct,null);

Viene aggiunto al carrello l'articolo con codice TEGAME in quantità 2, e
se sul sito si è autenticato un agente abilitato alla modifica dello
sconto, viene applicato all'articolo lo sconto del 10+20.

Site.cart.addProduct('PRESINA','4',null,null,null,callbackAddProduct,true);

Viene aggiunto al carrello l'articolo con codice PRESINA in quantità 4
solo se l'utente è già loggato.

Site.cart.addProduct('PRESINA','4',null,null,null,myCustomCallbackAddProduct,null);

function myCustomCallbackAddProduct(data){

if(data.errore)

{

console.log(data.codiceErrore + ' ' + data.messaggio);

}

}

