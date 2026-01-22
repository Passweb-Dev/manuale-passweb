# DOCUVISION



La sezione Docuvision consente all'Agente di accedere in tempo reale al
documentale Passepartout (Docuvision) **e prelevare tutte le risorse
associate all'anagrafica del cliente attualmente selezionato**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_dettaglio_utente_docuvision.bmp](./assets/media/image202.png)

Effettuando l'accesso a questa sezione verrà infatti aperta una
connessione in tempo reale con Mexal e verrà visualizzato l'elenco di
tutte i file associati in Docuvision allo specifico cliente.

**ATTENZIONE! da questa sezione è possibile prelevare le sole risorse
associate in Docuvision alla classe "Anagrafica Cliente"**

Il pannello "**Ricerca Documenti**" consente invece di effettuare
ricerche mirate tra gli allegati Docuvision indicando Data e/o Titolo
del file da ricercare

**ATTENZIONE!** **il pannello di ricerca sarà visibile solo nel caso in
cui siano state correttamente attivate, per il proprio sito Ecommerce,
le Web Api Mexal.** In caso contrario (Web Api non attive) non sarà
quindi possibile effettuare alcun tipo di ricerca tra gli allegati
Docuvision.

Per maggiori informazioni relativamente all'attivazione delle Web Api
Mexal si veda anche quanto indicato nel capitolo "*Configurazione --
Mexal Configurazione Gestionale -- WebApi Mexal*" di questo manuale

Il pulsante "**Download**"
(![Videate\\ar_pulsante_scarica_documento.bmp](./assets/media/image203.png)) presente in corrispondenza di ogni
singola risorsa in elenco consente di scaricare il relativo file.

**ATTENZIONE!** dipendentemente dalle dimensioni del file da scaricare,
e considerando anche che lo stesso file verrà prelevato in tempo reale
dal gestionale, il download potrebbe impiegare un po' di tempo.

In conseguenza di ciò, una volta avviato il download, verrà visualizzata
un'animazione di loading in maniera tale, da una parte, da indicare
all'utente che l'operazione sta procedendo e, dall'altra parte, da
impedirgli di effettuare ulteriori click su eventuali altri documenti da
scaricare prima che l'operazione in essere sia terminata correttamente

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\ar_ec_loading_docuvison.bmp](./assets/media/image204.png)

