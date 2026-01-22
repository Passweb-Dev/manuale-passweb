# JAVASCRIPT



L'editor di codice presente all'intero di questa sezione consente di
gestire codice javascript personalizzato che verrà poi eseguito in tutte
le pagine cui si deciderà di associare il layout in questione.

> **NOTA BENE:** per inserire codice in modalità full screen utilizzare
> il tasto funzione **"F11"**. Per tornare alla modalità di
> visualizzazione originale utilizzare il tasto "ESC"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\inserimento_js_personalizzato_res.bmp](./assets/media/image166.png)

Anche in questo, caso, come già per la sezione CSS sono attivi, i
seguenti tasti funzione:

- **Ctrl + F / Cmd + F** Consente di abilitare la funzione di ricerca
  all'interno dell'editor di codice HTML, attivando il relativo campo di
  testo

- **Ctrl + G / Cmd + G**: Consente, una volta effettuata una specifica
  ricerca all'interno dell'editor di codice HTML, di attivare la
  funzione "**Passa al successivo**"

- **Shift + Ctrl + G / Shift + Cmd + G** : Consente, una volta
  effettuata una specifica ricerca all'interno dell'editor di codice
  HTML, di attivare la funzione "**Passa al precedente**"

- **Shift + Ctrl + F / Cmd + Option + F**: Consente di attivare la
  funzione di "**Cerca e sostituisci**".

- Utilizzando questa combinazione di tasti verrà quindi visualizzato un
  primo campo di input in cui inserire il testo da ricercare (campo
  "Replace")

> Una volta inserito il testo desiderato sarà necessario premere il
> tasto "Invio" in maniera tale da visualizzare un nuovo campo di input
> (campo "With") in cui inserire il nuovo testo che dovrà essere
> sostituito a quello precedentemente ricercato.
>
> Infine premendo nuovamente il taso invio verranno visualizzate tutte
> le possibili opzioni di sostituzione

- **Shift + Ctrl + R / Shift + Cmd + Option + F** : Consente di attivare
  la funzione di "**Cerca e sostituisci tutto**".

- **Alt + F**: Consente di attivare la funzione di ricerca
  "persistente".

> In queste condizioni nel caso in cui il testo ricercato dovesse
> presentare più occorrenze sarà possibile passare all'elemento
> successivo / precedente utilizzando rispettivamente i tasti
> "**Invio**" e "**Shift + Invio**"

- **Alt + G**: Consente di attivare la funzione "**Vai alla linea**".

> Utilizzando questa combinazione di tasti verrà quindi visualizzato un
> campo di input in cui inserire il numero di riga (ed eventualmente
> anche quello di colonna) in corrispondenza del quale spostare il
> cursore

Il check "**Creare il file js**", presente nella parte bassa della
maschera, permette di decidere come il codice javascript personalizzato
dovrà essere inserito all'interno della pagina web.

Nello specifico, selezionando questo parametro tutto il codice
javascript personalizzato verrà inserito, in fase di generazione della
pagina web, all'interno di un apposito file creato automaticamente da
Passweb e denominato **layout-inline_xxx.js**.

Al contrario nel caso in cui il parametro in oggetto non sia stato
selezionato, il codice javascript personalizzato verrà inserito
direttamente all'interno della pagina web (in-line) utilizzando per
questo un apposito tag \<script\> **inserito nella sezione \<Head\> di
tutte le pagine cui verrà applicato il layout in questione.**

> **NOTA BENE:** non racchiudere il codice js inserito all'interno di
> questa sezione in un tag \<script\>. Questo tipo di inclusione verrà
> infatti gestita in automatico da Passweb.

**ATTENZIONE! Nel caso in cui sia stato indicato un layout sia a livello
di Variante che a livello di singola Pagina il codice javascript
personalizzato definito sul layout di Pagina andrà ad accodarsi a quello
eventualmente definito a livello di Variante**

In particolare nel caso in cui si sia deciso di inserire questo codice
in un file esterno (parametro "**Creare il file js**" selezionato) verrà
caricato prima il file javascript generato dal layout definito a livello
di Variante, e dopo quello generato dal layout definito a livello di
pagina.

Allo stesso modo nel caso in cui si sia deciso di gestire questo codice
in-line alla pagina (parametro "**Creare il file js**" deselezionato),
all'interno del apposito tag script verrà inserito prima il javascript
definito sul layout di Variante, e in coda quello definito sul layout di
pagina.

**UTENTI ESPERTI:**

All'interno di questa sezione potranno essere richiamate ed utilizzate
funzioni o metodi javascript definiti all'interno di apposite librerie
incluse nel layout stesso e/o presenti a default sul proprio sito
Passweb.

In alternativa tali funzioni o metodi potranno essere richiamati anche
utilizzando specifici componenti HTML inseriti nelle pagina in oggetto
(in questo caso però il codice javascript inserito all'interno di un
componente HTML dovrà necessariamente essere racchiuso all'interno di un
apposito tag \<script\>).

Per maggiori informazioni relativamente alla gestione del componente
HTML si veda anche la corrispondente sezione di questo manuale.

**NOTA BENE: all'interno del Wizard è disabilitata l'esecuzione di
codice javascript personalizzato.**

Codice scritto in maniera non corretta potrebbe infatti, se eseguito,
compromettere il corretto funzionamento del Wizard stesso. In
conseguenza di ciò l'effettivo risultato di eventuali javascript
personalizzati, gestiti per uno specifico layout, potrà essere
visualizzato solo ed esclusivamente lato Front-end (ossia visitando la
corrispondente pagina del sito)

**NOTA BENE:** per maggiori informazioni relativamente all'associazione
di un layout ad una Variante sito si veda anche la sezione "Live Editing
-- Varianti Sito" di questo manuale.

