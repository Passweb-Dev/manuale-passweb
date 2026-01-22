# GESTIONE DEL VISITOR ID (SCRIPT DI CONFIGURAZIONE DI CLERK).



L'impostazione del parametro "visitor" nello script di configurazione di
Clerk determina il modo in cui verrà generato memorizzato e utilizzato
l'identificativo di ogni visitatore influenzando, di conseguenza, il
comportamento dell'applicativo e quello che dovrà o non dovrà essere
indicato nelle varie informative Privacy e Cookie Policy del sito (
<https://docs.clerk.io/docs/clerkjs-configuration> ).

Sotto questo aspetto Clerk gestisce 4 diverse modalità di Privacy (
<https://help.clerk.io/it/platform/data/cookieless-solution/#privacy-settings>
), corrispondenti alle 4 diverse possibili impostazioni del parametro
visitor:

- visitor: 'auto' -- opzione di default

- visitor: 'persistent'

- visitor: CUSTOM

- visitor: null

**ATTENZIONE!** per maggiori informazioni relativamente allo script di
configurazione di Clerk e ai relativi parametri di configurazione si
veda anche quanto indicato nel precedente capitolo "*Passweb e Clerk --
Integrazione*" di questo manuale

Nei successivi capitoli esamineremo più nel dettaglio ciascuna delle 4
possibili impostazione sopra indicate, mettendo in evidenza cosa
comporta la sua attivazione dal punto di vista applicativo e dal punto
di vista del GDPR.

**ATTENZIONE! in ogni caso Passepartout non è in alcun modo responsabile
in merito all'utilizzo, in maniera conforme a quanto previsto dal GDPR,
di strumenti di terze parti come può essere Clerk, per cui il consiglio
è quello di verificare sempre direttamente con il supporto di Clerk
piuttosto che con il proprio DPO se la soluzione che si è scelto di
adottare è o meno effettivamente conforme a quanto richiesto dalla
normativa**

