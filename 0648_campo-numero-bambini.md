# CAMPO NUMERO BAMBINI



Consente all'utente che compila il form di indicare il numero di bambini
per la relativa camera

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\form_welcome_campo_numero_bambini.bmp](./assets/media/image44.png)

**Tipologia di componente Passweb**: Campo Lista Valori

**PARAMETRI DI CONFIGURAZIONE DEL COMPONENTE**

**Id/Name** = numeroBambini1 -- dove 1 indica che il campo in esame è
relativo alla prima camera

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\form_welcome_campo_numero_bambini_2.bmp](./assets/media/image45.png)

**Obbligatorio** = No

**Condizioni di visibilità: numeroCamere è in 1,2,3 ...**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\form_welcome_campo_numero_bambini_3.bmp](./assets/media/image46.png)

I valori presenti all'interno della select dovranno essere coerenti,
ovviamente, con il numero di bambini effettivamente gestibili per la
relativa camera

Supponendo dunque che il numero di bambini gestibili per camera sia 2,
in fase di configurazione del componente, i valori da inserire
all'interno della sezione "**Gestione Valori**" dovranno essere 1 e 2

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\form_welcome_campo_numero_bambini_4.bmp](./assets/media/image47.png)

Nell'ipotesi poi che il numero massimo di camere gestite all'interno del
form sia 3 lo stesso componente "Numero Bambini" dovrà essere inserito
anche per il blocco camera 1, per il blocco camera 2 e per il blocco
camera 3 con le seguenti configurazione:

**[BLOCCO CAMERA 1]{.underline}**

**Id/Name** = numeroBambini1 -- dove 1 indica che il campo in esame è
relativo alla prima camera

**Obbligatorio** = No

**Condizioni di visibilità: numeroCamere è in 1,2,3** -- Consente di
visualizzare il componente solo nel caso in cui l'utente abbia indicato,
in fase di configurazione del form, un numero camere uguale a 1, a 2
oppure a 3

**[BLOCCO CAMERA 2]{.underline}**

**Id/Name** = numeroBambini2 -- dove 2 indica che il campo in esame è
relativo alla seconda camera

**Obbligatorio** = No

**Condizioni di visibilità: numeroCamere è in 2,3** -- Consente di
visualizzare il componente solo nel caso in cui l'utente abbia indicato,
in fase di configurazione del form, un numero camere uguale a 2 oppure a
3

**[BLOCCO CAMERA 3]{.underline}**

**Id/Name** = numeroBambini3 -- dove 3 indica che il campo in esame è
relativo alla terza camera

**Obbligatorio** = No

**Condizioni di visibilità: numeroCamere è in 3** -- Consente di
visualizzare il componente solo nel caso in cui l'utente abbia indicato,
in fase di configurazione del form, un numero camere uguale a 3

