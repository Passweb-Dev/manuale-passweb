# SECTION



L'elemento \< section \> **identifica una generica sezione della pagina
web**.

Una sezione in questo contesto è un raggruppamento tematico di contenuti
tipicamente corredato da un header e un footer.

Alcuni casi d'uso suggeriti per questo elemento potrebbero essere:

- I capitoli di una guida

- Le diverse sezioni di un componente Tab, Accordion e Slider

- Le varie sezioni di una Home Page che racchiudono contenuti generici e
  non correlati tra loro (es. introduzione, contatti, news ecc ...)

- ...

In generale dunque section dovrebbe essere utilizzato ogni qualvolta si
intenda veicolare del contenuto che richiede una sua specifica
intestazione.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\html5_12.bmp](./assets/media/image12.png){width="3.657638888888889in"
height="1.1513888888888888in"}

**ATTENZIONE!** questo tag non deve essere utilizzato come aggregatore
di stili per contenuti disomogenei. Per queste esigenze è infatti
possibile e consigliato utilizzare il tag div che sappiamo essere privo
di qualsiasi valore semantico

**ATTENZIONE!** Benché le sezioni possano contenere headings di
qualsiasi livello o rank (da 1 a 6) il W3C consiglia l\'uso di h1 o
comunque di un heading correlato al livello di indentazione della
sezione stessa.

Per poter implementare in Passweb questo tag semantico è necessario
utilizzare un Componente Contenitore configurato come nella figura di
seguito riportata:

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\html5_14.bmp](./assets/media/image13.png){width="4.605555555555555in"
height="3.032638888888889in"}

I contenuti della section andranno quindi inseriti, mediante gli
appositi componenti Passweb, all'interno di questo contenitore.

