# CATEGORIE LOGICHE



Le categorie di News definite e create secondo le modalità indicate nel
precedente capitolo, potranno essere utilizzate in Passweb
essenzialmente in due modi differenti:

Una volta creato l'albero delle proprie Categorie possiamo utilizzarle
in maniera **standard:**

1)  **Modalità Standard 🡪 Categorie visibili all'interno del sito**. In
    questo caso le categorie di News potranno essere utilizzate per
    generare appositi menu di categoria, in maniera tale da aiutare
    l'utente del sito a ricercare i contenuti che maggiormente gli
    interessano, oppure per creare ad esempio delle "Liste News"
    tematiche e contenenti quindi solo ed esclusivamente le notizie di
    un certo argomento.

> **In queste condizione dunque le categorie di News verranno
> utilizzate, in sostanza, per dire a Passweb cosa pubblicare
> all'interno di determinati componenti CMS**

2)  **Categorie Logiche 🡪 Non visibili all'interno del sito.** Una
    categoria logica altro non è se non una categoria non visualizzabile
    all'interno del sito (parametro "Nascondi categoria sul sito"
    selezionato). Questo tipo di categorie possono essere
    particolarmente utili non tanto per dire a Passweb cosa pubblicare
    all'interno di una pagina del sito, quanto più per dirgli
    esattamente dove pubblicarlo all'interno della pagina stessa.

> Supponiamo ad esempio di dover pubblicare in Home page e in testata
> media una notizia che per un certo periodo di tempo dovrà essere, ad
> esempio, la notizia più recente della categoria "Movie". Al termine di
> questo periodo nella stessa posizione della stessa pagina dovrà invece
> comparire la notizia più recente della categoria "Sport".
>
> Questo problema potrebbe essere risolto in due modi differenti. Si
> potrebbe ad esempio pensare di inserire in testata media un componente
> Lista News configurato, inizialmente, per visualizzare una sola
> notizia (l'ultima) della categoria Movie.
>
> In queste condizioni al termine del periodo in oggetto, dovremmo per
> forza di cose rientrare in editing della pagina e modificare le
> impostazioni del componente facendo in modo che visualizzi ora
> l'ultima notizia della categoria Sport.
>
> In alternativa si potrebbe pensare di risolvere questo problema in un
> modo diverso realizzando appunto una categoria logica denominata, ad
> esempio "Box2" e configurando il componente "Lista News" inserito in
> testata media in modo tale da visualizzare l'ultima News di questa
> specifica categoria logica.
>
> In queste condizioni si potrebbero quindi andare a codificare i due
> post della categoria Movie e Sport assegnandogli periodi di
> pubblicazione contigui ed associandoli, oltre che alle relative
> categorie standard, anche alla categoria logica "Box2".
>
> In questo modo al termine del periodo di pubblicazione della News
> relativa alla categoria Movie, questa verrebbe automaticamente
> eliminata dal sito e al suo posto in testata media della pagina
> verrebbe visualizzata automaticamente la nuova News della categoria
> Sport, senza dover modificare assolutamente nulla.
>
> Tutto ciò perché oltre alle categorie Sport e Movie i post in oggetto
> appartengono anche alla categoria "Box2" e abbiamo detto a Passweb di
> visualizzare in quella specifica posizione di quella specifica pagina
> le News di questa categoria logica indipendentemente poi da quella che
> possa essere effettivamente la loro categoria "standard".
>
> In definitiva dunque grazie alle categorie logiche, una volta definiti
> i Componenti CMS nelle pagine è possibile, non solo decidere a quale
> argomento appartiene la News ("Movie"), ma perfino "dove" verrà
> visualizzata (nel precedente esempio all'interno del "Box2" e in
> Homepage).

**NOTA BENE**: per maggiori informazioni relativamente a come gestire e
configurare il componente CMS "Lista News" si veda anche il
corrispondente capitolo di questo manuale

