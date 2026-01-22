# AGGIORNAMENTO CARRELLO



**Nome Evento**: trackEcommerceCartUpdate

**Requisiti di attivazione**: per attivare l'evento in esame è
necessario verificare:

- di aver attivato il tracciamento standard di Matomo

- di aver impostato in fase di configurazione del sito su Matomo il
  parametro "**Ecommerce**" sul valore "**Ecommerce Attivato**"

- di aver selezionato il parametro **Abilita Tracciamento Ecommerce**"
  presente alla pagina "**Sito -- Preferenze -- Tracciamento Dati**"
  (sezione "**Matomo -- Client**") del Wizard del proprio sito Passweb

**Generazione dell'evento**: l'evento in esame verrà generato ed inviato
a Matomo ogni volta in cui verrà aggiornato l'elenco dei prodotti
attualmente presenti in carrello

Questo evento non ha una precisa corrispondenza in Google Analytics.

A differenza di quello che avviene in GA4 infatti, dove sono gestiti
eventi distinti per l'aggiunta e la rimozione di prodotti in carrello,
**in Matomo quello che viene monitorato nello specifico sono i carrelli
abbandonati**

In questo senso quindi l'aggiunta del primo prodotto in carrello
determinerà, nei report Matomo, la creazione di un carrello abbandonato
contenente quello stesso prodotto. Da questo momento in avanti ogni
volta che, nell'ambito della stessa sessione, verranno aggiunti o
rimossi altri articoli in carrello, verrà contestualmente aggiornato su
Matomo il relativo carrello abbandonato.

Se poi l'utente dovesse concludere l'ordine quel carrello abbandonato
verrà automaticamente trasformato in una transazione (ordine)
correttamente conclusa

L'attivazione dell'evento in questione determinerà quindi l'invio ad
analytics dei dati relativi ai prodotti presenti in carrello mediante
una chiamata del tipo di quella di seguito indicata:

*\_paq.push(\[\'addEcommerceItem\',*

*\"0123456789\", // Codice Prodotto*

*\"Ecommerce Analytics Book\", // Titolo Prodotto*

*\[\"Books\", \"Best sellers\"\], // Categorie Merceologiche di
appartenenza*

*9.99, // Prezzo ivato*

*1 // Quantità dell'articolo attualmente presente in carrello*

*\]);*

*\_paq.push(\[\'trackEcommerceCartUpdate\', 15.5\]);*

dove, come indicato, per ogni articolo ancora presente in carrello al
momento dell'aggiornamento verranno inviate a Matomo le seguenti
informazioni:

- **Codice Prodotto**

- **Titolo Prodotto**

- **Categorie Merceologiche di appartenenza dello specifico prodotto**

- **Prezzo ivato del Prodotto**

- **Quantità con cui il prodotto è presente in carrello**

La chiamata *\_paq.push(\[\'trackEcommerceCartUpdate\', 15.5\]);* che
consentirà di effettuare il reale aggiornamento permetterà di passare a
Matomo anche il valore totale del carrello (totale merce + iva + spese)

