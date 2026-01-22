# ESTENSIONE



Consente di indicare se la tabella MyDB all'interno della quale si trova
il campo che si intende mappare è stata definita come estensione dei
campi Articolo o come estensione dei campi Cliente.

Quanto indicato in corrispondenza di questo parametro deve coincidere
esattamente con l'estensione dichiarata in Mexal per la corrispondente
tabella MyDB (campo **Estensione**)

![](./assets/media/image242.png)

E' possibile selezionare uno dei seguenti valori:

- **Articoli:** in questo caso la tabella MyDB contenente il campo che
  intendiamo mappare dovrà essere un' estensione dei campi articolo.
  Tale opzione andrà quindi selezionata nel momento in cui il campo
  "**Estensione**" della tabella MyDB dovesse essere impostato su uno
  dei seguenti valori:

  - Tutti gli articoli

  - Articoli di tipo merce

  - Articoli valorizzati

  - ...

![](./assets/media/image243.png)

> **ATTENZIONE!** E' necessario fare riferimento sempre alle tipologie
> di articoli effettivamente gestibili all'interno del proprio sito
> Passweb

- **Clienti**: in questo caso la tabella MyDB contenente il campo che
  intendiamo mappare dovrà essere un' estensione dei campi cliente. Tale
  opzione andrà quindi selezionata nel momento in cui il campo
  "**Estensione**" della tabella MyDB dovesse essere impostato su uno
  dei seguenti valori:

  - Clienti e Fornitori

  - Clienti

  - Fornitori

  - ...

![](./assets/media/image244.png)

> **ATTENZIONE!** E' necessario fare riferimento sempre alle tipologie
> di utenti gestiti all'interno del proprio sito Passweb

Infine, nel momento in cui si dovesse tentare di creare un nuovo campo
Passweb appartenente ad una Tabella MyDB per cui è già stato creato un
altro campo, indicando ora per la stessa Tabella una "Estensione"
diversa da quella dichiarata in precedenza, in fase di salvataggio verrà
ritornato un apposito messaggio di errore.

