# DO NOTHING APPROACH



Questa è sicuramente la soluzione più semplice da implementare in
quanto, di fatto, non prevede particolari accorgimenti oltre a quelli di
cui abbiamo parlato fino a questo momento e che sono necessari, in
generale, per realizzare un sito responsivo.

Il menu di navigazione va collocato, generalmente, in testata alla
pagina web, deve avere una larghezza in percentuale e un'altezza che si
adatti automaticamente al contenuto

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\gr_14.png](./assets/media/image59.png)

In queste condizioni diminuendo l'area di visualizzazione del documento
quello che potrà succedere è che le voci di menu di primo livello,
inizialmente disposte su di un'unica riga shiftino una sotto l'altra
disponendosi dunque su due o più righe (come evidenziato in figura).

**[CONTRO]{.underline}**

- Altezza complessiva variabile -- Considerando che nei dispositivi di
  piccole dimensioni si tende a linearizzare il layout sviluppando il
  sito in verticale, l'altezza degli elementi diventa un aspetto
  fondamentale in relazione all'immediata visualizzazione o meno di
  determinati contenuti. Il fatto che un menu possa disporsi su due o
  più righe, anziché su una soltanto, potrebbe far scorrere verso il
  basso e non rendere quindi immediatamente visibili, altri contenuti
  importanti della pagina

- Difficilmente scalabile -- Aggiungere voci al menu può modificare
  sensibilmente l'altezza complessiva del componente

- Voci difficilmente cliccabili -- Cercando di avvicinare le voci per
  far rientrare il menu all'intero di una singola riga potrebbe rendere
  difficile selezionare con un dito la pagina di destinazione.

**[COME REALIZZARLO NELLE VARIANTI PASSWEB RESPONSIVE]{.underline}**

E' sufficiente utilizzare la normale componentistica di Passweb
(Componente Menu, Componente Paragrafo con link ecc...) prestando
particolare attenzione al fatto di utilizzare delle dimensioni in
percentuale.

Nel caso in cui si decida di utilizzare un Componente "Menu" in fase di
configurazione del componente stesso sarà necessario selezionare
l'opzione "**Flottante Orizzontale**"

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\menu_flottante_orizzontale.bmp](./assets/media/image60.png)

