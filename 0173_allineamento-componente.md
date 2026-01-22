# ALLINEAMENTO COMPONENTE



Come evidenziato nei precedenti capitoli di questo manuale le opzioni di
allineamento automatico impostate a default per le colonne di una
griglia piuttosto che per i componenti interni ad una colonna o ad un
contenitore possono essere modificate agendo direttamente sulla singola
colonna piuttosto che sui singoli componenti interni alla colonna stessa
o al contenitore.

In sostanza dunque pur avendo impostato mediante l'icona "Allineamento
dei componenti interni" le colonne di una griglia in maniera tale, ad
esempio, che queste siano tutte allineate a sinistra, è poi possibile
agire sulle impostazioni di configurazione di una singola colonna della
stessa griglia impostandola in maniera tale che essa risulti essere
allineata non più a sinistra ma bensì a destra.

L'icona "**Allineamento Componente**" (
![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\icona_allineamento_componente.bmp](./assets/media/image251.png) ) **consente infatti di impostare
l\'allineamento automatico del componente stesso rispetto al suo
elemento padre.**

**ATTENZIONE!** le opzioni di allineamento automatico del componente
sono prioritarie rispetto a quelle impostate mediante il pulsante di
"Allineamento componenti interni (
![Videate\\icona_allineamento_componenti_interni.bmp](./assets/media/image232.png) )" presente nel R.O.C. dell'elemento
padre di quello attualmente considerato

In relazione alle opzioni di allineamento automatico di un componente
rispetto al suo elemento padre, vanno fatte poi alcune considerazioni di
fondamentale importanza.

Nello specifico è sempre bene ricordare che:

- L'icona di "Allineamento Componente" non verrà mai visualizzata sul
  R.O.C. di componenti di primo livello

- L'icona di "Allineamento Componente" è disponibile per le colonne di
  una griglia, per i componenti comuni interni ad una colonna o ad un
  contenitore e per la maggior parte (**ma non per tutti**) dei
  componenti Ecommerce anch'essi inseriti all'interno di un componente
  contenitore o della colonna di una griglia.

- **Affinchè le impostazioni di allineamento automatico di un componente
  rispetto al suo elemento padre possano funzionare in maniera corretta
  è necessario che, tanto per l'elemento padre, quanto per il componente
  stesso, sia stata impostata una visualizzazione Flex oppure
  Inline-Flex**

Anche in questo caso dunque cliccando sull'icona **Allineamento
Componente** (
![Videate\\icona_allineamento_componente.bmp](./assets/media/image252.png) )" verrà visualizzata nella parte bassa
della pagina una piccola maschera del tutto analoga a quella analizzata
nei precedenti capitoli di questo manuale mediante la quale poter
impostare il tipo di visualizzazione per il componente in esame e le sue
specifiche opzioni di allineamento automatico.

> ![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\opzioni_allineamento_20.bmp](./assets/media/image253.png)

Il menu a tendina presente nella parte alta della maschera consente
dunque di impostare il tipo di visualizzazione che dovrà assumere il
componente in esame. E' possibile selezionare uno dei seguenti valori:

- **Visualizzazione Flex:** selezionando questa opzione:

  - la proprietà display del componente in esame verrà impostata sul
    valore **flex** (tecnicamente verrà assegnata al componente la
    classe **d-flex**)

  - nel caso in cui anche la proprietà display dell'elemento padre fosse
    impostata sul valore flex o inline-flex, il componente in esame
    assumerà una larghezza automatica indipendentemente da come è stato
    impostato il parametro "Larghezza" presente nella maschera di
    configurazione del componente stesso (sezione "Avanzate e
    Animazioni") e si disporrà sempre su di una stessa riga assieme agli
    atri componenti eventualmente presenti all'interno del contenitore
    padre

  - nel caso in cui il componente in esame sia un Componente di tipo
    Contenitore i suoi componenti interni assumeranno una larghezza
    automatica indipendentemente da come è stato impostato per essi il
    parametro "Larghezza" presente nella loro maschera di configurazione
    (sezione "Avanzate e Animazioni") e si disporranno tutti su di una
    stessa riga

> Tecnicamente in questa configurazione verrà assegnata la classe
> "**d-flex**" (corrispondente alla proprietà "display: flex")
> all'elemento Riga della Griglia che è, per l'appunto, l'elemento che
> contiene le varie colonne.

- **Visualizzazione Inline-Flex:** selezionando questa opzione:

  - la proprietà display del componente in esame verrà impostata sul
    valore **inline-flex** (tecnicamente verrà assegnata al componente
    la classe **d-inline-flex**)

  - nel caso in cui anche la proprietà display dell'elemento padre fosse
    impostata sul valore flex o inline-flex, il componente in esame
    assumerà una larghezza automatica indipendentemente da come è stato
    impostato il parametro "Larghezza" presente nella maschera di
    configurazione del componente stesso (sezione "Avanzate e
    Animazioni") e si disporrà sempre su di una stessa riga assieme agli
    atri componenti eventualmente presenti all'interno del contenitore
    padre

  - nel caso in cui il componente in esame sia un Componente di tipo
    Contenitore i suoi componenti interni assumeranno una larghezza
    automatica indipendentemente da come è stato impostato per essi il
    parametro "Larghezza" presente nella loro maschera di configurazione
    (sezione "Avanzate e Animazioni") e si disporranno tutti su di una
    stessa riga.

- **Visualizzazione Custom:** selezionando questa opzione il componente
  in esame manterrà esattamente la sua configurazione iniziale (non gli
  verrà infatti assegnata nessuna classe aggiuntiva) rendendo di fatto
  inutilizzabili le opzioni di allineamento automatico.

> **In queste condizioni dunque i check presenti all'interno, tanto
> della sezione "Orizzontale" quanto di quella "Verticale", saranno
> disattivati.**
>
> In conseguenza di ciò l'allineamento del componente rimarrà
> esattamente quello impostato mediante l'azione di "Allineamento
> componenti interni" effettuata, eventualmente, sul suo elemento padre.

Una volta impostata una Visualizzazione Flex oppure Inline-Flex, i check
presenti all'interno delle sezioni Orizzontale e Verticale permetteranno
di impostare le specifiche opzioni di allineamento automatico del
componente in questione rispetto al suo elemento padre

**[POSSIBILI ALLINEAMENTI ORIZZONTALI]{.underline}**

**Allineamento automatico a sinistra:** il componente in esame verrà
posizionato a fianco di quelli eventualmente già presenti a partire dal
bordo sinistro del componente padre

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\opzioni_allineamento_21.bmp](./assets/media/image254.png)

Tecnicamente, in queste condizioni verrà applicata al componente in
esame la classe "**mr-auto**" che imposta il margine destro del
componente sul valore "auto" allineando così il componente stesso sul
lato sinistro del suo componente padre

**Allineamento automatico a destra:** il componente in esame verrà
posizionato a fianco di quelli eventualmente già presenti a partire dal
bordo destro del componente padre

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\opzioni_allineamento_22.bmp](./assets/media/image255.png)

