# VISUALIZZAZIONE PRODOTTO



**Nome Evento**: setEcommerceView (corrispondente all'evento "view_item"
di GA4)

**Requisiti di attivazione**: per attivare l'evento in esame è
necessario verificare:

- di aver attivato il tracciamento standard di Matomo

- di aver impostato in fase di configurazione del sito su Matomo il
  parametro "**Ecommerce**" sul valore "**Ecommerce Attivato**"

- di aver selezionato il parametro **Abilita Tracciamento Ecommerce**"
  presente alla pagina "**Sito -- Preferenze -- Tracciamento Dati**"
  (sezione "**Matomo -- Client**") del Wizard del proprio sito Passweb

**Generazione dell'evento**: l'evento in esame verrà attivato visitando
la pagina di dettaglio di un qualsiasi prodotto gestito all'interno del
sito

L'attivazione dell'evento in questione determinerà l'invio a Matomo dei
dati relativi al prodotto visualizzato mediante una chiamata del tipo di
quella di seguito indicata:

*\_paq.push(\[\'setEcommerceView\',*

*"0123456789", // Codice Prodotto*

*"Ecommerce Analytics Book", // Titolo Prodotto*

*"Books", // Categoria Merceologia di appartenenza*

*9.99 // Prezzo ivato*

*\]);*

*\_paq.push(\[\'trackPageView\'\]);*

dove, come evidenziato, i dati relativi al prodotto visualizzato
saranno:

- **Codice Prodotto**

- **Titolo Prodotto**

- **Categoria Merceologica di appartenenza dello specifico prodotto**

- **Prezzo ivato del Prodotto**

Per verificare che l'evento in questione venga tracciato in maniera
corretta è sufficiente accedere al report "**Ecommerce log**" e passare
con il mouse sull'azione relativa alla vista alla pagina prodotto.

![](./assets/media/image30.png)

Se l'evento è stato tracciato in maniera corretta, come evidenziato
nella figura sopra riportata, nel relativo tooltip oltre ai dati della
pagina saranno presenti anche i dati del corrispondente prodotto passati
a Matomo con la chiamata alla funzione setEcommerceView

