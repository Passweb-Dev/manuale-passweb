# PUBBLICAZIONE DI ARTICOLI A TAGLIE E COLORI



Come evidenziato nei precedenti capitoli di questo manuale, per
pubblicare articoli a Taglie / Colori, o comunque con elementi varianti,
è necessario innanzitutto predisporre apposite Inserzioni in cui
dovranno essere gestiti i relativi elementi di variazione

A tali Inserzioni andranno poi collegate liste di vendita in cui
potranno essere inseriti solamente Articoli a Taglie / Colori o Articoli
padri di struttura (per maggiori informazioni in merito a queste due
operazioni si veda anche quanto indicato all'interno del capitolo
"*Marketplace -- Altri Marketplace -- Articoli a Taglie / Colori*" di
questo manuale).

Una volta creata anche la lista di vendita l'ultimo passo sarà
ovviamente quello di pubblicare sulla piattaforma terza gli articoli
presenti all'interno della lista stessa

In questo senso il processo di pubblicazione di articoli a taglie /
colori o comunque con un massimo di due elementi varianti, è
sostanzialmente analogo a quello utilizzato per la creazione di una
normale lista di vendita utilizzata per la pubblicazione di semplici
articoli di magazzino.

Ci sono però alcune considerazione di fondamentale importanza da fare
che riguardano essenzialmente il modo in cui i vari articoli verranno
poi "raggruppati" sulla piattaforma terza e come viene determinato il
"Nome" ad essi assegnato.

**Dipendentemente da come è stata configurata l'Inserzione utilizzata
per la pubblicazione, l'elemento che consentirà di "raggruppare", nella
piattaforma terza, gli articoli pubblicati sarà il penultimo o il
terzultimo livello della struttura.**

Nello specifico:

- Se i due elementi di variazione nell' Inserzione sono stati impostati
  su "Ultimo Campo Struttura" e "Tabella Taglie" l'elemento che
  consentirà di "raggruppare" i singoli articoli sarà il penultimo campo
  della struttura

- Se i due elementi di variazione nell' Inserzione sono stati impostati
  su "Penultimo Campo Struttura" e "Ultimo Campo Struttura" l'elemento
  che consentirà di raggruppare i singoli articoli sarà il terzultimo
  campo della struttura

Per quel che riguarda invece il nome assegnato ai vari articoli
pubblicati sulla piattaforma terza, questo sarà determinato dal Titolo
utilizzato per quello che in Passweb è l'articolo padre di tutta la
struttura cui verrà aggiunta la descrizione associata, a seconda dei
casi, all'elemento del penultimo o del terzultimo campo della struttura

**[ESEMPIO]{.underline}**

Per comprendere meglio questo aspetto supponiamo di fare riferimento ad
una situazione in cui sia necessario trattare articoli a taglie e colori
configurati su Mexal con una struttura in cui gli ultimi due livelli
sono rappresentati rispettivamente dalla "Marca" e dal "Colore".

![Videate\\marketplace_strutture_es1.bmp](./assets/media/image506.png)

Le taglie sono invece gestite mediante la relativa tabella Mexal.

Supponiamo inoltre di aver codificato ed esportato all'interno del sito
Passweb, in relazione al padre di struttura FNU04 i seguenti articoli
figlio

- FNU04NIKNER

- FNU04NIKROS

- FNU04ADIGRI

![](./assets/media/image507.png)

Supponiamo infine di aver personalizzato, in Passweb, i possibili valori
assunti dal penultimo livello della struttura (NIK e ADI)
rispettivamente con le stringhe "Nike" e "Adidas"

![](./assets/media/image508.png)

In queste condizioni, posto di aver configurato correttamente (secondo
quanto indicato nei precedenti capitoli) l'Inserzione da utilizzare per
la pubblicazione dei prodotti , tentando di aggiungere articoli alla
Lista di Vendita troveremo ora tra le possibili scelte l'articolo padre
FNU04

![](./assets/media/image509.png)

Selezionando questo articolo e inserendolo nella Lista di Vendita
Passweb prenderà in considerazione i soli articoli figlio ad esso
relativi effettivamente esportati e gestiti all'interno del sito (quindi
i tre precedentemente indicati) e, in relazione ad ognuno di essi, andrà
ad inserire in lista un elemento per ogni taglia indicata nella
corrispondente tabella Mexal.

![](./assets/media/image510.png)

A questo punto sarà quindi possibile selezionare gli articoli presenti
in lista e pubblicarli sul Merchant Center di Google.

Il Titolo ad essi assegnato sarà costruito prendendo il Titolo di quello
che in Passweb è l'articolo padre (FNU04) cui verrà aggiunta la
descrizione associata, per i relativi figli, al penultimo campo della
struttura

Nel caso considerato dunque, a tutte le taglie degli articoli
FNU04NIKNER e FNU04NIKROS verrà assegnato:

- il **titolo** "Felpa Elite Performance -- NIKE"

![](./assets/media/image511.png)

- lo stesso valore per l'attributo "**identificatore di gruppo**" in
  maniera tale da poter raggruppare tra loro tutti i colori e le taglie
  della felpa di marca NIKE

![](./assets/media/image512.png)

Allo stesso modo, a tutte le taglie dell'articolo FNU04ADIGRI verrà
assegnato

- il **titolo** "Felpa Elite Performance -- ADIDAS"

![](./assets/media/image513.png)

- uno stesso valore per l'attributo "**identificatore di gruppo**"
  (diverso ovviamente da quello assegnato alle taglie e ai colori della
  felpa di marca NIKE) in maniera tale da poter raggruppare tra loro,
  questa volta, tutti i colori e le taglie della felpa di marca ADIDAS

![](./assets/media/image514.png)

