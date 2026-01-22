# VISUALIZZAZIONE DELLA DATA E ORA DI ULTIMA SINCRONIZZAZIONE



In relazione all'utilizzo del componente "Disponibilità" potrebbe essere
interessante visualizzare all'interno del sito oltre al pulsante per la
richiesta in tempo reale della disponibilità di un certo articolo e/o al
dato relativo a questo tipo di informazione, anche la data e l'ora cui
questa stessa informazione fa riferimento, data e ora che, come
evidenziato nel precedente capitolo di questo manuale, coincidono con
data e ora di ultima sincronizzazione.

**Per poter visualizzare un'informazione di questo tipo è sufficiente
utilizzare un componente "Paragrafo" o un componente "HTML" inserendo al
suo interno il segnaposto {{SYNCAV}} come evidenziato nella figura di
seguito riportata**

![\\\\doctohelp\\D\\ManPassweb_Ecommerce_Sviluppo\\Videate\\data_ultima_sincronizzazione_res.bmp](./assets/media/image581.png){width="4.638194444444444in"
height="2.9444444444444446in"}

Tale segnaposto verrà poi sostituito in fase di generazione dalla pagina
web con la data e l'ora dell'ultima sincronizzazione terminata
correttamente, dando quindi all'utente del sito un'informazione più
precisa relativamente alla data cui fa riferimento la disponibilità
attualmente visualizzata per un certo articolo.

**ATTENZIONE!** affinchè il segnaposto indicato possa essere sostituito
con la data e l'ora di ultima sincronizzazione è indispensabile che sia
inserito esattamente come indicato. Alterando la struttura di questo
segnaposto esso sarà infatti considerato come del semplice testo.

![\\\\doctohelp\\D\\ManPassweb_Ecommerce\\Videate\\data_ultima_sincronizzazione2.bmp](./assets/media/image582.png){width="5.116666666666666in"
height="3.6319444444444446in"}

Ovviamente l'utente avrebbe sempre la possibilità di utilizzare il
pulsante per aggiornare in tempo reale il valore della disponibilità di
un certo articolo ma, in ogni caso, il dato inizialmente visualizzato è
sempre relativo alla data e ora di ultima sincronizzazione.

**ATTENZIONE! la richiesta della disponibilità in tempo reale aggiorna
il dato relativo alla disponibilità dello specifico articolo ma non
quello relativo alla data e all'ora di ultima sincronizzazione. Tale
dato verrà quindi aggiornato automaticamente solo al termine di una
sincronizzazione sito-gestionale terminata correttamente**

