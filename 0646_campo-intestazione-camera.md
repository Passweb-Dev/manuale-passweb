# CAMPO INTESTAZIONE CAMERA



Consente di inserire un titolo utile ad indicare che i dati inseriti poi
nei successivi campi saranno relativi alla camera N

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\form_welcome_campo_intestazione_camera.bmp](./assets/media/image39.png)

**Tipologia di componente Passweb**: Campo Intestazione

**PARAMETRI DI CONFIGURAZIONE DEL COMPONENTE**

**Obbligatorio** = No ma fortemente consigliato

**Condizione di visibilità**: **numeroCamere è in 1,2,3 ...**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\form_welcome_campo_intestazione_configurazione.bmp](./assets/media/image40.png)

Nell'ipotesi che il numero massimo di camere gestite all'interno del
form sia 3, la condizione di visibilità indicata in figura
(**numeroCamere è in 1,2,3**) farà sì che il componente in questione sia
visualizzato nel caso in cui l'utente abbia indicato, in fase di
configurazione del form, un numero camere uguale a 1, a 2 oppure a 3

Considerando poi che il form dovrà gestire un numero massimo di 3
camere, lo stesso componente "Campo intestazione" dovrà essere inserito
anche per il blocco camera 2 e per il blocco camera 3, ovviamente con
una label diversa (Camera 2 piuttosto che Camera 3) e con le seguenti
condizioni di visibilità

**numeroCamere è in 2,3** 🡪 per il blocco relativo alla camera 2.
Consente di visualizzare il componente solo nel caso in cui l'utente
abbia indicato, in fase di configurazione del form, un numero camere
uguale a 2, oppure a 3

**numeroCamere è in 3** 🡪 per il blocco relativo alla camera 3. Consente
di visualizzare il componente solo nel caso in cui l'utente abbia
indicato, in fase di configurazione del form, un numero camere uguale a
3

