# NUMERO



Consente di indicare il numero sequenziale (all'interno della tabella in
esame) del campo MyDB che si intende mappare.

Per individuare tale numero occorre tener conto del fatto che:

- la numerazione dei campi all'interno della tabella MyDB parte da 1

- il primo campo della tabella è sempre il campo chiave ed è
  caratterizzato dal fatto di avere codice zzz

- **il campo chiave della tabella MyDB (quello con codice zzz e
  numerazione = 1) non dovrà mai essere mappato**

In conseguenza di ciò è semplice comprendere come i valori da inserire
all'interno di questo campo dovranno, ovviamente, essere maggiori o
uguali a 2.

Facendo quindi riferimento ad una situazione del tipo di quella
rappresentata in figura

![](./assets/media/image254.png)

e supponendo di voler mappare il campo "Supporto", il valore da inserire
all'interno del campo "Numero" dovrà essere 5

