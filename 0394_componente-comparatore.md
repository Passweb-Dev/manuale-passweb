# COMPONENTE COMPARATORE



Il Componente **"Comparatore"** **può** **essere inserito solo ed
esclusivamente all'interno delle Pagine Generiche (Pagine Bianche)**

![](./assets/media/image212.png)

e consente di realizzare una tabella di comparazione mediante la quale
poter mettere a confronto tra loro le diverse caratteristiche e le
diverse proprietà degli articoli in essa inseriti.

![](./assets/media/image213.png)

Di base sarà l'utente stesso sul front end del sito a decidere quali
articoli mettere in comparazione, volendo però è anche possibile
preparare dei comparatori preconfigurati in cui è l'amministratore del
sito a decidere esattamente quali prodotti dovranno essere mostrati
all'interno componente in esame.

Il Comparatore, al pari del Catalogo E-commerce, è un componente di tipo
Contenitore per cui sarà possibile specificare esattamente che tipo di
componenti dovranno essere inseriti al suo interno e quali saranno i
campi e gli attributi dei vari articoli che dovranno essere confrontati
tra loro.

Nella prima colonna verrà visualizzata la label degli attributi e/o dei
campi da confrontare; nelle successive colonne, una per ogni articolo
presente all'interno del comparatore, verranno visualizzati invece i
valori di questi stessi attributi.

**NOTA BENE:** Titolo e Immagine articolo non hanno label associate. Si
consiglia quindi di inserire tali componenti come primi elementi della
tabella di comparazione (come nella figura sopra riportata).

Oltre ai campi e agli attributi articolo sarà possibile inserire
all'interno del comparatore anche i componenti "**Disponibilità**",
"**Aggiunta al Carrello**" e "**Aggiunta alla Wishlist**" mediante i
quali poter richiedere, ad esempio, la disponibilità in tempo reale
degli articoli presenti nella tabella di comparazione e/o aggiungere
questi stessi articoli in Carrello o nella Wishlist.

Una cosa importante da tenere sempre in considerazione è che nel momento
in cui il comparatore dovesse essere impostato per consentire agli
utenti del sito di decidere quali articoli mettere a confronto, in fase
di aggiunta verrà applicato un apposito controllo per verificare che i
prodotti inseriti appartengano effettivamente a categorie merceologiche
con associato lo stesso set di attributi e che abbiano quindi lo stesso
tipo di caratteristiche.

In queste condizioni dunque nel momento in cui si dovesse tentare di
mettere a confronto articoli con diversi set di attributi, e quindi con
caratteristiche diverse (come potrebbe avvenire ad esempio per un
televisore e una macchina fotografica) verrà visualizzato un apposito
messaggio di errore e l'articolo con caratteristiche diverse rispetto a
quelle degli articoli già presenti all'interno del comparatore non verrà
inserito.

![](./assets/media/image214.png)

**ATTENZIONE! articoli associati a categorie merceologiche prive di un
set attributi potranno sempre essere aggiunti al Comparatore.**

Lo stesso controllo **NON verrà invece applicato** nel momento in cui
dovesse essere l'amministratore del sito a decidere, direttamente in
fase di configurazione del componente, quali articoli dovranno essere
visualizzati al suo interno.

In queste condizioni sarà dunque l'amministratore del sito a dover porre
attenzione al fatto che gli articoli messi a confronto mediante il
componente in questione abbiano effettivamente le stesse caratteristiche
e gli stessi attributi.

