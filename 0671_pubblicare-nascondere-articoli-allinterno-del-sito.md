# PUBBLICARE /NASCONDERE ARTICOLI ALL'INTERNO DEL SITO



Nel momento in cui l'esigenza dovesse essere quella di non gestire più
determinati articoli all'interno del proprio sito Ecommerce, sarà
possibile procedere in due modi diversi:

1.  Eliminare completamente l'articolo dal sito deselezionando
    l'apposito campo **"Abilita Passweb"** presente nell'anagrafica
    gestionale dell'articolo in esame (sezione "Lista Articoli e
    Listini")

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\anagrafica_ar_horeca2.bmp](./assets/media/image111.png){width="4.779166666666667in"
height="3.0131944444444443in"}

> Per maggiori informazioni relativamente alle modalità di
> esportazione/eliminazione degli articoli all'interno del sito
> e-commerce si vedano anche i precedenti capitoli di questo manuale.
>
> In questo modo alla successiva sincronizzazione l'articolo in
> questione verrà eliminato dal database di Passweb e con esso verranno
> eliminate anche le eventuali risorse associate (immagini, schede
> articolo ecc. ...).

2.  Oscurare temporaneamente la visibilità dell'articolo senza però
    eliminarlo in maniera definitiva dal database di Passweb e senza
    eliminare quindi eventuali immagini e schede tecniche ad esso
    associate e già trasferite sul sito.

La prima soluzione dovrebbe essere adottata nel caso in cui gli articoli
da eliminare non dovessero più essere gestiti all'interno del sito web.
In questo modo infatti si potrebbero "liberare" dei posti per altri
articoli e si potrebbe anche risparmiare dello spazio su disco. Si
ricorda infatti che il numero degli articoli gestiti all'interno del
sito web così come lo spazio su disco sono due parametri limitati in
relazione alla tipologia di contrato sottoscritto.

La seconda soluzione dovrebbe invece essere adottata nel caso in cui
determinati articoli dovessero essere oscurati solo in maniera
temporanea in modo tale dunque da non eliminare definitivamente le
risorse ad essi associate e da non doverle quindi reimportare dal
gestionale qualora questi articoli tornassero ad essere pubblicati
all'interno del negozio web.

Ovviamente in queste condizioni gli articoli e le relative risorse
resteranno nel database di Passweb e non si risparmierà nulla dunque ne
in relazione al numero degli articoli gestiti ne tanto meno in relazione
allo spazio su disco.

**Per poter adottare questa seconda soluzione è sufficiente portarsi
nell'anagrafica Passweb dell'articolo che si è deciso di oscurare in
maniera temporanea e deselezionare il parametro "Pubblica"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\horeca_pubblica_no.bmp](./assets/media/image122.png){width="5.759722222222222in"
height="3.5131944444444443in"}

**ATTENZIONE! A default il parametro "Pubblica" è sempre selezionato.**

In definitiva dunque nel momento in cui per un determinato articolo si
dovesse decidere di deselezionare il parametro evidenziato in figura,
questo stesso articolo non sarà più visualizzato all'interno del sito e,
ovviamente, non potrà più essere acquistato via web.

In ogni caso l'articolo e le relative risorse saranno ancora presenti
all'interno del database di Passweb per cui, se in un secondo momento,
si dovesse decidere di riattivare l'articolo, sarebbe sufficiente
selezionare nuovamente il parametro Pubblica senza dover intervenire in
alcun modo sul gestionale e, soprattutto, senza dover effettuare una
nuova sincronizzazione.

