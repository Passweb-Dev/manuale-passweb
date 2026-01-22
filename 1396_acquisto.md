# ACQUISTO



**Nome Evento**: trackEcommerceOrder (corrispondente all'evento
"purchase" di GA4)

**Requisiti di attivazione**: per attivare l'evento in esame è
necessario verificare:

- di aver attivato il tracciamento standard di Matomo

- di aver impostato in fase di configurazione del sito su Matomo il
  parametro "**Ecommerce**" sul valore "**Ecommerce Attivato**"

- di aver selezionato il parametro **Abilita Tracciamento Ecommerce**"
  presente alla pagina "**Sito -- Preferenze -- Tracciamento Dati**"
  (sezione "**Matomo -- Client**") del Wizard del proprio sito Passweb

**Generazione dell'evento**: l'evento in esame verrà attivato ogni volta
in cui verrà concluso un' ordine

Come indicato nella documentazione ufficiale di Matomo (
<https://matomo.org/faq/reports/advanced-manually-tracking-ecommerce-actions-in-matomo/>
) il tracciamento delle transazioni concluse all'interno del sito
comporta l'invio a Matomo di due diversi insiemi di dati (e quindi la
creazione di due distinte push), il primo relativo all'insieme dei
prodotti aggiunti in ordine (e analogo a quello già utilizzato per
gestire l'aggiornamento dei prodotti attualmente in carrello) che si
espliciterà mediante una chiamata del tipo di quella di seguito
indicata:

*\_paq.push(\[\'addEcommerceItem\',*

*\"0123456789\", // Codice Prodotto*

*\"Ecommerce Analytics Book\", // Titolo Prodotto*

*\[\"Books\", \"Best sellers\"\], // Categorie Merceologiche di
appartenenza*

*9.99, // Prezzo ivato*

*1 // Quantità dell'articolo attualmente presente in carrello*

*\]);*

dove, come evidenziato, i dati relativi ad ogni prodotto presente in
ordine saranno esattamente:

- **Codice Prodotto**

- **Titolo Prodotto**

- **Categorie Merceologiche di appartenenza dello specifico prodotto**

- **Prezzo ivato del Prodotto**

- **Quantità con cui il prodotto è presente in ordine**

Il secondo insieme di dati inviati a Matomo sarà invece quello relativo
ai dettagli dell'ordine e si espliciterà questa volta mediante una
chiamata del tipo di quella di seguito indicata:

*\_paq.push(\[\'trackEcommerceOrder\',*

*\"000123\", // Id Ordine*

*10.99, // Totale Ordine*

*9.99, // Sub Totale (Totale Ordine -- Spese di spedizione)*

*1.5, // Tasse (IVA)*

*1 // Spesi di spedizione*

*\]);*

dove, come evidenziato, i dati relativi all'ordine appena concluso
saranno esattamente:

- **Id Ordine**

- **Totale Ordine**

- **Sub Totale (calcolato come "Totale Ordine -- Spese di spedzione")**

- **Tasse (IVA)**

- **Spese di spedizione**

