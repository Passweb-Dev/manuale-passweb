# ARTICOLI DI TIPO SPESA



Il campo **"Articolo Spesa"** presente nella sezione "Informazioni
Generali" dell'Anagrafica Passweb di ogni singolo articolo

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\horeca_articolo_spesa.bmp](./assets/media/image134.png)

consente, se selezionato, di trattare l'articolo in esame come un
**Articolo di tipo Spesa**.

**ATTENZIONE! E' possibile marcare come articolo di tipo Spesa solo ed
esclusivamente articoli "semplici", ossia articoli che, all'interno del
gestionale, sono stati codificati con Tipologia = Articolo.**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\horeca_articolo_spesa2.bmp](./assets/media/image135.png)

Nel caso in cui si tenti di marcare come articolo di Tipo Spesa un
Prototipo (utilizzato per la gestione delle Varianti Articolo e, dunque,
per gli articoli strutturati) o un Trattamento al' salvataggio
dell'Anagrafica Passweb verrà ritornato un errore

Considerando inoltre l'utilizzo che verrà fatto di questi articoli
all'interno del sito, **è consigliabile utilizzare articoli che non
movimentano il magazzino ed utilizzare per essi un'aliquota iva con
attiva l'opzione "Escludi da sconti e storni" in modo tale da non
dividere su questi articoli eventuali sconti e/o storni.**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\horeca_articolo_spesa3.bmp](./assets/media/image136.png)

Come per i siti Ecommerce collegati a Mexal infatti, anche nel caso di
siti collegati ad uno dei gestionali Ho.Re.Ca. **gli articoli di tipo
Spesa non saranno mai venduti all'interno del sito**.

Una volta selezionato il parametro "Articolo Spesa", al salvataggio
della relativa Anagrafica Passweb, verrà quindi automaticamente
deselezionato il precedente parametro "**Visualizza in Catalogo**"

Tali articoli non saranno quindi visualizzabili in Catalogo ne avranno
una loro specifica pagina Prodotto; **verranno invece utilizzati nella
gestione delle Spese Accessorie, dei Buoni Sconto, delle Promozioni
ecc...** (esattamente come avviene per i siti Ecommerce collegati a
Mexal)

Per un articolo di tipo Spesa,ovviamente, i parametri Pubblica, Offerte,
Novità, Minimo Vendibile ecc... non hanno alcun significato.

**ATTENZIONE! Una volta marcato un articolo come Articolo di Tipo Spesa,
il flag potrà essere rimosso solo ed esclusivamente nel caso in cui
l\'articolo non sia poi stato utilizzato per la gestione delle spese o
degli sconti.**

