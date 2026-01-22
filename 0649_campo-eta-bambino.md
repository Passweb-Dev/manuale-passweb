# CAMPO ETA' BAMBINO



Consente all'utente che compila il form di indicare, in relazione alla
specifica camera, l'età del bambino

**ATTENZIONE!** Dovrà essere inserito un campo di questo tipo per
ciascuno dei bambini effettivamente gestiti nella relativa camera

![](./assets/media/image48.png)

**Tipologia di componente Passweb**: Campo di Testo

**PARAMETRI DI CONFIGURAZIONE DEL COMPONENTE**

**Id/Name** = camera1EtaBambino1 -- dove 1 indica che il campo in esame
è relativo alla prima camera e al primo Bambino

![](./assets/media/image49.png)

**Tipo Valore** = Numerico

**Valore minimo e massimo** = da settare coerentemente con l'età
definita per i bambini all'interno del gestionale

**Obbligatorio** = Si

**Condizioni di visibilità: numeroCamere è in 1,2,3... e numeroBambini1
è in 1,2 ...**

**Condizioni di obbligatorietà: numeroCamere è in 1,2,3 ... e
numeroBambini1 è in 1,2 ...**

![](./assets/media/image50.png)

Nell'ipotesi poi il numero massimo di camere gestite all'interno del
form sia 3 e che il numero massimo di bambini per camera sia 2 lo stesso
componente "Età Bambino" dovrà essere inserito per entrambi i bambini
con le seguenti configurazioni:

**[BAMBINO 1]{.underline}**

**Id/Name** = camera1EtaBambino1 -- dove 1 indica che il campo in esame
è relativo alla prima camera e al primo Bambino

**Tipo Valore** = Numerico

**Valore minimo e massimo** = da settare coerentemente con l'età
definita per i bambini all'interno del gestionale

**Obbligatorio** = Si

**Condizioni di visibilità: numeroCamere è in 1,2,3 e numeroBambini1 è
in 1,2**

**Condizioni di obbligatorietà: numeroCamere è in 1,2,3 e numeroBambini1
è in 1,2**

**[BAMBINO 2]{.underline}**

**Id/Name** = camera1EtaBambino2 -- dove 1 indica che il campo in esame
è relativo alla prima camera e 2 al secondo Bambino

**Tipo Valore** = Numerico

**Valore minimo e massimo** = da settare coerentemente con l'età
definita per i bambini all'interno del gestionale

**Obbligatorio** = Si

**Condizioni di visibilità: numeroCamere è in 1,2,3 e numeroBambini1 è
in 2**

**Condizioni di obbligatorietà: numeroCamere è in 1,2,3 e numeroBambini1
è in 2**

Seguendo poi la stessa logica definita per i campi precedenti, anche
quelli che consentono di inserire l'età dei bambini dovranno ovviamente
essere ripetuti, con le corrette configurazione per ogni blocco camere.

Nell'ipotesi poi il numero massimo di camere gestite all'interno del
form sia 3 e che il numero massimo di bambini per camera sia 2 gli
stessi componenti "Età Bambino" dovranno essere inseriti anche per il
blocco camera 2 e per il blocco camera 3 con le seguenti configurazione:

**[BLOCCO CAMERA 2 -- BAMBINO 1]{.underline}**

**Id/Name** = camera2EtaBambino1 -- dove 2 indica che il campo in esame
è relativo alla seconda camera e 1 al primo Bambino

**Tipo Valore** = Numerico

**Valore minimo e massimo** = da settare coerentemente con l'età
definita per i bambini all'interno del gestionale

**Obbligatorio** = Si

**Condizioni di visibilità: numeroCamere è in 2,3 e numeroBambini2 è in
1,2**

**Condizioni di obbligatorietà: numeroCamere è in 2,3 e numeroBambini2 è
in 1,2**

**[BLOCCO CAMERA 2 -- BAMBINO 2]{.underline}**

**Id/Name** = camera2EtaBambino2 -- dove 2 indica che il campo in esame
è relativo alla seconda camera e al secondo Bambino

**Tipo Valore** = Numerico

**Valore minimo e massimo** = da settare coerentemente con l'età
definita per i bambini all'interno del gestionale

**Obbligatorio** = Si

**Condizioni di visibilità: numeroCamere è in 2,3 e numeroBambini2 è in
2**

**Condizioni di obbligatorietà: numeroCamere è in 2,3 e numeroBambini2 è
in 2**

**[BLOCCO CAMERA 3 -- BAMBINO 1]{.underline}**

**Id/Name** = camera3EtaBambino1 -- dove 3 indica che il campo in esame
è relativo alla terza camera e 1 al primo Bambino

**Tipo Valore** = Numerico

**Valore minimo e massimo** = da settare coerentemente con l'età
definita per i bambini all'interno del gestionale

**Obbligatorio** = Si

**Condizioni di visibilità: numeroCamere è in 3 e numeroBambini3 è in
1,2**

**Condizioni di obbligatorietà: numeroCamere è in 3 e numeroBambini3 è
in 1,2**

**[BLOCCO CAMERA 3 -- BAMBINO 2]{.underline}**

**Id/Name** = camera3EtaBambino2 -- dove 3 indica che il campo in esame
è relativo alla terza camera e 2 al secondo Bambino

**Tipo Valore** = Numerico

**Valore minimo e massimo** = da settare coerentemente con l'età
definita per i bambini all'interno del gestionale

**Obbligatorio** = Si

**Condizioni di visibilità: numeroCamere è in 3 e numeroBambini3 è in
2**

**Condizioni di obbligatorietà: numeroCamere è in 3 e numeroBambini3 è
in 2**
