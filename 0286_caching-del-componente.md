# CACHING DEL COMPONENTE



Come per il Contenitore, anche il componente Griglia non ha tra i suoi
parametri di configurazione il "Disabilita Cache".

Anche in questo caso occorre quindi considerare che se inserito a
livello 1, un componente Griglia, sarà sempre e comunque un componente
cachabile e non si potrà mai decidere di escluderlo dalla cache.

Nel momento in cui dovesse invece essere gestito come componente di
livello maggiore o uguale a 2 (ed essere quindi inserito all'interno di
un altro componente di tipo contenitore) il fatto di metterlo o meno in
cache dipenderà direttamente delle impostazioni settate per il
componente padre.

