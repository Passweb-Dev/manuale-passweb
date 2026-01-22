# CONDIZIONI DI VISIBILITA' E OBBLIGATORIETA' DEI CAMPI DEL FORM



Per ogni campo (Campo di Testo, Campo Radio, Campo Checkbox, Campo Lista
Valori ecc...) interno ad un Form è possibile definire specifiche
condizioni di visibilità e/o obbligatorietà mediante le quali poter
rendere il controllo stesso visibile e/o obbligatorio sulla base del
valore assunto da altri campi presenti all'interno dello stesso form

Per poter definire tali condizioni è necessario agire rispettivamente
mediante i campi "**Condizione di Visibilità**" e "**Condizione di
Obbligatorietà**" presenti nella maschera di configurazione di ogni
singolo componente interno al Form

![](./assets/media/image144.png)

**ATTENZIONE!** Per i componente "**Pulsante**" e "**Intestazione**" è
presente, per ovvie ragioni, solamente il campo relativo alla condizione
di visibilità

Nello specifico dunque il campo:

**Condizione di Visibilità:** consente di impostare una condizione in
base alla quale poter definire quando il componente in oggetto dovrà o
meno essere visibile all'interno del relativo form.

Come già evidenziato nei precedenti capitoli di questo manuale tale
condizione potrà essere definita sulla base dei valori assunti:

- dal campo "**Nazione**"

> In queste condizioni, affinché il controllo di visibilità possa
> funzionare in maniera corretta sarà necessario, ovviamente, inserire
> nello stesso form anche un campo "**Lista Valori**" mappato sul valore
> "**Nazione**". In questo modo dipendentemente dalla Nazione
> selezionata all'interno del controllo di tipo "Lista Valori" la
> condizione di visibilità potrà o meno essere soddisfatta e,
> conseguentemente, il relativo campo potrà o meno essere visualizzato
> all'interno del form.
>
> **ATTENZIONE!** Nel caso in cui all'interno del form non dovesse
> essere presente alcun campo di tipo "Lista Valori" mappato sul valore
> "Nazione", **la condizione di visibilità verrà valutata, in prima
> istanza, sulla base della lingua impostata sul browser utilizzato per
> navigare il sito**. Nel caso in cui tale lingua sia priva
> dell'indicazione dello specifico paese, la provenienza del visitatore,
> e conseguentemente la condizione di visibilità, verrà valutata invece
> sulla base del suo indirizzo IP (per maggiori informazioni in merito
> si veda anche la sezione "*Sito -- Gestione Lingue del sito --
> Visualizzazione contenuti in lingua*" di questo manuale)

- da uno qualsiasi dei campi presenti all'interno del form per cui sia
  stato correttamente valorizzato, in fase di configurazione, il
  parametro "**Id/name**"

**ATTENZIONE!** nel caso in cui per nessuno dei componenti interni al
form dovesse essere stato impostato un valore per il parametro "Id/name"
l'eventuale condizione di visibilità potrà essere impostata unicamente
sulla base della "Nazione"

Per poter impostare una condizione di visibilità sarà necessario
cliccare sul pulsante "**Aggiungi nuovo filtro**" e selezionare poi, dal
relativo menu a tendina, il campo in base al quale definire la
condizione desiderata.

![](./assets/media/image145.png)

**ATTENZIONE!** all'interno del menu a tendina evidenziato in figura
verranno visualizzato solo ed esclusivamente il campo "Nazione" e
eventuali altri campi del form per cui è stato correttamente valorizzato
il parametro "Id/name"

Fatto questo sarà poi necessario selezionare l'operatore relazionale da
utilizzare per definire la condizione di visibilità oltre che,
ovviamente, il / i valori per i quali la condizione di visibilità dovrà
o meno essere soddisfatta.

![](./assets/media/image146.png)

Cliccando, ad esempio, sull'etichetta "**Nazioni**" verrà aperta una
piccola finestra contenente l'elenco di tutte le nazioni utilizzabili
per definire la condizione di visibilità delle specifico campo del form.

![](./assets/media/image147.png)

Una volta impostate le Nazioni in grado di soddisfare la condizione di
visibilità sarà poi sufficiente chiudere la finestra di selezione del
Paese (cliccando in un qualsiasi punto del box relativo al parametro
"Condizioni di Visibilità") e salvare il componente del form che si sta
modificando mediante l'apposito pulsante posto nella parte alta della
maschera.

**ATTENZIONE! Nel caso in cui un dato campo del form risulti non
visibile a seguito dell'applicazione di determinate condizioni di
visibilità, lo stesso campo non verrà mai considerato come obbligatorio
ai fini della corretta compilazione del form, indipendentemente dal
fatto che, per esso, siano state impostate o meno eventuali condizioni
di obbligatorietà.**

**Condizione di obbligatorietà**: visualizzato solo nel caso in cui il
campo "**Obbligatorio**" sia stato impostato sul valore Si.

Consente di impostare una condizione in base alla quale poter definire
quando il componente in oggetto dovrà o meno essere considerato come
obbligatorio per la corretta compilazione del form.

Come per la "Condizione di Visibilità" anche in questo caso, tale
condizione potrà essere definita sulla base dei valori assunti:

- dal campo "**Nazione**"

- da uno qualsiasi dei campi presenti all'interno del form per cui sia
  stato correttamente valorizzato, in fase di configurazione, il
  parametro "**Id/name**"

Allo stesso modo per poter impostare la condizione di obbligatorietà
sarà necessario cliccare sul pulsante "**Aggiungi nuovo filtro**",
selezionare dal relativo menu a tendina il campo in base al quale
definire la condizione desiderata

![](./assets/media/image148.png)

e impostare poi operatore relazionale e valori per i quali la condizione
di obbligatorietà dovrà o meno essere soddisfatta

**ATTENZIONE!** **Nel caso in cui il campo obbligatorio sia stato
impostato sul valore SI e non siano state definite specifiche condizioni
di obbligatorietà, il campo in esame sarà considerato sempre come
obbligatorio per la corretta compilazione del form.**

