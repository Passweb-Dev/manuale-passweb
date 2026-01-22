# CONTENITORI STICKY



Per rendere un contenitore Sticky, fissandolo cioè in una specifica
posizione della pagina, è sufficiente selezionare il relativo parametro
presente nella maschera di configurazione del Contenitore stesso

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\contenitore_sticky_0.bmp](./assets/media/image91.png)

**Sticky:** consente di "fissare" il Contenitore in esame in una
specifica posizione, mantenendolo quindi sempre visibile allo scrolling
del sito verso il basso.

**ATTENZIONE!** Una volta assunta la posizione "sticky" al componente
verrà assegnata in maniera del tutto automatica la classe CSS
"**pw-sticky**" che può risultare particolarmente utile nel momento in
cui si dovesse decidere di assegnargli, in queste particolari
condizioni, una diversa formattazione grafica.

Selezionando questo parametro compariranno poi due ulteriori campi
"**Top Position per lo Sticky**" e "**Classe o elemento per fermare lo
sticky**" che consentono rispettivamente di:

- **Top Position per lo Sticky:** consente di impostare l'offset,
  rispetto al bordo alto della pagina, in corrispondenza del quale il
  contenitore in esame dovrà diventare sticky.

> Supponendo dunque di inserire all'interno di questo campo il valore
> 100, il contenitore in questione seguirà lo scrolling del sito
> fintanto che la distanza tra di esso ed il bordo superiore della
> pagina risulti essere maggiore o uguale a 100px. Una volta raggiunta
> tale distanza il contenitore si fisserà invece alla pagina mantenendo
> quindi inalterata la sua posizione indipendentemente dal fatto che
> l'utente continui a scrollare il sito verso il basso.
>
> **ATTENZIONE!** Lasciando il campo vuoto o, in alternativa, impostando
> il valore 0 il Contenitore diventerà sticky una volta raggiunto
> esattamente il bordo alto della pagina web

- **Classe o elemento per fermare lo sticky:** consente di impostare la
  classe CSS (.classeElemento) o l'identificativo (#idElemento) dello
  specifico Componente che dovrà interrompere, una volta entrato
  nell'area visibile della pagina web, per il Contenitore in questione,
  il posizionamento sticky.

> Per maggiori informazioni relativamente a come poter individuare la
> classe o l'id di un componente Passweb si veda anche la sezione "*Live
> Editing -- Componenti -- Azioni Componente -- Informazioni
> Componente*" di questo manuale.
>
> **ATTENZIONE!** **Per ovvie ragioni il parametro Sticky potrà
> funzionare correttamente solo se applicato ad un Contenitore di primo
> livello (che non è stato cioè inserito all'interno di altri componenti
> di tipo Contenitore)**

