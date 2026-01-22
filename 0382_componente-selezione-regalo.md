# COMPONENTE SELEZIONE REGALO



Il Componente **"Selezione Regalo"** può essere inserito solo ed
esclusivamente all'interno della pagina Carrello e/o della pagina Ordine

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\componente_selezione_regalo_res.bmp](./assets/media/image173.png)

e consente di visualizzare, al verificarsi delle condizioni di
applicabilità della relativa Promozione / Buono Sconto, un elenco di
articoli "Omaggio" (o a "condizioni particolari"), tra cui l'utente
potrà selezionare quali andare ad inserire effettivamente in ordine per
poter usufruire della Promozione / Buono Sconto in oggetto.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\selezione_regalo1.bmp](./assets/media/image174.png)

**ATTENZIONE! lato Sito il componente "Selezione Regalo" verrà
effettivamente visualizzato solo ed esclusivamente nel momento in cui
verranno soddisfatte le condizioni di applicabilità della relativa
Promozione / Buono Sconto**

Per maggiori informazioni relativamente alla Promozione e/o ai Buoni
Sconto di tipo "Scegli Articoli in Carrello" (da cui dipende l'effettiva
visualizzazione di questo componente) si vedano anche le sezione
*"Ordini --Promozioni --Promozioni Carrello -- Promozione Azioni --
Scegli Articoli in Carrello"* e "*Ordini -- Buoni Sconto- Azione --
Scegli Articoli in Carrello"* di questo manuale.

Nel momento in cui dovessero dunque essere soddisfatte le condizioni di
applicabilità di una **promozione di tipo "Scegli Articoli in
Carrello",** all' interno di questa stessa pagina l'utente avrà la
possibilità di visualizzare l' elenco di articoli definiti in fase di
configurazione della relativa promozione e avrà la possibilità di
aggiungerli al suo ordine.

**ATTENZIONE! Il fatto che gli articoli presenti in questo elenco
vengano aggiunti gratuitamente in Carrello piuttosto che con uno
specifico sconto, così come il fatto che l'utente abbia la possibilità
di aggiungere uno o più di questi articoli al suo Carrello, dipende da
quelle che sono le condizioni impostate in fase di configurazione della
Promozione stessa.**

Come si può facilmente comprendere dunque l'effettivo funzionamento,
lato sito, di questo componente dipenderà in maniera piuttosto evidente
da quelle che sono le specifiche impostazioni della promozione "Scelta
Articoli in Carrello" cui il componente stesso fa riferimento.

Nello specifico occorre dunque considerare che:

- Nel caso in cui tra gli articoli "omaggio" della promozione sia stato
  inserito un padre di struttura, l'utente prima di poterlo aggiungere
  in Carrello dovrà ovviamente configurarlo in maniera tale da arrivare
  ad indicare un ben preciso articolo figlio

> **ATTENZIONE! In queste condizioni è ovviamente richiesta la presenza
> all'interno del componente "Selezione Regalo" del "Configuratore
> E-Commerce"**

- Nel caso in cui tra gli articoli "omaggio" della promozione sia stato
  inserito un articolo gestito, in Mexal, a Taglie/Colori l'utente potrà
  avere o meno, dipendentemente sempre dalle impostazioni della
  promozione, la possibilità di selezionare la specifica Taglia/Colore
  dell'articolo "omaggio" da inserire in Carrello.

> Nello specifico nel caso in cui la promozione sia stata configurata
> per dare all'utente la possibilità di selezionare la specifica
> Taglia\\Colore, all'interno del componente **"Selezione Regalo"**
> verrà visualizzato, in corrispondenza del componente "Aggiungi in
> Carrello" la grafica minimale (select box) per la selezione della
> Taglia

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\selezione_regalo3.bmp](./assets/media/image175.png)

> Nel caso in cui invece la promozione dovesse consentire all'utente di
> inserire in carrello solo una specifica Taglia\\Colore del relativo
> articolo, la select box sarà disabilitata e l'utente non avrà, in
> questo senso, nessuna possibilità di scelta.

- L'utente potrà selezionare quali articoli, tra quelli presenti in
  elenco inserire in Carrello, **ma non potrà, ovviamente, variare in
  alcun modo la quantità** con cui questi stessi articoli verranno
  effettivamente aggiunti in Carrello. Tali quantità sono infatti
  stabilite dall'amministratore del sito in fase di configurazione della
  relativa Promozione.

- Il prezzo degli articoli "omaggio" verrà visualizzato solo ed
  esclusivamente nel caso in cui tali articoli non siano dei veri e
  propri omaggi ma vengano aggiunti in carrello con uno sconto specifico
  (es. 50%)

- Una volta selezionato uno degli articoli presenti in elenco ed
  aggiuntolo in carrello, questo scomparirà automaticamente dal
  componente "Selezione Regalo". Allo stesso modo nel momento in cui
  l'utente dovesse cambiare idea e decidesse di eliminare dal carrello
  uno degli articoli "omaggio" precedentemente aggiunti, questo tornerà
  ad essere nuovamente visibile e disponibile all'interno del componente
  "Selezione Regalo".

- Nel momento in cui l'utente avrà aggiunto in Carrello il numero
  complessivo di articoli "omaggio" previsti dalla promozione, il
  componente "Selezione Regalo" scomparirà automaticamente e l'utente
  non potrà più aggiungerne altri a meno, ovviamente, di non aver prima
  rimosso dal Carrello uno degli "omaggi" precedentemente aggiunti.

- Gli articoli "omaggio" oggetto della relativa promozione non sono
  sottoposti ad eventuali condizioni di "Filtri Articolo per Utente"

- Gli articoli "omaggio" non verranno ovviamente passati ne alla
  Wishlist ne tanto meno al Comparatore.

- **Gli articoli "omaggio" verranno aggiunti in Carrello in maniera
  gratuita piuttosto che con lo specifico sconto per essi definito, solo
  ed esclusivamente nel caso in cui l'aggiunta al Carrello avvenga
  direttamente dalla pagina Carrello, tramite il Componente "Selezione
  Regalo", oppure partendo dalla loro Scheda Prodotto nel momento in cui
  però questa stessa scheda sia stata raggiunta a partire da uno dei
  link presenti nei componenti interni alla "Selezione Regalo".**

> Ciò significa dunque che se l'utente dovesse visitare la scheda
> prodotto di uno degli articoli presenti all'interno del componente
> "Selezione Regalo" **cliccando su uno dei link associati ai componenti
> interni (es. titolo o immagine) ad esso**, verranno visualizzate per
> lo specifico articolo le condizione definite dalla relativa promozione
> (e quindi l'articolo potrà essere aggiunto, ad esempio, gratuitamente
> in carrello anche in questo modo).
>
> **Nel momento in cui si dovesse invece vistare la scheda prodotto di
> uno di questi articoli partendo dal Catalogo Ecommerce, dai Risultati
> Ricerca, dal componente "Popolarità Prodotto" ecc... l'articolo stesso
> verrà visualizzato e conseguentemente aggiunto in carrello sempre e
> comunque a prezzo pieno.**

