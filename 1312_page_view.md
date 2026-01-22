# PAGE_VIEW



**Nome Evento**: page_view

**Requisiti di attivazione**: per attivare l'evento in esame è
sufficiente verificare di aver attivato correttamente il tracciamento
standard collegato ad una proprietà GA4

**Generazione dell'evento**: l'evento in esame viene gestito in
automatico da Google Analytics (e dal relativo tag di configurazione) e
verrà generato ed inviato ogni volta in cui viene visualizzata una
qualsiasi pagina del sito

All'evento in questione, oltre ai parametri standard gestiti da Google
Analytics (es. page_title, page_location, page_referrer ...) verranno
aggiunti anche i seguenti parametri custom:

**page_type**: Tipologia di pagina visitata.

Il valore assegnato a questo parametro potrà variare in relazione alla
pagina visitata secondo il seguente schema:

- **store_root 🡪** Pagina Catalogo Articoli

- **store_cart 🡪**Pagina Carrello

- **store_checkout 🡪** Pagina di Checkout (Ordine)

- **store_booking 🡪** Pagina di Prenotazione (per siti Ho.Re.Ca.)

- **store_productpage 🡪** Pagine Prodotto (Generica)

- **registration 🡪** Pagina Registrazione (Nuovo Account)

- **profile 🡪** Pagina Profilo (Dati Utente)

- **store_orders 🡪** Pagina Ordini

- **store_page 🡪** Pagine Catalogo (pagine "azzurre")

- **product_page 🡪** Pagina Prodotto di Categoria (pagine "rosse")

- **wishlist 🡪** Pagina Wishlist

- **rma 🡪** Pagina Reso Merce

- **giftregistry 🡪** Pagina Lista Regalo

- **giftcard 🡪** Pagina Gift Card

- **rewardpoints 🡪** Pagina Punti Utente

- **page 🡪** Pagina Generica (pagine "bianche")

**visitor_login_state**: stato dell'utente che visita il sito.

Il valore assegnato a questo parametro varierà in relazione al fatto che
l'utente abbia o meno effettuato l'accesso al sito secondo il seguente
schema:

- **logged-in 🡪** valore assegnato al parametro nel caso in cui l'utente
  abbia già effettuato il login al sito

- **not-logged 🡪** valore assegnato al parametro nel caso in cui
  l'utente non abbia ancora effettuato il login al sito

**visitor_type**: tipologia dell'utente autenticato

Il parametro in esame verrà valorizzato, solo dopo che l'utente che
visita il sito ha effettuato il login, secondo il seguente schema:

- **privato 🡪** valore assegnato al parametro nel caso in cui l'utente
  autenticato sia un "Privato"

- **azienda 🡪**valore assegnato al parametro nel caso in cui l'utente
  autenticato sia un' "Azienda"

