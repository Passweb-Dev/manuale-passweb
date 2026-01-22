# MONITORAGGIO ECOMMERCE



Nel momento in cui l'esigenza dovesse essere quella sfruttare
l'integrazione diretta Passweb -- Matomo per gestire anche il
tracciamento degli eventi Ecommerce, sarà necessario (oltre ovviamente
ad aver attivato correttamente il tracciamento standard secondo quanto
descritto nel precedente capitolo di questo manuale):

- **Lato Matomo** verificare di aver attivato le relative funzionalità
  impostando, nello specifico, il parametro "**Ecommerce**" presente
  nella maschera di configurazione del sito, sul valore "**Ecommerce
  Attivato**" come nella figura di seguito riportata

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\matomo_29.bmp](./assets/media/image29.png){width="5.157638888888889in"
height="3.532638888888889in"}

- **Lato Passweb** verificare di aver selezionato i due parametri
  "**Abilita Tracciamento Ecommerce**" e "**Abilita Tracciamento
  Ricerca**" presenti alla pagina "**Sito -- Preferenze -- Tracciamento
  Dati**" (sezione "**Matomo -- Client**") del Wizard

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\matomo_28.bmp](./assets/media/image28.png){width="5.795833333333333in"
height="3.50625in"}

**ATTENZIONE!** Se una delle due condizioni non dovesse essere
soddisfatta gli eventuali report presenti in Matomo relativamente all'
Ecommerce e/o alle ricerche effettuate all'interno del sito, potrebbero
non essere creati e/o popolati in maniera corretta

Una volta soddisfatte entrambe queste condizioni verranno quindi
tracciati e inviati alla corrispondente installazione Matomo (definita
nel codice di tracciamento inserito su Passweb) i seguenti eventi:

- **Visualizzazione Prodotto**

- **Aggiornamento carrello**

- **Acquisto**

