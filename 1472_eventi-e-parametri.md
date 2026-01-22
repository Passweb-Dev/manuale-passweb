# EVENTI E PARAMETRI



Come già indicato nei precedenti capitoli di questo manuale Passweb
implementa in maniera nativa il tracciamento dei principali eventi
standard gestiti da Facebook e, in aggiunta a questo, anche il
tracciamento di determinati eventi custom.

Ciò significa dunque che nel momento in cui l'esigenza dovesse essere
quella di tracciare uno o più di questi eventi, una volta attivato in
maniera corretta (e secondo quanto descritto nei precedenti capitoli di
questo manuale) il tracciamento lato server e/o quello lato client, non
saranno poi necessarie ulteriori azioni.

Nello specifico, nel caso del tracciamento lato client non dovremo
quindi preoccuparci di inserire gli snippet di codice javascript
necessari per inviare a facebook informazioni come ad esempio la
visualizzazione di pagina, l'aggiunta di articoli in carrello, il
completamento di un ordine ... perché sarà tutto gestito (sia a livello
client che a livello server) in maniera automatica da Passweb.

L'unica cosa di cui dovremo preoccuparci sarà dunque quella di
configurare in maniera corretta il Business Manager di Facebook per
creare il relativo Pixel e/o per attivare le Conversion API e prelevare
il relativo Access Token.

Il discorso cambia invece nel momento in cui l'esigenza dovesse essere
quella di tracciare uno degli eventi standard di Facebook non
implementati nativamente da Passweb o uno specifico evento
personalizzato che non dovesse rientrare tra quelli già previsti da
Passweb stesso.

In questo caso infatti sarà necessario considerare che:

- Il tracciamento lato client di uno degli eventi standard e/o custom
  non gestiti nativamente da Passweb richiede obbligatoriamente di dover
  gestire l'evento stesso in maniera manuale.

> Sarà quindi necessario verificare innanzitutto di poter effettivamente
> intercettare l'evento in questione secondo le specifiche esigenze del
> caso e andare poi ad inserire il codice javascript indispensabile per
> trasmettere a Facebook l'evento in questione con i relativi parametri

- Considerando che l'utente non ha la possibilità di intervenire sul
  codice server dell'applicativo per poter attivare il tracciamento lato
  server di un evento standard o custom non gestito nativamente da
  Passweb sarà necessario inoltrare a Passepartout un'apposita richiesta
  di implementazione.

Nei successivi capitoli di questo manuale verranno analizzati più nel
dettaglio gli eventi standard e custom con i relativi parametri gestiti
nativamente da Passweb sia nel tracciamento lato client che in quello
lato server

