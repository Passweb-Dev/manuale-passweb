# CREZIONE DEL BOT TELEGRAM PER L'INVIO DEI MESSAGGI



Come precedentemente evidenziato la prima cosa da fare per consentire a
Passweb di inviare messaggi Telegram al verificarsi di determinati
eventi, sarà creare quella di creare il Bot Telegram che dovrà poi
occuparsi di questa cosa.

Per fare questo l'esercente dovrà:

- Accedere al proprio account Telegram (o in alternativa aprire la
  relativa app) e utilizzare la barra di ricerca della sezione Chat per
  trovare **\@BotFather** (che è il Bot ufficiale di Telegram da
  utilizzare per la creazione di altri Bot)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\bot_telegram_1.bmp](./assets/media/image1.png)

- Una volta trovato il \@BotFather sarà sufficiente avviare una
  comunicazione con lui per visualizzare il messaggio da cui partire per
  la creazione del Bot che verrà poi utilizzato da Passweb per l'invio
  automatico dei messaggi Telegram

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\bot_telegram_2.bmp](./assets/media/image2.png)

- Cliccando sul pulsante "**Avvia**" verrà infatti visualizzata una
  lista di comandi da utilizzare per interagire con \@BotFather

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\bot_telegram_3.bmp](./assets/media/image3.png)

> Nel caso in esame, per creare un nuovo Bot sarà sufficiente utilizzare
> il comando **/newbot** evidenziato in figura (cliccando per questo sul
> relativo link o, in alternativa, inviando a \@BotFather un messaggio
> con il testo /newbot)

- A questo punto, sarà sufficiente continuare la chat con \@BotFather e
  fornire tutte le informazioni che verranno richieste per la creazione
  del Bot ossia **un Nome** e **uno Username** (che dovrà
  necessariamente terminare con la parola bot)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\bot_telegram_4.bmp](./assets/media/image4.png)

- Completata la creazione del Bot, nel successivo messaggio verrà
  indicato un token che sarà poi quello che dovremo inserire (assieme
  allo Username definito al punto precedente) nel Wizard di Passweb per
  completare l'integrazione tra le due piattaforme.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\bot_telegram_5.bmp](./assets/media/image5.png)

- Infine, per completare il processo dovremo collegare il Bot appena
  creato al dominio del sito.

> Per far questo è necessario inviare a \@BotFather il comando
> "**/setdomain**" e rispondere poi indicando prima il nome del Bot
> appena creato (in alternativa è anche possibile cliccare sull'icona
> evidenziata in figura che consente di visualizzare tutti i Bot creati
> con il proprio account Telegram)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\bot_telegram_6.bmp](./assets/media/image6.png)

> e successivamente indicando il domino del proprio sito (comprensivo di
> protocollo https)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\bot_telegram_7.bmp](./assets/media/image7.png)

Volendo è anche possibile personalizzare ulteriormente il Bot
utilizzando i comandi precedentemente evidenziati.

In questo senso potrebbe essere utile associare anche un'immagine al Bot
e, considerando che questa verrà poi mostrata come immagine del mittente
dei messaggi, il consiglio è quello di utilizzare lo stesso logo
presente anche sul sito Ecommerce (o quanto meno un'immagine che
consenta comunque di identificare facilmente il mittente con il sito
Ecommerce).

Per effettuare questa operazione il comando da inviare a \@BothFather è
"**/setuserpic**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\bot_telegram_8.bmp](./assets/media/image8.png)

Anche in questo caso dovremo rispondere indicando il nome del Bot cui
vogliamo associare la nuova immagine

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\bot_telegram_9.bmp](./assets/media/image9.png)

e, infine, utilizzando il pulsante "Allegati" dovremo inviare a
\@BotFather l'immagine da utilizzare

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\bot_telegram_10.bmp](./assets/media/image10.png)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\bot_telegram_11.bmp](./assets/media/image11.png)

