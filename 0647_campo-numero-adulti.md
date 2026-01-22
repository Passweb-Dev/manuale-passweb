# CAMPO NUMERO ADULTI



Consente all'utente che compila il form di indicare il numero di adulti
per la relativa camera

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\form_welcome_campo_numero_adulti.bmp](./assets/media/image41.png){width="5.723611111111111in"
height="3.33125in"}

**Tipologia di componente Passweb**: Campo di Testo

**PARAMETRI DI CONFIGURAZIONE DEL COMPONENTE**

**Id/Name** = numeroAdulti1 -- dove 1 indica che il campo in esame è
relativo alla prima camera

**Tipo Valore** = Numerico

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\form_welcome_campo_numero_adulti_2.bmp](./assets/media/image42.png){width="4.417361111111111in"
height="3.097916666666667in"}

**Obbligatorio** = Si

**Condizioni di visibilità: numeroCamere è in 1,2,3 ...**

**Condizioni di obbligatorietà: numeroCamere è in 1,2,3 ...**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\form_welcome_campo_numero_adulti_3.bmp](./assets/media/image43.png){width="4.417361111111111in"
height="3.1104166666666666in"}

Nell'ipotesi che il numero massimo di camere gestite all'interno del
form sia 3 lo stesso componente "Numero Adulti" dovrà essere inserito
anche per il blocco camera 1, per il blocco camera 2 e per il blocco
camera 3 con le seguenti configurazione:

**[BLOCCO CAMERA 1]{.underline}**

**Id/Name** = numeroAdulti1 -- dove 1 indica che il campo in esame è
relativo alla prima camera

**Tipo Valore** = Numerico

**Obbligatorio** = Si

**Condizioni di visibilità: numeroCamere è in 1,2,3** -- Consente di
visualizzare il componente solo nel caso in cui l'utente abbia indicato,
in fase di configurazione del form, un numero camere uguale a 1, a 2
oppure a 3

**Condizioni di obbligatorietà: numeroCamere è in 1,2,3** -- Consente di
rendere obbligatorio il componente solo nel caso in cui l'utente abbia
indicato, in fase di configurazione del form, un numero camere uguale a
1, a 2 oppure a 3

**[BLOCCO CAMERA 2]{.underline}**

**Id/Name** = numeroAdulti2 -- dove 2 indica che il campo in esame è
relativo alla seconda camera

**Tipo Valore** = Numerico

**Obbligatorio** = Si

**Condizioni di visibilità: numeroCamere è in 2,3** -- Consente di
visualizzare il componente solo nel caso in cui l'utente abbia indicato,
in fase di configurazione del form, un numero camere uguale a 2, oppure
a 3

**Condizioni di obbligatorietà: numeroCamere è in 2,3** -- Consente di
rendere obbligatorio il componente solo nel caso in cui l'utente abbia
indicato, in fase di configurazione del form, un numero camere uguale a
2, oppure a 3

**[BLOCCO CAMERA 3]{.underline}**

**Id/Name** = numeroAdulti3 -- dove 3 indica che il campo in esame è
relativo alla terza camera

**Tipo Valore** = Numerico

**Obbligatorio** = Si

**Condizioni di visibilità: numeroCamere è in 3** -- Consente di
visualizzare il componente solo nel caso in cui l'utente abbia indicato,
in fase di configurazione del form, un numero camere uguale a 3

**Condizioni di obbligatorietà: numeroCamere è in 3** -- Consente di
rendere obbligatorio il componente solo nel caso in cui l'utente abbia
indicato, in fase di configurazione del form, un numero camere uguale a
3

