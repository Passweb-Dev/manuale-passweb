# HEADER



L'elemento \< header \> **identifica un gruppo di informazioni
introduttive che fungono da intestazione ad una determinata sezione
della pagina web**.

La prima cosa che può venir in mente in questo senso riguarda
l'intestazione del sito con la conseguente necessità di inserire
all'interno di questo tag elementi quali il logo e/o il nome del sito.

In ogni caso questi tag possono contenere anche più informazioni
rispetto alla sola intestazione della sezione cui fanno riferimento.
Sarebbe ad esempio ragionevole pensare di includere all'interno di
questo tag anche elementi necessari per gestire delle sotto-intestazioni
(da realizzarsi magari con appositi tag h1 h2 ecc...) o altre
informazioni di supporto alla sezione cui l'header in oggetto fa da
intestazione.

![](./assets/media/image7.png)

**E' all'interno di questo elemento che andrebbero quindi inseriti i tag
title h1 e h2 più importanti della pagina.**

Considerando che questo elemento può essere utilmente impiegato per
racchiudere qualsiasi contenuto che abbia un intento introduttivo è
semplice comprendere come sarebbe sbagliato identificare questo tag solo
ed esclusivamente con la "testata" della pagina web.

E' possibile infatti, anzi il più delle volte è necessario, utilizzare
più di un header all'interno di una pagina web, il primo per
rappresentare l'introduzione alla pagina (tipicamente è quello
posizionato in testata), i successivi per introdurre le varie sezioni
presenti all'interno della pagina stessa.

**ATTENZIONE! il tag header non serve per segnare l'inizio di una
sezione (per questo esiste un altro tag semantico) ma per racchiudere la
sua intestazione**

All'interno del tag \< header \>, infine possono anche essere inserite
informazioni di aiuto alla navigazione del sito. E' prassi comune
infatti quella di inserire il menu di navigazione, racchiuso da un
apposito tag nav proprio all'interno di un tag header.

Per poter implementare in Passweb questo tag semantico è necessario
utilizzare un Componente Contenitore impostando, in fase di
configurazione del componente stesso, il parametro "**Tag**" sul valore
"**Header**"

![Videate\\html5_5.bmp](./assets/media/image8.png)

I contenuti introduttivi della sezione andranno quindi inseriti,
mediante gli appositi componenti Passweb, all'interno di questo
contenitore.

