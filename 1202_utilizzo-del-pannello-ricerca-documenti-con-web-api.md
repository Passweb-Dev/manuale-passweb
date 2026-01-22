# UTILIZZO DEL PANNELLO RICERCA DOCUMENTI CON WEB API



Una volta **attivate le Web Api**, all'interno del pannello "Ricerca
Documenti" troveremo oltre al campo "**Titolo**" anche i campi
"**Data**", "**Classe**" e "**Tipo**", e soprattutto, tale pannello
potrà essere utilizzato per ricercare non solo i documenti presenti
all'interno delle Cartelle Standard ma anche quelli presenti all'interno
del gestionale e associati, per una certa azienda, ad una delle Classi
Docuvision pubblicate sul sito

![](./assets/media/image113.png)

In queste condizioni sarà quindi possibile ricercare documenti per:

- Data

- Classe Documento (Docuvision)

- Tipo Documento (Docuvision)

- Titolo Documento

**ATTENZIONE!** le select "**Classe Documento**" e "**Tipo Documento**"
verranno popolate solo dopo aver selezionato una specifica Azienda e i
relativi parametri di filtro verranno quindi presi in considerazione,
ovviamente, solo in fase di ricerca dei documenti Docuvision

In conseguenza di ciò, nel momento in cui, l'azienda selezionata dovesse
corrispondere ad un utente non esportato dal gestionale ma codificato
direttamente dal back end di Passweb le due select relative alla Classe
Documento e al Tipo Documento saranno ovviamente vuote. In queste
condizioni il pannello "Ricerca Documenti" potrà comunque essere
utilizzato per ricercare i documenti in base alla loro data e/o al loro
Titolo

**ATTENZIONE! la ricerca per titolo del documento è sempre una ricerca
di tipo "contiene"**

Per la stessa ragione, nel momento in cui l'azienda selezionata dovesse
corrispondere ad un utente esportato dal gestionale, indicando come
parametri di filtro la Classe e/o la Tipologia Documento, la ricerca in
esame prenderà in considerazione, ovviamente, i soli documenti
Docuvision (**i documenti caricati direttamente da area riservata non
hanno infatti né una Classe né una Tipologia associata**)

**ATTENZIONE!** Per maggiori informazioni relativamente ai documenti
Docuvision si veda anche quanto indicato nel successivo capitolo di
questo manuale.

