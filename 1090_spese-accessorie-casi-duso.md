# SPESE ACCESSORIE -- CASI D'USO



Per cercare di comprendere in maniera più chiara la definizione e
l'utilizzo delle spese accessorie si considerino i seguenti esempi:

**[CONDIZIONI GENERALI]{.underline}**

**Utente:** Rossi Mario

**Indirizzo di Spedizione:** Via Gilberto 4, Rimini

**Spedizioni:** Corriere1 (trasporto abituale), Corriere2

**[ARTICOLI IN ORDINE]{.underline}**

  ------------------------------------------------------------------------
  **ARTICOLO**       **CATEGORIA**       **QUANTITA'**    **PREZZO**
  ------------------ ------------------- ---------------- ----------------
  Computer Acer      Computer            1                560€

  Cellulare Samsung  Cellulari           3                620€

  Ferro da Stiro     Piccoli             1                70€
  Roventa            Elettrodomestici                     
  ------------------------------------------------------------------------

**[CASO D'USO 1]{.underline}**

Per il caso d'uso in oggetto verranno considerate le seguenti spese
accessorie

  ----------------------------------------------------------------------------------
   **DESCRIZIONE   **SELEZIONABILE**     **GESTIONE     **SPEDIZIONI     **COSTI
      SPESA**                             COSTI**       ASSOCIATE**   ASSOCIATI ALLA
                                                                         SPESA**
  --------------- ------------------- ---------------- -------------- --------------
    Imballaggio           NO             Sommatoria                    Per l'Italia
                                                                       Costo Fisso\
                                                                          di 5€

   Assicurazione          SI             Sommatoria      Corriere 2    Per l'Italia
                                                                       Costo Fisso\
                                                                          di 10€
  ----------------------------------------------------------------------------------

In queste condizioni nel caso in cui l'utente Rossi Mario effettui un
ordine contenente gli articoli indicati nelle Condizioni generali, in
Conferma Ordine nello step relativo alle spese di spedizione verranno
visualizzate le opzioni:

- Corriere1 🡪 Opzione già selezionata (perché vettore abituale)

- Corriere2

Nella sezione relativa alle spese accessorie verrà inizialmente
visualizzata la sola spesa "Imballaggio" selezionata a default e non
modificabile con il corrispondente valore di 5€

Nel caso in cui l'utente dovesse selezionare come metodo di spedizione
il "Corriere2" allora nella sezione delle spese accessorie oltre alla
spesa relativa all'imballaggio comparirà anche la voce relativa alla
spesa di assicurazione. Tale spesa potrà essere o meno selezionata
dall'utente e avrà il corrispondente valore di 10€

**[CASO D'USO 2]{.underline}**

Per il caso d'uso in oggetto verranno considerate le seguenti spese
accessorie

+-----------------+-------------------+--------------+-----------------+----------------------------+
| **DESCRIZIONE** | **SELEZIONABILE** | **GESTIONE** | **SPEDIZIONI    | **COSTI ASSOCIATI ALLA     |
|                 |                   |              | ASSOCIATE**     | SPESA**                    |
+:===============:+:=================:+:============:+:===============:+============================+
| Assicurazione   | Sì                | Sommatoria   | [/]{.underline} | [Per Articoli della        |
|                 |                   |              |                 | Categoria                  |
|                 |                   |              |                 | COMPUTER]{.underline}:     |
|                 |                   |              |                 |                            |
|                 |                   |              |                 | Costo Tabellare            |
|                 |                   |              |                 | sull'Italia con i seguenti |
|                 |                   |              |                 | Scaglioni definiti in base |
|                 |                   |              |                 | al numero Articoli in      |
|                 |                   |              |                 | ordine                     |
|                 |                   |              |                 |                            |
|                 |                   |              |                 |   ---------------------    |
|                 |                   |              |                 |   **FINO   **VALORE**      |
|                 |                   |              |                 |   A**                      |
|                 |                   |              |                 |   -------- ------------    |
|                 |                   |              |                 |   2        5€              |
|                 |                   |              |                 |                            |
|                 |                   |              |                 |   OLTRE    10€             |
|                 |                   |              |                 |   ---------------------    |
|                 |                   |              |                 |                            |
|                 |                   |              |                 | [Per Articoli della        |
|                 |                   |              |                 | Categoria                  |
|                 |                   |              |                 | CELLULARI]{.underline}:    |
|                 |                   |              |                 |                            |
|                 |                   |              |                 | Costo Tabellare            |
|                 |                   |              |                 | sull'Italia con i seguenti |
|                 |                   |              |                 | Scaglioni definiti in base |
|                 |                   |              |                 | al numero Articoli in      |
|                 |                   |              |                 | ordine                     |
|                 |                   |              |                 |                            |
|                 |                   |              |                 |   ---------------------    |
|                 |                   |              |                 |   **FINO   **VALORE**      |
|                 |                   |              |                 |   A**                      |
|                 |                   |              |                 |   -------- ------------    |
|                 |                   |              |                 |   8        6€              |
|                 |                   |              |                 |                            |
|                 |                   |              |                 |   OLTRE    15€             |
|                 |                   |              |                 |   ---------------------    |
+-----------------+-------------------+--------------+-----------------+----------------------------+

In queste condizioni nel caso in cui l'utente Rossi Mario effettui un
ordine contenente gli articoli indicati nelle Condizioni Generali nello
step relativo alle spese di trasporto comparirà anche la sezione delle
spese accessorie con indicata la spesa di Assicurazione, liberamente
selezionabile dall'utente, e con importo pari a 11€.

Tale importo sarà determinato dalla somma tra il costo relativo ai
Computer presenti in Ordine (1Articolo 🡪 Scaglione "Fino a 2" 🡪Importo
5€) e quello relativo ai Cellulari presenti nello stesso ordine (3
Articoli 🡪 Scaglione "Fino a 8" 🡪 Importo 6€)

**Assicurazione: 5€+6€ = 11€**

**[CASO D'USO 3]{.underline}**

Per il caso d'uso in oggetto verranno considerate le seguenti spese
accessorie

+-----------------+-------------------+--------------+--------------+---------------------------+
| **DESCRIZIONE** | **SELEZIONABILE** | **GESTIONE** | **SPEDIZIONI | **COSTI ASSOCIATI ALLA    |
|                 |                   |              | ASSOCIATE**  | SPESA**                   |
+:===============:+:=================:+:============:+:============:+===========================+
| Assicurazione   | Sì                | Sommatoria   | /            | [Per Articoli della       |
|                 |                   |              |              | Categoria                 |
|                 |                   |              |              | COMPUTER]{.underline}:    |
|                 |                   |              |              |                           |
|                 |                   |              |              | **Limite Minimo = 5€**    |
|                 |                   |              |              |                           |
|                 |                   |              |              | **Limite Massimo = 10€**  |
|                 |                   |              |              |                           |
|                 |                   |              |              | Costo Tabellare           |
|                 |                   |              |              | sull'Italia con i         |
|                 |                   |              |              | seguenti Scaglioni        |
|                 |                   |              |              | definiti in base al       |
|                 |                   |              |              | numero Articoli in ordine |
|                 |                   |              |              |                           |
|                 |                   |              |              |   ---------------------   |
|                 |                   |              |              |   **FINO   **VALORE**     |
|                 |                   |              |              |   A**                     |
|                 |                   |              |              |   -------- ------------   |
|                 |                   |              |              |   10       5€             |
|                 |                   |              |              |                           |
|                 |                   |              |              |   OLTRE    10€            |
|                 |                   |              |              |   ---------------------   |
|                 |                   |              |              |                           |
|                 |                   |              |              | [Per Articoli della       |
|                 |                   |              |              | Categoria                 |
|                 |                   |              |              | CELLULARI:]{.underline}   |
|                 |                   |              |              |                           |
|                 |                   |              |              | **Limite Minimo = 2€**    |
|                 |                   |              |              |                           |
|                 |                   |              |              | **Limite Massimo = 4€**   |
|                 |                   |              |              |                           |
|                 |                   |              |              | Costo Tabellare           |
|                 |                   |              |              | sull'Italia con i         |
|                 |                   |              |              | seguenti Scaglioni        |
|                 |                   |              |              | definiti in base al       |
|                 |                   |              |              | numero Articoli in ordine |
|                 |                   |              |              |                           |
|                 |                   |              |              |   ---------------------   |
|                 |                   |              |              |   **FINO   **VALORE**     |
|                 |                   |              |              |   A**                     |
|                 |                   |              |              |   -------- ------------   |
|                 |                   |              |              |   10       6€             |
|                 |                   |              |              |                           |
|                 |                   |              |              |   OLTRE    12€            |
|                 |                   |              |              |   ---------------------   |
+-----------------+-------------------+--------------+--------------+---------------------------+

In queste condizioni nel caso in cui l'utente Rossi Mario effettui un
ordine contenente gli articoli indicati nelle Condizioni Generali nello
step relativo alle spese di trasporto comparirà anche la sezione delle
spese accessorie con indicata la spesa di Assicurazione, liberamente
selezionabile dall'utente, e con importo pari A 9€.

Tale importo sarà determinato dalla somma tra il costo relativo ai
Computer presenti in Ordine (1Articolo 🡪 Scaglione "Fino a 10" 🡪Importo
5€) e quello relativo ai Cellulari presenti nello stesso ordine (3
Articoli 🡪 Scaglione "Fino a 10" 🡪 Importo 6€ \> Limite Massimo).

**In particolare per quel che riguarda i Cellulari in ordine in queste
condizioni verrà applicato il Limite Massimo di 4€**

**Assicurazione: 5€+4€ = 9€**

**[CASO D'USO 4]{.underline}**

Per il caso d'uso in oggetto verranno considerate le seguenti spese
accessorie

+-----------------+-------------------+--------------+--------------+---------------------------+
| **DESCRIZIONE** | **SELEZIONABILE** | **GESTIONE** | **SPEDIZIONI | **COSTI ASSOCIATI ALLA    |
|                 |                   |              | ASSOCIATE**  | SPESA**                   |
+:===============:+:=================:+:============:+:============:+===========================+
| Assicurazione   | Sì                | Minimo       | /            | [Per Articoli della       |
|                 |                   | Limite       |              | Categoria                 |
|                 |                   | Massimo o    |              | COMPUTER]{.underline}:    |
|                 |                   | Sommatoria   |              |                           |
|                 |                   |              |              | **Limite Minimo = 5€**    |
|                 |                   |              |              |                           |
|                 |                   |              |              | **Limite Massimo = 10€**  |
|                 |                   |              |              |                           |
|                 |                   |              |              | Costo Tabellare           |
|                 |                   |              |              | sull'Italia con i         |
|                 |                   |              |              | seguenti Scaglioni        |
|                 |                   |              |              | definiti in base al       |
|                 |                   |              |              | numero Articoli in ordine |
|                 |                   |              |              |                           |
|                 |                   |              |              |   ---------------------   |
|                 |                   |              |              |   **FINO   **VALORE**     |
|                 |                   |              |              |   A**                     |
|                 |                   |              |              |   -------- ------------   |
|                 |                   |              |              |   10       5€             |
|                 |                   |              |              |                           |
|                 |                   |              |              |   OLTRE    10€            |
|                 |                   |              |              |   ---------------------   |
|                 |                   |              |              |                           |
|                 |                   |              |              | [Per Articoli della       |
|                 |                   |              |              | Categoria                 |
|                 |                   |              |              | CELLULARI:]{.underline}   |
|                 |                   |              |              |                           |
|                 |                   |              |              | **Limite Minimo = 2€**    |
|                 |                   |              |              |                           |
|                 |                   |              |              | **Limite Massimo = 4€**   |
|                 |                   |              |              |                           |
|                 |                   |              |              | Costo Tabellare           |
|                 |                   |              |              | sull'Italia con i         |
|                 |                   |              |              | seguenti Scaglioni        |
|                 |                   |              |              | definiti in base al       |
|                 |                   |              |              | numero Articoli in ordine |
|                 |                   |              |              |                           |
|                 |                   |              |              |   ---------------------   |
|                 |                   |              |              |   **FINO   **VALORE**     |
|                 |                   |              |              |   A**                     |
|                 |                   |              |              |   -------- ------------   |
|                 |                   |              |              |   10       6€             |
|                 |                   |              |              |                           |
|                 |                   |              |              |   OLTRE    12€            |
|                 |                   |              |              |   ---------------------   |
+-----------------+-------------------+--------------+--------------+---------------------------+

In queste condizioni pur essendo variato il metodo di calcolo dei costi
associati alla spesa accessoria in oggetto si ottiene esattamente lo
stesso risultato del caso precedente. Considerando infatti che solo uno
dei due costi associati alla spesa supera il proprio limite massimo
verrà comunque considerata la sommatoria dei singoli costi.

**Assicurazione: 5€+4€ = 9€**

**[CASO D'USO 5]{.underline}**

Per il caso d'uso in oggetto verrà considerato il seguente ordine

  ------------------------------------------------------------------------
  **ARTICOLO**       **CATEGORIA**       **QUANTITA'**    **PREZZO**
  ------------------ ------------------- ---------------- ----------------
  Computer Acer      Computer            2                560€

  Cellulare Samsung  Cellulari           3                620€

  Ferro da Stiro     Piccoli             1                70€
  Roventa            Elettrodomestici                     
  ------------------------------------------------------------------------

Verranno inoltre considerate le seguenti spese accessorie

+-----------------+-------------------+--------------+--------------+---------------------------+
| **DESCRIZIONE** | **SELEZIONABILE** | **GESTIONE** | **SPEDIZIONI | **COSTI ASSOCIATI ALLA    |
|                 |                   |              | ASSOCIATE**  | SPESA**                   |
+:===============:+:=================:+:============:+:============:+===========================+
| Assicurazione   | Sì                | Minimo       | /            | [Per Articoli della       |
|                 |                   | Limite       |              | Categoria                 |
|                 |                   | Massimo o    |              | COMPUTER]{.underline}:    |
|                 |                   | Sommatoria   |              |                           |
|                 |                   |              |              | **Limite Minimo = 5€**    |
|                 |                   |              |              |                           |
|                 |                   |              |              | **Limite Massimo = 10€**  |
|                 |                   |              |              |                           |
|                 |                   |              |              | Costo Tabellare           |
|                 |                   |              |              | sull'Italia con i         |
|                 |                   |              |              | seguenti Scaglioni        |
|                 |                   |              |              | definiti in base al       |
|                 |                   |              |              | numero Articoli in ordine |
|                 |                   |              |              |                           |
|                 |                   |              |              |   ---------------------   |
|                 |                   |              |              |   **FINO   **VALORE**     |
|                 |                   |              |              |   A**                     |
|                 |                   |              |              |   -------- ------------   |
|                 |                   |              |              |   1        5€             |
|                 |                   |              |              |                           |
|                 |                   |              |              |   OLTRE    10€            |
|                 |                   |              |              |   ---------------------   |
|                 |                   |              |              |                           |
|                 |                   |              |              | [Per Articoli della       |
|                 |                   |              |              | Categoria                 |
|                 |                   |              |              | CELLULARI:]{.underline}   |
|                 |                   |              |              |                           |
|                 |                   |              |              | **Limite Minimo = 2€**    |
|                 |                   |              |              |                           |
|                 |                   |              |              | **Limite Massimo = 4€**   |
|                 |                   |              |              |                           |
|                 |                   |              |              | Costo Tabellare           |
|                 |                   |              |              | sull'Italia con i         |
|                 |                   |              |              | seguenti Scaglioni        |
|                 |                   |              |              | definiti in base al       |
|                 |                   |              |              | numero Articoli in ordine |
|                 |                   |              |              |                           |
|                 |                   |              |              |   ---------------------   |
|                 |                   |              |              |   **FINO   **VALORE**     |
|                 |                   |              |              |   A**                     |
|                 |                   |              |              |   -------- ------------   |
|                 |                   |              |              |   10       6€             |
|                 |                   |              |              |                           |
|                 |                   |              |              |   OLTRE    12€            |
|                 |                   |              |              |   ---------------------   |
+-----------------+-------------------+--------------+--------------+---------------------------+

In queste condizioni nel caso in cui l'utente Rossi Mario effettui un
ordine contenente gli articoli precedentemente indicati, nello step
relativo alle spese di trasporto comparirà anche la sezione delle spese
accessorie con indicata la spesa di Assicurazione, liberamente
selezionabile dall'utente, e con importo pari A 4€.

Questa volta infatti entrambi i costi associati alla spesa accessoria in
esame raggiungono o superano il loro limite massimo per cui considerando
il tipo di gestione dei costi impostata il valore complessivo della
spesa accessoria sarà dato dal più basso dei limiti massimi associati ai
singoli costi.

2 articoli computer 🡪 10€ = MAX 10€

3 articoli cellulari 🡪 6€ = MAX 4€

Il minimo tra i due massimi è 4€.

