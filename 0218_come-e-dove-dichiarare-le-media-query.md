# COME E DOVE DICHIARARE LE MEDIA QUERY



Le media query possono essere dichiarate in tre modi diversi:

1.  Si definisce la query nel contesto dell'attributo **media**
    all'interno delle elemento **\< link \>**

> [Esempio:]{.underline}

\<link rel=\"stylesheet\" media**=\"only screen and (color)\"**
href=\"colore.css\" /\>

> In questo modo è possibile condizionare l'applicazione o meno di un
> intero foglio di stile al verificarsi delle condizioni indicate nella
> media query
>
> Questo tipo di istruzione viene generalmente inserita nella sezione \<
> head \> della pagina

2.  All'interno di un foglio di stile si può impostare una query
    mediante la direttiva **\@media**

> [Esempio:]{.underline}

\@media screen and (color) {

/\* qui vanno le regole CSS \*/

}

> In questo modo è possibile condizionare l'applicazione di singole
> regole CSS al verificarsi o meno delle condizioni indicate nella media
> query.
>
> La direttiva **\@media** può essere utilizzata solo ed esclusivamente
> all'interno di un foglio di stile come una qualsiasi altra regola CSS

3.  Si può importare un CSS specifico attraverso una media query usando
    la direttiva **\@import** all'interno di un altro foglio di stile

> [Esempio:]{.underline}

\@import url(colore.css) screen and (color);

> In questo modo è possibile condizionare l'importazione di tutte le
> regole presenti all'interno di un determinato foglio di stile in un
> altro foglio di stile al verificarsi o meno delle condizioni indicate
> nella media query.
>
> La direttiva **\@import** può essere utilizzata solo ed esclusivamente
> all'interno di un foglio di stile

