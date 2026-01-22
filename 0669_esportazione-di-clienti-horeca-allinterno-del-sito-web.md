# ESPORTAZIONE DI CLIENTI HO.RE.CA. ALL'INTERNO DEL SITO WEB



Mentre per gli articoli/servizi è possibile definire, attraverso il
corrispondente flag "Abilita Passweb" presente nell'anagrafica Ho.Re.Ca.
di questi stessi articoli/servizi, quali di essi dovranno essere
esportati e gestiti all'interno del sito e quali no, per i clienti già
presenti nella base dati del gestionale non è possibile effettuare
questo tipo di distinzione.

**Alla prima sincronizzazione sito -- gestionale infatti, tutti i
clienti presenti nel gestionale stesso verranno esportati e potranno
essere gestiti anche all'interno del sito.**

> **NOTA BENE:** il fatto di esportare alla prima sincronizzazione dal
> gestionale verso il sito tutti i clienti presenti all'interno del
> gestionale stesso non significa per forza di cose che tutti questi
> clienti potranno poi accedere al sito per effettuare acquisiti e/o
> prenotazioni via web.

**Condizione necessaria per poter accedere al sito ed effettuare quindi
delle prenotazioni e/o degli ordini, è infatti quella di avere assegnato
nella propria anagrafica una specifica login e una specifica password di
accesso al sito.**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\horeca_esportazione_utenti.bmp](./assets/media/image119.png)

In questo senso poi, come per Mexal, è bene sottolineare che per quel
che riguarda la login utente nel caso di:

- **esportazione sul sito di un nuovo utente, già presente tra le
  anagrafiche del gestionale**: prima di effettuare l'esportazione sarà
  ovviamente necessario assegnare un valore al relativo campo e,
  successivamente, comunicarlo all'utente che ne dovrà far uso

- **registrazione web di un nuovo utente**: il dato presente all'interno
  di questo campo verrà inserito alla sincronizzazione direttamente da
  Passweb e coinciderà con quanto indicato dall'utente stesso in fase di
  registrazione al sito

- **variazione dell'anagrafica utente sul sito:** nel momento in cui un
  utente già esportato e gestito all'interno del sito dovesse agire
  dalla pagina del suo profilo per modificare la login di accesso, alla
  successiva sincronizzazione anche il campo "Login Utente" del
  gestionale Ho.Re.Ca. verrà correttamente aggiornato

Per quel che riguarda invece la password di accesso nel caso di:

- **esportazione sul sito di un nuovo utente, già presente tra le
  anagrafiche del gestionale**: come per la login, anche in questo caso
  prima di effettuare l'esportazione sarà necessario assegnare
  all'utente una specifica password e, successivamente, comunicargliela.

> **ATTENZIONE! Una volta arrivata sul sito, per ragioni di privacy, la
> password verrà opportunamente crittografata e, da questo momento in
> avanti, sarà gestita solo ed esclusivamente all'interno del sito**
>
> Ciò significa dunque che nel momento in cui l'utente dovesse andare a
> modificare, dal proprio profilo, la password di accesso al sito, il
> nuovo valore resterà memorizzato, opportunamente crittografato, solo
> sul database di Passweb e NON verrà quindi riportato nel campo
> "Password" del gestionale Ho.Re.Ca.

- **registrazione web di un nuovo utente:** coerentemente con quanto
  indicato per il punto precedente, la password dei nuovi utenti che si
  sono registrati al sito resterà memorizzata, opportunamente
  crittografata, solo sul database di Passweb e NON verrà quindi mai
  riportata nel campo "Password" del gestionale Ho.Re.Ca.

Una volta esportato un cliente, e assegnatogli una login e una password
di accesso, sarà comunque possibile in qualsiasi momento bloccare per
questo stesso utente l'accesso al sito impedendogli quindi di effettuare
nuovi ordini e/o nuove prenotazioni.

Questo può essere fatto in due diversi modi:

a.  Operando direttamente all'interno del gestionale ed utilizzando per
    questo il flag "**Black List**" presente all'interno dell'anagrafica
    del cliente stesso (scheda "**Tessera e Promozioni**")

> **NOTA BENE:** una volta impostato il flag "Black List", per impedire
> al relativo utente l'accesso al sito sarà necessario anche lanciare
> una nuova sincronizzazione in modo tale da consentire a Passweb di
> leggere il nuovo dato

b.  Operando direttamente all'interno del Wizard di Passweb, ed
    utilizzando per questo il flag "**Blocca Accesso al Login**"
    presente nell'anagrafica dello specifico cliente

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\black_list2.bmp](./assets/media/image120.png)

