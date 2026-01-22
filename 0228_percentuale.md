# PERCENTUALE



Al pari degli em, esaminati nel capitolo precedente, anche la
percentuale rappresenta, ovviamente, un'unità di misura relativa e
quindi perfettamente scalabile. Anche in questo caso, inoltre, le varie
regole possono essere applicate "a cascata" dall'elemento "genitore"
all'elemento "figlio".

In sostanza dunque, non c'è una gran differenza tra gli em e le
dimensioni percentuali, anche se, allo stato attuale gli em sembrano
essere l'unità di misura preferita sul web.

Indipendentemente dal fatto di utilizzare gli em o le percentuali,
**occorre però tenere sempre in considerazione che entrambe queste unità
di misura hanno bisogno di un valore di riferimento sulla base del quale
verranno poi calcolate le corrispondenti dimensioni in pixel**.

Questo valore di riferimento non deve necessariamente essere un valore
fissato in pixel ma può essere esso stesso un valore relativo (in em o
in %). Ovviamente però, risalendo nella cascata degli elementi del DOM,
bisognerà pur sempre giungere ad un valore del font-size fissato in
pixel e sulla base del quale poter poi calcolare anche tutte le altre
dimensioni.

Nel caso in cui dunque anche sugli elementi body o html dovesse essere
impostato un font-size in unità di misura relativa (em o %) il valore di
riferimento in pixel sarà quello indicato nei fogli di stile adottati a
default dallo specifico browser.

In questo senso occorre anche fare una considerazione piuttosto
importante legata, principalmente, all'utilizzo di Internet Explorer.

**Nel caso in cui il font-size di riferimento fosse esso stesso relativo
ed impostato in em, dipendentemente dalla versione utilizzata, Explorer
potrebbe non essere in grado di calcolare correttamente le dimensioni
del testo aumentando o diminuendo, senza seguire una regola specifica,
il modo in cui i caratteri verranno effettivamente visualizzati.**

Questo problema può essere risolto utilizzando appunto le dimensioni in
percentuale ed impostando quindi nel body il font-size di riferimento al
100%

body {

font-size: 100%;

}

In questo modo potremo definire il font-size degli altri elementi della
pagina web in em avendo comunque la certezza che i contenuti testuali
presenti all'interno della pagina, vengano correttamente ridimensionati
senza alcun tipo di esagerazione.

