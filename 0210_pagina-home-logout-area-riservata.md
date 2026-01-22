# PAGINA HOME / LOGOUT AREA RISERVATA



All'interno della sezione "**Pagina Home / Logout Area Riservata**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\variante_res_pagina_logout.bmp](./assets/media/image41.png){width="5.149305555555555in"
height="3.1569444444444446in"}

è possibile impostare, per la Variante in esame, la pagina del sito cui
dovrà essere indirizzato l'utente nel momento in cui dovesse cliccare:

- sul pulsante di **Logout** presente in Area Riservata

> ![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\area_riservata_logout.bmp](./assets/media/image42.png){width="1.30625in"
> height="1.0895833333333333in"}

- sul pulsante **Home**
  (![Videate\\ar_menu_home.bmp](./assets/media/image43.png){width="0.17916666666666667in"
  height="0.17916666666666667in"}) presente anch'esso in Area Riservata:

Nel caso in cui non dovesse essere indicata nessuna pagina:

- effettuando il logout dall'area riservata l'utente verrà indirizzato
  alla pagina di accesso all'area riservata stessa, pagina questa
  gestita in automatico dall'applicazione

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\accesso_area_riservata.bmp](./assets/media/image44.png){width="5.552083333333333in"
height="3.5145833333333334in"}

- cliccando sul tasto Home l'utente verrà invece reindirizzato alla Home
  Page del sito

**[ATTENZIONE!]{.underline}**

Nel momento in cui l'esigenza dovesse essere quella di far si che, tanto
al logout del sito, quanto cliccando sul tasto Home, l'utente venga
reindirizzato ad una pagina di un sito diverso dal sito Passweb, sarà
necessario:

- Creare una apposita pagina all'interno del proprio sito Passweb, priva
  di componenti e denominata, ad esempio "Redirect Area Riservata"

- Inserire nella sezione \< head \> della suddetta pagina il meta tag di
  seguito indicato

> **\< meta http-equiv=\"refresh\"
> content="0;URL=http://www.sito.it/pagina" \>**
>
> dove, ovviamente, in corrispondenza del parametro URL andrà indicato
> l'indirizzo assoluto della pagina del sito cui l'utente dovrà essere
> reindirizzato

- Impostare la suddetta pagina come "Pagina Home / Logout Area
  Riservata" mediante l'apposito parametro presente nella maschera di
  configurazione della Variante Sito in esame.