Tecnicamente, in queste condizioni verrà applicata al componente in
esame la classe "**ml-auto**" che imposta il margine sinistro del
componente sul valore "auto" allineando così il componente stesso sul
lato destro del suo componente padre

**Allineamento automatico centrato:** il componente in esame verrà
posizionato al centro dello spazio residuo presente all'interno del suo
componente padre

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\opzioni_allineamento_23.bmp](./assets/media/image256.png)

Tecnicamente, in queste condizioni verranno applicata al componente in
esame entrambe le classi "**ml-auto**" e "**mr-auto**" posizionando, di
fatto il componente in esame al centro dello spazio residuo.

**[POSSIBILI ALLINEAMENTI VERTICALI]{.underline}**

**Allineamento automatico in alto:** il componente in esame verrà
posizionato a partire dal bordo alto del suo contenitore padre

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\opzioni_allineamento_24.bmp](./assets/media/image257.png)

Tecnicamente, in queste condizioni verrà applicata al componente in
esame la classe "**align-self-start** che imposta la proprietà
**align-self** del componente stesso sul valore **flex-start**
posizionandolo di fatto a partire dal bordo alto del suo elemento padre

**Allineamento automatico in basso:** il componente in esame verrà
posizionato a partire dal bordo basso del suo contenitore padre

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\opzioni_allineamento_25.bmp](./assets/media/image258.png)

Tecnicamente, in queste condizioni verrà applicata al componente in
esame la classe "**align-self-end** che imposta la proprietà
**align-self** del componente stesso sul valore **flex-end**
posizionandolo di fatto a partire dal bordo basso del suo elemento padre

**Allineamento automatico in basso:** il componente in esame verrà
posizionato a partire dal bordo basso del suo contenitore padre

![Videate\\opzioni_allineamento_25.bmp](./assets/media/image259.png)

Tecnicamente, in queste condizioni verrà applicata al componente in
esame la classe "**align-self-end** che imposta la proprietà
**align-self** del componente stesso sul valore **flex-end**
posizionandolo di fatto a partire dal bordo basso del suo elemento padre

**Allineamento automatico centrato:** il componente in esame verrà
posizionato, verticalmente, al centro del suo contenitore padre.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\opzioni_allineamento_26.bmp](./assets/media/image260.png)

Tecnicamente, in queste condizioni verrà applicata al componente in
esame la classe "**align-self-center** che imposta la proprietà
**align-self** del componente stesso sul valore **center**
posizionandolo di fatto al centro del suo elemento padre

**Allineamento automatico baseline:** il componente in esame verrà
posizionato, verticalmente, sulla linea di base del suo contenitore
padre.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\opzioni_allineamento_27.bmp](./assets/media/image261.png)

Tecnicamente, in queste condizioni verrà applicata al componente in
esame la classe "**align-self-baseline** che imposta la proprietà
**align-self** del componente stesso sul valore **baseline.**

**Allineamento automatico stretch:** il componente in esame verrà
"stirato" verticalmente fino ad occupare per intero l'altezza del suo
contenitore padre

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\opzioni_allineamento_28.bmp](./assets/media/image262.png)

Tecnicamente, in queste condizioni verrà applicata al componente in
esame la classe "**align-self-stretch** che imposta la proprietà
**align-self** del componente stesso sul valore **stretch.**

**ATTENZIONE!** nel caso in cui si considerino annidamenti di componenti
a più di due livelli le diverse possibili combinazioni di allineamento
automatico potrebbero diventare via via più complesse.

In questo senso per comprendere il perché di un certo risultato occorre
sempre prestare particolare attenzione a due distinti elementi:

- il tipo di visualizzazione (proprietà display) impostata per
  l\'elemento padre e l\'allineamento automatico eventualmente impostato
  per i suoi figli

- il tipo di visualizzazione (proprietà display) e l\'eventuale
  allineamento automatico impostato per l\'elemento stesso

