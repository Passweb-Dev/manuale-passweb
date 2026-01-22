# CASHBACK WORLD



Cashback World ( <https://www.cashbackworld.com> ) è un servizio di
cashback che consente agli utenti iscritti (e proprietari quindi di una
Cashback Card) di ottenere vantaggi in termini di cashback (restituzione
denaro) e Shopping Point, per ogni ordine effettuato all'interno del
sito.

Per poter attivare questo tipo di servizio è necessario:

- Essere un'azienda convenzionata al sistema Cashback World

- Essere in possesso del Secret Code necessario per la generazione del
  checksum utilizzato per il tracciamento degli ordini.

Soddisfatti questi due requisiti, per completare l'integrazione tra il
proprio sito Passweb e la piattaforma terza sarà poi necessario:

- Inserire il secret code all'interno dell'apposito campo presente nella
  sezione "**Sito -- Preferenze -- Integrazioni**" del Wizard

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sito_cashback_world.bmp](./assets/media/image136.png){width="5.759722222222222in"
height="3.636111111111111in"}

- Inserire lo snippet di codice javascript necessario per il
  tracciamento degli ordini all'interno del campo "**Codice
  completamento**" presente alla pagina "Ordini -- Configurazione Ordini
  -- Documento" del Wizard facendo attenzione al fatto di sostituire
  tutti i dati richiesti (es . totale ordine, checksum, valuta, numero
  ordine ecc...) con i relativi segnaposto messi a disposizione da
  Passweb

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sito_cashback_world_2.bmp](./assets/media/image137.png){width="5.811805555555556in"
height="3.545138888888889in"}

> Per maggiori informazioni relativamente al campo "Codice
> Completamento" si veda anche quanto indicato all'interno della sezione
> "*Ordini -- Ordini -- Configurazione Ordini -- Documento --
> Impostazione di un codice di tracciamento nella pagina di conferma
> ordine*" di questo manuale.
>
> Per quel che riguarda invece il funzionamento di Cashback World (come
> poter aderire al servizio, come ottenere il secret code, dove reperire
> lo snippet di codice javascript necessario per il tracciamento degli
> ordini ...) si rimanda alla documentazione della relativa piattaforma.
>
> **ATTENZIONE!** Affinché l'invio dei dati al sistema Cashback World
> possa avvenire in maniera corretta è necessario accertarsi di aver
> inserito e configurato correttamente, all'interno del campo sopra
> evidenziato, lo snippet di codice javascript necessario per il
> tracciamento degli ordini.

