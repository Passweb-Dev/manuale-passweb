# COME EVIDENZIARE ARTICOLI INSERITI IN CARRELLO / WISHLIST



Nel caso in cui si desideri evidenziare, tra tutti gli articoli presenti
all'interno del componente, quelli già inseriti in carrello / wishlist è
possibile intervenire direttamente dallo style editor del componente
agendo sugli elementi

**Catalogo - Cella Articolo in Carrello**

**Catalogo - Cella hover Articolo in Carrello**

**Catalogo -- Cella Articolo in Wishlist**

**Catalogo -- Cella hover Articolo in Wishlist**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\cella_articoli_in_carrello_1_res.bmp](./assets/media/image15.png)

In questo modo sarà quindi possibile, ad esempio, utilizzare per le
celle degli articoli già aggiunti in carrello / wishlist un'immagine di
sfondo diversa da quella normalmente utilizzata per questi elementi.

Volendo potrebbe anche essere possibile utilizzare per questi articoli
un font o un colore del testo diverso da quello utilizzato per gli
articoli non ancora inseriti in carrello / wishlist. **In questo caso
però occorre sempre ricordare che le impostazioni grafiche vengo date a
livello di "Cella Articolo" e non a livello di singoli componenti
presenti all'interno della cella.**

In queste condizioni dunque, nel caso in cui i componenti interni alla
cella siano stati formattati in un certo modo (indicando, ad esempio,
per essi uno specifico colore del testo), le impostazioni grafiche del
singolo componente interno alla cella avranno sempre priorità sulle
stesse impostazioni grafiche settate a livello di "Cella Articolo".

Sfruttando le potenzialità offerte da Passweb a livello di layout di
pagina e codice CSS, potrebbe anche essere possibile marcare le celle
degli articoli inseriti in carrello facendo in modo di visualizzare al
loro interno un' immagine che in condizioni normali (articolo non ancora
inserito in carrello) non viene invece visualizzata.

In questo senso può essere utile evidenziare che nel momento in cui un
determinato articolo dovesse già essere inserito in Carrello / Wishlist
la relativa cella assumerà la seguente classe CSS:

- **incart:** classe CSS presente nelle celle degli articoli già
  aggiunti in Carrello

- **inwishlist:** classe CSS presente nelle celle degli articoli già
  aggiunti in Wishlist

