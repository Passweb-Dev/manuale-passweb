# GESTIONE LINGUE DEL SITO



All'interno di questa sezione del Wizard è possibile impostare la
gestione del proprio sito in più lingue differenti decidendo esattamente
quali lingue gestire, quali attivare effettivamente sul front end e
quale utilizzare come lingua di default.

Accedendo a questa pagina verrà quindi visualizzato un elenco di tutte
le lingue che possono essere effettivamente attivate e gestite per il
proprio sito.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\sito_lingue.bmp](./assets/media/image424.png){width="5.727083333333334in"
height="3.49375in"}

I tre check presenti in corrispondenza di ciascuna lingua presente in
elenco consentono rispettivamente di:

- **Gestita:** consente di indicare se la lingua in esame dovrà o meno
  essere gestita.

> Selezionando questo parametro dunque, la relativa lingua sarà
> perfettamente gestibile all'interno del Wizard dove, per ogni
> componente inserito/da inserire, verranno aggiunti tutti i campi
> necessari per poterne gestire i contenuti e le proprietà nella lingua
> in esame.
>
> **ATTENZIONE! Una lingua Gestita ma non ancora Attivata non potrà mai
> essere visibile sul front end del sito**

- **Attiva:** consente di attivare la relativa lingua rendendola di
  fatto visibile ed accessibile anche sul front end del sito

> **ATTENZIONE! E' possibile attivare solo ed esclusivamente le lingue
> gestite**
>
> Per ovvie ragioni dunque il check Attiva sarà selezionabile solo se,
> per la stessa lingua, è stato messo il segno di spunta anche sul
> precedente parametro "Gestita"

- **Default:** selezionando questo parametro la relativa lingua verrà
  poi considerata come lingua di default per il sito.

> Anche in questo caso, ovviamente il check in questione sarà
> selezionabile solo se, per la stessa lingua, è stato messo il segno di
> spunta sul precedente parametro "Gestita".
>
> Considerando inoltre che la lingua per la quale è stato selezionato
> questo parametro sarà quella in cui verranno poi visualizzate a
> default le pagine del sito, è semplice comprendere come questa stessa
> lingua oltre ad essere correttamente gestita dovrà per forza di cose
> essere anche attiva e quindi perfettamente visibile sul front end del
> sito.
>
> **Per la stessa ragione è possibile impostare come default una sola
> lingua alla volta,** per cui mettendo il segno di segno di spunta su
> "Default" per una determinata lingua, verrà settato automaticamente
> anche il corrispondente flag "Attiva" e contemporaneamente verrà
> deselezionato un eventuale Default impostato su altre lingue.

In virtù di quanto detto il procedimento corretto, anche in ottica SEO,
per attivare e gestire sul sito una lingua aggiuntiva oltre a quella di
Default dovrebbe essere il seguente:

1.  Settare per la lingua desiderata il flag "Gestita" in maniera tale
    da abilitare la gestione all'interno del Wizard

2.  Impostare tutti i contenuti del sito nella lingua appena gestita

3.  Attivare la lingua aggiuntiva rendendola quindi visibile e
    accessibile anche sul front end del sito

**Nel momento in cui si dovesse gestire una determinata lingua senza
averla ancora attivata (fase 2) tale lingua sarà perfettamente
accessibile e visibile sul back end del sito (Wizard), sul front end
invece i contenuti in lingua non saranno ancora accessibili,** verranno
automaticamente oscurate eventuali voci di menù o immagini con link che
puntano ad una lingua non ancora attiva e qualora si tentasse, in
qualche modo, di accedere sul front end ad una pagina in lingua si verrà
automaticamente ricondotti alla home del sito.

In queste condizioni dunque per poter visualizzare sul front end
l'effetto finale che si avrà una volta attivata la lingua aggiuntiva
sarà necessario per forza di cose utilizzare il pulsante "**Accedi
Sito**" presente nella maschera di gestione delle Varianti

**ATTENZIONE! Sulla sitemap del sito generata in automatico da Passweb
verranno inserite solo ed esclusivamente le pagine corrispondenti alle
lingue attualmente attivate**

