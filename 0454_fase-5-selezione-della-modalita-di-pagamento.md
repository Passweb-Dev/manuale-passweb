# FASE 5 -- SELEZIONE DELLA MODALITA' DI PAGAMENTO



In questa fase l'utente avrà la possibilità di selezionare tra quelle
proposte la specifica modalità di pagamento che intende adottare per la
propria prenotazione.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\spiagge_configurazione_18.bmp](./assets/media/image389.png)

Tipicamente potrebbe essere presente un pagamento online (carta di
credito) oppure un pagamento in contanti una volta arrivato in
struttura.

**ATTENZIONE! A seconda della modalità di pagamento selezionata
dall'utente cambierà poi anche lo stato della prenotazione inserita
all'interno del gestionale (con tutto ciò che ne consegue)**

In particolare, nel momento in cui l'utente dovesse selezionare:

- un pagamento on line (PayPal, Carta di credito, Stripe ecc...) la
  prenotazione verrebbe poi inserita nel gestionale in stato di
  "**Confermata**"

- un pagamento in contanti all'arrivo in struttura o comunque non
  immediato, la prenotazione verrebbe poi inserita nel gestionale in
  stato di "**Preventivo**"

**ATTENZIONE**! anche se l'utente dovesse selezionare in questa fase un
pagamento on line, l'effettiva ridirezione sul sito della banca per
completare il pagamento non avverrà in questo step ma solamente al
termine dello step successivo, dopo aver quini revisionato tutti i dati
della propria prenotazione (per maggiori informazioni in merito si veda
anche quanto indicato nel successivo capitolo di questo manuale)

