# CACHING DEL COMPONENTE



A differenza dei componenti analizzati fino a questo momento tra i
parametri di configurazione del componente Contenitore, come si può
facilmente osservare, non compare il parametro "Disabilita Cache".

Relativamente alla possibilità di mettere o meno in cache un componente
di questo tipo occorre infatti considerare che per come è strutturato e
per quello che è il suo utilizzo, un Contenitore inserito a livello 1
sarà sempre e comunque un componente cachabile e non si potrà mai
decidere di escluderlo dalla cache.

Nel momento in cui dovesse invece essere gestito come componente di
livello maggiore o uguale a 2 (ed essere quindi inserito all'interno di
un altro componente di tipo contenitore) il fatto di metterlo o meno in
cache dipenderà direttamente delle impostazioni settate per il
componente padre.

