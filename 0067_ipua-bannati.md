# IP/UA BANNATI



La sezione "**IP/UA Bannati**" accessibile dalla relativa voce del menu
"**Sito** -- **Preferenze**" del Wizard consente di gestire indirizzi ip
/ user agent ai quali impedire in maniera permanente l'accesso al sito

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\lista_ip_bannati.bmp](./assets/media/image351.png){width="5.941666666666666in"
height="3.5972222222222223in"}

Gli elementi presenti in lista possono essere di due tipi diversi:

- Indirizzi ip / User Agent inseriti manualmente mediante l'apposito
  pulsante presente nella barra degli strumenti (colonna "**Modalità di
  inserimento**" impostata su "**Manuale**")

- Indirizzi ip / User Agent inseriti automaticamente da Passweb a
  seguito di ban permanenti prodotti dalla funzionalità "Prevenzione
  DDos" (colonna "**Modalità di inserimento**" impostata su
  "**Automatico**"). Per maggiori informazioni in merito a questa
  funzionalità di Passweb si rimanda a quanto indicato all'interno del
  capitolo "*Configurazione -- DDos*" di questo manuale

Per aggiungere un nuovo indirizzo IP / User Agent alla black list è
sufficiente cliccare sul pulsante "**Aggiungi IP**" (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_aggiungi.bmp](./assets/media/image352.png){width="0.43472222222222223in"
height="0.21458333333333332in"} ) presente nella contestuale barra degli
strumenti e inserire l'indirizzo o lo user agent desiderato all'interno
del successivo campo **IP/UA**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\nuovo_ip_bannato.bmp](./assets/media/image353.png){width="5.941666666666666in"
height="3.5972222222222223in"}

**ATTENZIONE!** Per ovvie ragioni lo stesso indirizzo IP non potrà
essere inserito contemporaneamente nella lista degli IP Bannati e in
quella degli IP Consentiti

**ATTENZIONE!** La black list definita all'interno di questa sezione ha
effetto solo ed esclusivamente per il front end del sito

Dopo aver aggiunto manualmente nuovi indirizzi ip e/o nuovi user agent
da bannare, per rendere effettive le impostazioni sarà necessario
cliccare sul pulsante "**Applica le nuove impostazioni**" posto nella
parte bassa della maschera.

L'applicazione di queste impostazioni causerà, come indicato dal
relativo messaggio, un riciclo del pool del sito e sarà quindi
necessario effettuare nuovamente l'autenticazione al Wizard

Gli altri pulsanti presenti nella barra degli strumenti consentono
rispettivamente di:

**Modifica** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_modifica.bmp](./assets/media/image349.png){width="0.4027777777777778in"
height="0.18819444444444444in"} ): presente solo per indirizzi ip / user
agent inseriti in maniera manuale. Consente di modificare l'elemento
attualmente selezionato in elenco

**Elimina** (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_elimina.bmp](./assets/media/image347.png){width="0.35694444444444445in"
height="0.18819444444444444in"} ): consente di eliminare dalla black
list l'elemento attualmente selezionato in elenco

**ATTENZIONE! Nel momento in cui si dovesse tentare di accedere al sito
con uno degli indirizzi ip / user agent presenti in elenco verrà
ritornato un errore 403 e l'accesso sarà ovviamente interdetto**

![Videate\\ddos_2.bmp](./assets/media/image354.png){width="5.707638888888889in"
height="1.0715277777777779in"}

