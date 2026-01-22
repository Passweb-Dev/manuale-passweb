# ESCLUSIONE DEI BOT "NEGATIVI" DAI SISTEMI DI TRACCIAMENTO



Un bot è un'applicazione programmata per eseguire determinati compiti.

I bot sono automatizzati, funzionano secondo le istruzioni che gli sono
state fornite senza aver bisogno di essere avviati da un utente umano,
di cui spesso imitano o sostituiscono il comportamento ed eseguono
compiti ripetitivi molto più rapidamente di quanto riesca a fare un
essere umano.

Generalmente ogni sito web può interagire con diverse tipologie di bot
presenti in rete, da quelli che scansionano (in modo più o meno lecito)
i contenuti del sito, a quelli che consentono di interagire in diversi
modi (ad esempio creando sistemi di chat per gli utenti) con le pagine
web fino a quelli che cercano semplicemente dei bersagli da attaccare.

Dipendentemente da quello che fanno e da come lo fanno i bot possono
quindi essere considerati "buoni" oppure "cattivi"

Un classico esempio di bot "buoni" è rappresentato dai bot di motori di
ricerca come Google, Bing ... che navigano il sito in maniera
automatizzata per indicizzarne i contenuti e renderli disponibili nelle
varie ricerche che verranno poi effettuate dagli utenti sul web.
Tipicamente questi bot "seguono" le regole definite nel file robots.txt
che ogni sito dovrebbe implementare e che serve proprio per dire a
questi bot come dovranno navigare il sito stesso (con che frequenza, a
quali parti del sito poter accedere ...)

Classici esempi di bot "cattivi" (i cosiddetti "bad bot" o "negative
bot") sono invece quelli che effettuano scraping dei contenuti del sito
senza esplicito permesso, quelli programmati per effettuare tentativi
forzati di accesso a pagine protette del sito, quelli che scansionano il
web per trovare contatti a cui inviare spam o ancora quelli che
bersagliano in maniera continuativa un determinato target (dominio) fino
a portare il sito offline.

Inoltre per sferrare i loro attacchi e occultare la fonte del traffico
molto spesso questi "bad bot" operano e sono distribuiti su diverse
botnet. In altri termini copie dello stesso bot possono essere
distribuite e possono quindi agire partendo da diversi dispositivi,
molto spesso senza che i proprietari degli stessi dispositivi ne siano a
conoscenza, per cui il traffico dannoso in arrivo sul sito potrà
provenire da tantissimi indirizzi IP diversi rendendo più difficile
identificarne e bloccarne l'origine.

Dal punto di vista del sito in sé infatti le richieste (visite) che
arrivano da parte di un bot potrebbero tranquillamente configurarsi come
richieste di un essere umano, o di un bot "lecito". In tutti i casi
infatti queste richieste proverranno da un determinato indirizzo ip,
avranno uno specifico user agent (mascherare lo user agent di una
richiesta web facendolo diventare quello utilizzato da bot "buoni"
piuttosto che quello di veri e propri browser web è una pratica molto
semplice e molto diffusa) ....

Il sito in se quindi non può distinguere se la richiesta di una pagina
web proviene o meno da una fonte lecita e potrà soltanto limitarsi a
fornire i contenuti richiesti.

Va da se quindi che, in queste condizioni, il traffico generato dai bot
"cattivi" può anche travolgere le risorse di un sito web rallentando o
bloccando completamente il servizio per gli utenti umani "legittimi".

Oltre ai danni prodotti da questi bot negativi, che come detto possono
portare anche al down completo del sito, occorre considerare anche che,
nel momento in cui questo traffico non dovesse bloccarlo, potrebbe
comunque portare a falsarne in maniera più o meno considerevole le
statistiche.

Detto quindi che è assolutamente consigliabile proteggersi a monte dal
traffico dannoso prodotto da questi bot negativi dotandosi di appositi
strumenti quali Cloudflare, Cloudfront o qualsiasi altro servizio che
offra la gestione di un WAF (Windows Application Firewall) e che, dal
punto di vista delle statistiche, strumenti di tracciamento quali Google
Analytics implementano già un meccanismo di filtraggio relativo alle
visite prodotte dai bot, restando sempre in ambito di statistiche e di
pulizia del dato da inviare ai relativi sistemi di tracciamento anche
Passweb offre un suo meccanismo di "protezione".

In questo senso infatti Passweb evita nativamente di inviare dati di
tracciamento a Google Analytics e/o a Facebook (sia lato client che lato
server) nel momento in cui la visita o l'azione effettuata sul sito
dovesse provenire da una richiesta web configurata con uno user agent
che rientra nella lista di seguito indicata (lista questa che verrà
aggiornata nel momento in cui si dovessero identificare altri user agent
"dannosi"):

- AhrefsBot

- Babbar

- PetalBot

- Amazonbot

- MJ12bot

- SeekportBot

- SemrushBot

- rogerbot

- dotbot

- DataForSeoBot

- Linguee Bot

- Domain Re-Animator Bot

- MauiBot

- MegaIndex.ru

- BLEXBot

- CCBot

- ChatGPT-User

- GPTBot

- Google-Extended

- anthropic-ai

- Omgilibot

- Omgili

- FacebookBot

- Diffbot

- Bytespider

- ImagesiftBot

- cohere-ai

- ClaudeBot

**ATTENZIONE!** **Il meccanismo in questione si occupa solo ed
esclusivamente di non inviare dati di tracciamento a Google Analytics o
a Facebook nel caso in cui la visita al sito avvenga con uno user agent
tra quelli sopra indicati ma, in nessun caso e in nessun modo, blocca la
visita stessa al sito**

Resta quindi valido il consiglio di proteggersi a monte dal traffico
dannoso generato dai relativi bot e dai danni che possono causare (e di
cui Passepartout non può essere ritenuta responsabile) dotandosi di
appositi strumenti

