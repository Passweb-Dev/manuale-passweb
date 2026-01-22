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

![](./assets/media/image29.png)

- **Lato Passweb** verificare di aver selezionato i due parametri
  "**Abilita Tracciamento Ecommerce**" e "**Abilita Tracciamento
  Ricerca**" presenti alla pagina "**Sito -- Preferenze -- Tracciamento
  Dati**" (sezione "**Matomo -- Client**") del Wizard

![](./assets/media/image28.png)

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

