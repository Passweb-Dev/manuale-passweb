# CARRELLI ABBANDONATI



La sezione "**Carrelli Abbandonati**" presente all'interno del tab
"**Configurazione**", solo per siti Ecommerce, e solo dopo aver inserito
e salvato i parametri "**BOT Token**" e "**BOT Username**", consente di
impostare alcuni parametri di fondamentale importanza per il corretto
invio dei messaggi Telegram relativi alla creazione dei carrelli
abbandonati.

![](./assets/media/image16.png)

Nello specifico il campo:

**Intervallo per invio messaggio carrelli**: consente di impostare il
numero di ore che dovranno trascorrere prima che l'applicativo possa
inviare messaggi Telegram relativi ad eventuali carrelli abbandonati

**ATTENZIONE!** il messaggio di carrello abbandonato verrà inviato alla
prima sincronizzazione utile successiva all'intervallo di tempo indicato
in corrispondenza del parametro "**Intervallo per invio messaggio
carrelli**"

In sostanza, supponendo di aver impostato il parametro in questione sul
valore 3 (ore), e di registrare un carrello abbandonato sul sito alle
ore 10:00, la corrispondente notifica Telegram verrà inviata alla prima
sincronizzazione utile (per variati o parziale) dopo le ore 13:00.

In queste condizioni dunque, se non dovessero essere effettuati altri
ordini sul sito dopo le 13:00 e la sincronizzazione automatica fosse
schedulata una volta al giorno alle ore 12:00 la notifica di carrello
abbandonato sarebbe inviata, di fatto, il giorno successivo alle ore
12:00.

