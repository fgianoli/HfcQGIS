## Come aggiungere le coordinate x e y alla tabella attributi

Facciamo un esempio, geopackage con vettore puntuale:

<img src="/img/esempi_uso/add_coord_xy/add_coord1.png">

selezionare il layer (presente nel _Layer Panel_), tasto destro mouse 'Apri tabella attributi' oppure cliccare sull'icona ![icona_tab_attr](https://docs.qgis.org/2.18/it/_images/mActionOpenTable.png) oppure tasto funzione F6

<img src="/img/esempi_uso/add_coord_xy/add_coord2.png">

1. attivare editing;
2. aprire calcolatore di campi ![calc](https://docs.qgis.org/testing/en/_images/mActionCalculateField.png)
3. crea nuoco campo e digittare nome campo **coord_x**;
4. tipo campo uscita Real e lunghezza uscita 13 e 2;
5. cercare la funzione [$x](/gr_funzioni/geometria/funzioni/$x.md);
6. doppio clic sul risultato della ricerca per inserire la funzione;
7. OK per eseguire; verrà aggiunta la colonna coord_x e popolata;

ripere gli stessi passi per la coord_y e usare la funzione [\$y](/gr_funzioni/geometria/funzioni/$y.md):

<img src="/img/esempi_uso/add_coord_xy/add_coord3.png">