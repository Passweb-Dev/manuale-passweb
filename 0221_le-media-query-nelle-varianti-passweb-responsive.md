# LE MEDIA QUERY NELLE VARIANTI PASSWEB RESPONSIVE



Parlando di media query è bene sottolineare subito come **tutti i
Componenti presenti nella libreria utilizzabile in una qualsiasi
Variante Responsiva di Passweb, implementano nativamente uno specifico
sistema di media query** **che gli consente dunque di adattarsi
perfettamente alle diverse dimensioni dei dispositivi di visualizzazione
del sito.**

Come già per il Meta Tag Viewport, anche per le media query, di base,
non dovremo dunque preoccuparci di nulla.

Sarà sufficiente selezionare il componente desiderato, impostare i suoi
parametri di configurazione ed inserirlo nella pagina. Sarà poi
l'applicazione a preoccuparsi di gestire l'adattamento del Componente
stesso alle diverse dimensioni del dispositivo di visualizzazione.

In realtà, dipendentemente dallo specifico risultato grafico che si
vuole ottenere (es. visualizzazione di un bordo di una cella solo in
dispositivi desktop), potrebbe comunque essere necessario utilizzare
alcuni degli strumenti di editing avanzato offerti da Passweb (es.
Layout di sito e/o Componenti HTML) per scrivere piccole media query
necessarie per ottenere effettivamente l'effetto desiderato.

In questo senso dunque è bene mettere in evidenza come e dove poter
utilizzare in Passweb delle media query.

A seconda di come si intenda gestire queste dichiarazioni sarà
necessario agire in due modi diversi, che prevedono entrambi, l'utilizzo
dei Layout. Nello specifico:

- nel caso in cui si dovesse decidere di creare uno o più fogli di stile
  (file .css) esterni in cui racchiudere tutte le regole CSS che
  dovranno essere applicate al verificarsi di specifiche condizioni,
  sarà poi necessario applicare la media query nel contesto
  dell'attributo **media** all'interno delle elemento **\< link \>** che
  identifica il file CSS da utilizzare.

> **ATTENZIONE!** In queste condizioni non è sufficiente importare il
> file .css esterno tramite la sezione "Inclusione nella Pagina" perché
> questo tipo di inclusione non consente di gestire l'attributo media
> del relativo elemento **\< link \>**
>
> Per risolvere il problema sarà quindi necessario utilizzare la sezione
> "**Meta Tags**" del layout, sezione questa che ci consente di gestire
> manualmente l'elemento \< link \> potendo inserire per esso tutti gli
> attributi necessari, compreso ovviamente l'attributo media.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gr_3_res.bmp](./assets/media/image47.png)

> Nell' esempio riportato in figura il file colore.css viene caricato
> nelle pagine associate al layout in esame solo ed esclusivamente nel
> momento in cui il sito viene visitato da dispositivi in cui l'area di
> visualizzazione del documento (viewport) è compresa tra i 400 e i 1024
> pixel

- nel caso in cui si desideri impostare una query mediante le direttive
  **\@media** o **\@import,** il relativo codice necessario dovrà essere
  inserito direttamente all'interno della sezione CSS del layout di
  pagina / sito

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\gr_4_res.bmp](./assets/media/image48.png)

Per maggiori informazioni in merito alla gestione dei layout Passweb si
veda anche la sezione "*Live Editing per Varianti Responsive -- Layout*"
di questo manuale.

