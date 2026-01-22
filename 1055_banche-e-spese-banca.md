# BANCHE E SPESE BANCA



Per i siti Ecommerce collegati a Mexal, indipendentemente dalla
particolare modalità di pagamento selezionata dal cliente, verranno
calcolate se presenti, ed esattamente allo stesso modo di quanto avviene
all\'interno del gestionale stesso, anche eventuali spese banca, bolli e
sconti/abbuoni relativi al pagamento selezionato. Pertanto:

- Se il cliente non è un privato, le spese banca verranno calcolate
  moltiplicando il valore indicato in Mexal nella relativa tabella
  **\"Importo Spese Banca\"**, ed in relazione anche alla valuta di
  gestione del cliente, per il numero di rate di tipo R,B,A,T,V definite
  per il pagamento in esame.

![](./assets/media/image249.png)

> Su tali spese verrà poi calcolata anche l\'iva secondo con le stesse
> modalità di Mexal.

![](./assets/media/image250.png)

- Se il cliente non è un privato le spese bolli verranno calcolate
  esattamente allo stesso modo di quanto avviene all\'interno di Mexal
  considerando quindi il numero di rate di tipo T definite per il
  pagamento in esame, e la percentuale in millesimi indicata nel campo
  \"Bolli su tratte (%.)\" della tabella \"Bolli/Spese banca/omaggi
  rivalsa iva\" di Mexal.

- Se il cliente è un esportatore abituale (cioè se nelle sue condizioni
  commerciali è stato posto ad S il parametro \"Bollo esp.Ab\" ) e se il
  totale documento supera l\'importo minimo indicato nel campo \"Importo
  minimo\" della tabella \"Bolli/Spese banca/omaggi rivalsa iva\" di
  Mexal, verrà aggiunto al calcolo dei bolli anche il valore del bollo
  per l\'esportatore abituale (campo Bollo della tabella \"Bolli/Spese
  banca/omaggi rivalsa iva\" di Mexal).

**ATTENZIONE:** se per il pagamento in esame è previsto uno sconto
merce, la relativa percentuale verrà sottratta dal totale merce; se è
previsto invece uno sconto abbuono tra i totali del documento verrà
inserita la relativa voce contenente il valore dell\'abbuono che verrà
poi sottratto al totale documento.

Per maggiori informazioni relativamente alla gestione dei bolli e spese
banca si rimanda all'apposita sezione del manuale Mexal.

Per quel che riguarda invece la gestione delle banche nel piede del
documento Mexal occorre considerare che nel momento in cui il pagamento
selezionato dall'utente dovesse avere **delle rate di tipo B (Banca) o T
(Tratte)** allora, in fase di memorizzazione sul gestionale, il campo
"**Banca Azienda**" presente nel piede del relativo documento

![](./assets/media/image251.png)

verrà valorizzato con le coordinate della banca inserita all'interno del
campo "**Banca presentazione effetti**" presente nell'anagrafica
gestionale dell'intestatario del documento

![](./assets/media/image252.png)

Nel caso in cui la "Banca presentazione effetti" dell'intestatario non
dovesse essere impostata il campo "Banca Azienda" verrà valorizzato
invece con le coordinate della banca abituale per bonifici definita
all'interno della relativa tabella gestionale "**Contabilità --
Banche**"

![](./assets/media/image253.png)

Nel caso in cui, infine, non dovesse essere impostata neppure una banca
abituale per i bonifici, ovviamente il campo "Banca Azienda" risulterà
essere vuoto.

**ATTENZIONE!** se, in fase di salvataggio del documento sul gestionale,
si dovessero verificare errori dovuti ad una non corretta configurazione
del conto banca (es. "**Conto Banca non collegato a banca**" o "**Conto
Banca non presente in Rubrica**"), il documento verrà comunque
memorizzato senza però valorizzare in alcun modo il campo "Banca
Azienda".

