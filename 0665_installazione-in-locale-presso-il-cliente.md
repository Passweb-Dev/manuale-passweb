# INSTALLAZIONE IN LOCALE PRESSO IL CLIENTE



Nel caso di installazioni in locale sarà necessario, per prima cosa,
impostare il radio button presente nella parte alta della maschera sul
valore **"Installazione Locale"** in maniera tale da poter visualizzare
tutti i parametri necessari per realizzare l'integrazione
sito-gestionale in questa specifica configurazione di prodotto.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\parametri_conf_Horeca_locale.bmp](./assets/media/image110.png){width="5.8375in"
height="3.532638888888889in"}

In queste condizioni, ovviamente, l'identificazione della specifica
installazione gestionale con cui il sito dovrà colloquiare non potrà
avvenire mediante un "Dominio" ma servirà indicare espressamente
l'indirizzo IP del server e la relativa porta su cui è stato posto in
ascolto il servizio del gestionale deputato al trasferimento dei dati.

In questo senso quindi per completare l'integrazione, oltre ai parametri
già analizzati nel precedente capitolo di questo manuale, sarà
necessario indicare un valore anche per i campi:

**Server**: indirizzo IP o nome della macchina in cui è installato il
server Ho.Re.Ca

**NOTA BENE**: sono gestiti ed accettati anche DNS Dinamici (a patto,
ovviamente, che siano configurati in maniera corretta).

**Porta**: porta sulla quale è stato posto in ascolto il Message Box del
gestionale Ho.Re.Ca. (a default corrisponde alla porta del server del
gestionale + 3)

Per maggiori informazioni relativamente a tutti gli altri parametri di
configurazione è possibile fare riferimento a quanto già indicato nel
precedente capitolo di questo manuale.

