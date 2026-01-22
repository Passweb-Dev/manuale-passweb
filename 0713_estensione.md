# ESTENSIONE



Consente di indicare se la tabella MyDB all'interno della quale si trova
il campo che si intende mappare è stata definita come estensione dei
campi Articolo o come estensione dei campi Cliente.

Quanto indicato in corrispondenza di questo parametro deve coincidere
esattamente con l'estensione dichiarata in Mexal per la corrispondente
tabella MyDB (campo **Estensione**)

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\estensione_tabella_mydb.bmp](./assets/media/image242.png){width="4.486805555555556in"
height="2.532638888888889in"}

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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\estensione_tabella_mydb_1.bmp](./assets/media/image243.png){width="5.532638888888889in"
height="2.8118055555555554in"}

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

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\estensione_tabella_mydb_2.bmp](./assets/media/image244.png){width="5.532638888888889in"
height="2.8118055555555554in"}

> **ATTENZIONE!** E' necessario fare riferimento sempre alle tipologie
> di utenti gestiti all'interno del proprio sito Passweb

Infine, nel momento in cui si dovesse tentare di creare un nuovo campo
Passweb appartenente ad una Tabella MyDB per cui è già stato creato un
altro campo, indicando ora per la stessa Tabella una "Estensione"
diversa da quella dichiarata in precedenza, in fase di salvataggio verrà
ritornato un apposito messaggio di errore.

