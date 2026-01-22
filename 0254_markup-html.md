# MARKUP HTML



In relazione al componente Immagine con Link vanno fatte alcune
considerazione di fondamentale importanza utili a comprendere,
principalmente, il corretto funzionamento dei parametri "**Immagine per
dispositivi Tablet**" e "**Immagini per dispositivi Smartphone**".

Nel fare questo tipo di considerazione va messo in evidenza, per forza
di cose, il markup HTML che viene inserito nella pagina da Passweb in
corrispondenza di un componente "Immagine con Link".

Supponendo dunque di valorizzare tutti i parametri indicati nel
precedente capitolo di questo manuale il markup del componente sarà
esattamente del tipo di quello di seguito indicato.

\<div id=\"imagelink_4551\" class=\" imagelinkComp container-fluid \"\>

\<figure class=\"figure\"\>

\<picture\>

\<source media=\"(max-width: 575px)\"
srcset=\"/Resources/image/img.smartphone.png\"\>

\<source media=\"(max-width: 991px)\"
srcset=\"/Resources/image/img-tablet.png\"\>

\<img src=\"/Resources/image/img-base.jpeg\" class=\"figure-img
img-fluid\" alt=\"valore-attributo-alt\" title=\"valore-attributo-title
\"\>

\</picture\>

\<figcaption class=\"figure-caption\"\>\<h4\>Caption Immagine\</h4\>

\</figcaption\>

\</figure\>

\</div\>

Come si può osservare dunque per gestire il componente Immagine vengono
utilizzati i tag HTML5 figure, picture e source oltre all'attributo
srcset utilizzato per gestire appunto diverse immagini in relazione alle
diverse dimensioni del dispositivo di visualizzazione del sito.

Ora mentre per quel che riguarda i tag principale (figure, picture) non
ci sono grossi problemi di compatibilità tra browser, per quel che
riguarda invece il tag source e soprattutto l'attributo srcset, va detto
che, a livello di browser desktop, non c'è ancora una piena
compatibilità tra i diversi browser.

**Nel caso in cui il visitatore del sito dovesse quindi utilizzare un
browser più datato che non offre supporto a questi elementi,
indipendentemente dal fatto di aver indicato o meno apposite immagini
per i Tablet e/o per gli Smartphone verrà comunque visualizzata sempre e
soltanto l'immagine base, gestita mediante il parametro "Immagine"
precedentemente analizzato e corrispondente al tag img universalmente
riconosciuto**

