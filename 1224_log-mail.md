# LOG MAIL



All'interno della sezione "**Logging**" accessibile dalla voce del menu
principale "Posta / SMS", è possibile consultare i log delle diverse
tipologie di mail inviate dall'applicativo

Una volta effettuato l'accesso a questa sezione del Wizard verrà infatti
visualizzata la maschera "**Log Mail**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\log_mail.bmp](./assets/media/image25.png)

contenente l'elenco di tutte le mail inviate dall'applicativo.

Il pannello di ricerca presente nella parte alta della pagina consente
di filtrare le mail in elenco in base al loro contenuto

Il campo di ricerca attivabile cliccando sulla lente di ingrandimento,
presente in testata di ogni singola colonna, consente invece di filtrare
i dati in griglia sulla base dei valori presenti all'interno della
colonna stessa.

Una volta impostato un filtro di ricerca, per poterlo poi eliminare sarà
sufficiente cliccare sull'icona raffigurante una piccola lente di
ingrandimento con un -- all'interno (
![Videate\\icona_elimina_filtro.bmp](./assets/media/image26.png) ) che comparirà in testata alla colonna
in corrispondenza della quale è stato impostato il filtro stesso.

Infine è anche possibile ordinare, in maniera crescente e/o decrescente,
gli elementi in griglia cliccando semplicemente sull'icona raffigurante
due piccole frecce posta anch' essa in testata ad ogni singola colonna
della griglia (
![Videate\\icona_ordinamento_griglia.bmp](./assets/media/image27.png) )

I due pulsanti presente nella contestuale barra degli strumenti
consentono rispettivamente di:

- **Visualizza Mail**
  (![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_visualizza_mail.bmp](./assets/media/image28.png) ): consente di accedere al dettaglio
  della mail attualmente selezionata in elenco

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\dettaglio_mail.bmp](./assets/media/image29.png)

> **ATTENZIONE!** nel dettaglio delle mail di recupero password il link
> di recupero è oscurato e sostituito da una serie di XXXXXXXXXX. Tale
> link sarà quindi visibile unicamente nella mail inviata all'utente che
> lo ha richiesto.

- **Invia Mail**
  (![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\pulsante_invia_mail.bmp](./assets/media/image30.png) ): consente di inviare nuovamente la
  mail attualmente selezionata in elenco.

> Tale funzionalità potrebbe quindi tornare particolarmente utile nel
> momento in cui si volesse, ad esempio, tentare di inviare nuovamente
> una mail che per qualsiasi ragione non è stata precedentemente
> consegnata in maniera corretta (Esito = Negativo)
>
> **ATTENZIONE!** Il pulsante "Invia Mail" non è ovviamente visibile nel
> momento in cui quella selezionata in elenco dovesse essere una "Mail
> di recupero Password"
>
> **ATTENZIONE! Le mail inviate mediante la funzionalità in oggetto non
> prenderanno in considerazione eventuali allegati presenti nella mail
> originale**

In caso di errori di invio mail tramite il server di posta esterno
(esito "Negativo" nella relativa colonna), verrà inviata
automaticamente, all'indirizzo impostato in "Configurazione Posta/SMS"
del Wizard, una mail di notifica con mittente
<noreplay@passepartout.net> e con indicato anche:

- Destinatario

- Destinatario in copia

- Oggetto

- Testo

della mail che ha riscontrato il problema.

**ATTENZIONE!** Per verificare il dettaglio dell'errore ed,
eventualmente, procedere ad un nuovo invio sarà necessario accedere alla
sezione "Log Mail" del Wizard.
