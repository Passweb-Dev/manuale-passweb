# CAMPO CAPTCHA (REGISTRAZIONE E PROFILO UTENTE)



Il Componente **"Campo Captcha"**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\campo_captcha_registrazione_res.bmp](./assets/media/image120.png)

consente di inserire all'interno dei form di Registrazione e di Profilo
Utente il captcha (***c**ompletely **a**utomated **p**ublic **T**uring
test to tell **c**omputers and **h**umans **a**part)* ossia un campo di
controllo utile per stabilire con certezza la natura di colui che
compila un Form evitandone quindi la compilazione automatica ad opera di
bot con il solo fine di generare dello Spam.

All'interno di Passweb è possibile attivare:

- Un **campo Captcha classico** che richiederà all' utente di ripetere
  la sequenza di caratteri visualizzata prima di poter confermare il
  form.

![Videate\\recaptcha_7.bmp](./assets/media/image121.png)

- Il **Google Recaptcha** ossia il sistema antispam offerto da Google e
  in grado di semplificare la vita agli utenti del sito grazie al fatto
  che non li costringe più ad interpretare e riscrivere sequenze più o
  meno leggibili di caratteri e/o numeri per poter dimostrare, in fase
  di compilazione di un form, di non essere un bot e li mette quindi
  nelle condizioni di poter procedere rapidamente alla conferma del form
  stesso

![Videate\\recaptcha_1.bmp](./assets/media/image122.png)

Il fatto di avere a disposizione all'interno dei propri form il captcha
classico piuttosto che il Google Recaptcha dipende essenzialmente dalle
impostazioni settate nella sezione "**Google recaptcha**" alla pagina
"*Sito -- Preferenze -- Integrazioni*" del Wizard.

In particolare nel caso in cui sia stata configurata correttamente
l'integrazione con il relativo servizio di Google inserendo il
componente Captcha all'interno di un form questo visualizzerà
automaticamente il Google Recaptcha, in caso contrario verrà invece
sempre visualizzato il campo Captcha classico.

Rilasciando il componente all'interno della pagina si aprirà **la sua
maschera di gestione e configurazione**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\Form_modifica_Campo_Captcha_res.bmp](./assets/media/image123.png)

Il campo è completamente automatizzato, è necessario inserire solo il
nome del campo e l'etichetta che dovrà avere sul sito, a generare il
Captcha penserà Passweb.

**Nome:** permette di inserire un nome per il campo che si sta editando;

**Pubblico (selezionato a default):** consente di impostare la
visibilità del componente lato sito web. Se selezionato il
corrispondente componente verrà correttamente pubblicato e visualizzato
all'interno del sito. Nel caso in cui invece tale parametro non sia
selezionato, il corrispondente componente passerà in modalità "Offline",
sarà quindi visibile all'interno del Wizard, dove potrà essere
normalmente gestito, ma non verrà pubblicato e visualizzato all'interno
del sito.

**Periodo di Pubblicazione:** consente di associare al Componente in
oggetto uno specifico periodo di pubblicazione, definendone l'effettiva
data di pubblicazione e la corrispondente data di oscuramento.

Nel primo dei due campi disponibili occorrerà quindi indicare,
utilizzando l'apposito calendario, la data di inizio pubblicazione. Nel
secondo campo andrà invece specificata la data di fine pubblicazione.

**ATTENZIONE!** Le date indicate all'interno di questi campi verranno
considerate solo ed esclusivamente nel caso in cui il precedente
parametro "Pubblico" sia stato selezionato

**Tab Index:** consente di personalizzare l'ordine di tabulazione del
form assegnando uno specifico numero d'ordine al campo in oggetto. Una
volta assegnato un numero d'ordine ad ogni campo del form sarà poi
possibile spostarsi da un elemento all'altro, utilizzando il tasto "TAB"
e secondo l'ordine di tabulazione impostato.

Nel caso in cui si decida di personalizzare l'ordine di tabulazione
degli elementi del form sarà necessario assegnare uno specifico numero
d'ordine ad ogni singolo campo. In caso contrario il passaggio da un
campo all'altro attraverso il tasto TAB si interromperà in
corrispondenza del campo con l'ultimo numero d'ordine impostato.

Lato accessibilità il consiglio è quello di non definire una navigazione
personalizzata impostando specifici valori per il parametro in oggetto e
lasciare quindi che sia il browser stesso, in base alla struttura della
pagina a definire gli spostamenti tra un campo e l'altro attraverso il
tasto TAB.

**Label (etichetta):** consente di impostare l'etichetta che verrà
visualizzata all'interno del form di registrazione in corrispondenza del
Componente in esame

**Posizionamento dei Campi:** consente di posizionare gli elementi
principali del componente secondo uno schema prestabilito.

Nello specifico, gli elementi soggetti al tipo di posizionamento
impostato mediante questo parametro saranno:

- La label

- Il Controllo (ossia il Campo di input)

- Il Messaggio di errore

E' possibile selezionare uno dei seguenti valori:

- Affiancati a destra

- Affiancati a sinistra

- Affiancati e giustificati

- Affiancati e opposti

- Centrati e affiancati

- Centrati e Incolonnati

- Incolonnati a destra

- Incolonnati a sinistra

- Custom

**ATTENZIONE!** Nel caso in cui si decidesse di utilizzare uno dei
preset presenti in elenco poi il posizionamento degli elementi sarà
esattamente quello indicato e non potrà essere modificato in alcun modo.

**L'opzione Custom consente invece di non applicare nessun preset
particolare.** **In queste condizioni dunque il posizionamento dei vari
elementi potrà essere variato liberamente agendo sulle corrette
proprietà CSS mediante lo style editor di Passweb e/o mediante i
relativi strumenti di editing avanzato.**

**Ordinamento di visualizzazione dei campi:** visualizzato solo nel caso
in cui il precedente parametro non sia stato impostato sul valore
Custom.

Consente di definire l'ordine di visualizzazione degli elementi
principali del componente in esame, permettendo dunque, già in fase di
configurazione del componente stesso di decidere quale elemento dovrà
essere visualizzato prima e quale dopo.

**ATTENZIONE**! Anche in questo caso l'opzione Custom, non attiva nessun
tipo di preset per cui l'ordine di visualizzazione dei rispettivi
elementi potrà essere variato liberamente agendo sulle corrette
proprietà CSS mediante lo style editor di Passweb e/o mediante i
relativi strumenti di editing avanzato.

Il pulsante "**Salva**" nella parte alta della maschera consentirà di
salvare le modifiche apportate al Componente in oggetto.

**NOTA BENE:** per maggiori informazioni relativamente alle sezioni
"**Avanzate e Animazioni**" e "**Protezione**", presenti nella maschera
di gestione e configurazione di tutti i componenti Passweb, si veda
anche il capitolo " Varianti Responsive -- Configurazione Componenti --
Caratteristiche Generali " di questo manuale.

