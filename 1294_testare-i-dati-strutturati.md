# TESTARE I DATI STRUTTURATI



Una volta deciso quale tipologia di Dati Strutturati utilizzare
all'interno del proprio sito Ecommerce e dopo avere eventualmente
integrato le informazioni gestite in automatico da Passweb con dati
custom, il consiglio è sempre quello di verificare la correttezza di
quanto fatto.

Perché i dati strutturati possano essere efficaci infatti, è
indispensabile che risultino **sintatticamente corretti e che siano
coerenti con il contenuto reale della pagina**

In questo senso, per quel che riguarda la correttezza sintattica Google
offre due strumenti per verificare eventuali errori all'interno dei dati
strutturati presenti in una pagina web

- **Rich Results Test** -- <https://search.google.com/test/rich-results>
  -- Controlla se il codice è idoneo per i rich results e segnala errori
  e avvisi.

- **Schema Markup Validator** -- <https://validator.schema.org> --
  verifica la conformità del codice agli standard di Schema.org.

Per maggiori informazioni relativamente agli strumenti di testing si
rimanda alla relativa documentazione presente in rete.

Per quel che riguarda invece il concetto di coerenza (spesso trascurato
ma di assoluta importanza**) è necessario accertarsi sempre**
(soprattutto nel caso di utilizzo del formato JSON-LD che, come noto,
tenda a separare i dati strutturati dal markup HTML) **che le
informazioni inserite nei dati strutturati coincidano esattamente con
quelle presenti anche nella pagina web.**

Se nei dati strutturati indichiamo, ad esempio, che un prodotto è
"InStock" mentre nel markup HTML della pagina lo stesso prodotto dovesse
risultare esaurito, Google potrebbe considerare questa informazione
ingannevole e, di conseguenza provvedere a scartare il markup.

Lo stesso discorso vale per recensioni inventate, prezzi errati o in
generale per qualsiasi valore non coerenti.

**ATTENZIONE!** le informazioni indicate nei dati strutturati devono
coincidere sempre con le informazioni del contenuto visibile stampato
all'interno della pagina web
