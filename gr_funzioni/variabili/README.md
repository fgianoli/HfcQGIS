# Variabili

[Funzionalità](http://nyalldawson.net/2015/12/exploring-variables-in-qgis-2-12-part-1/) introdotta da Nyall Dowson nella QGIS 2.12

Questo gruppo contiene variabili dinamiche relative all'applicazione, al file di progetto e ad altre impostazioni. Significa che alcune funzioni potrebbero non essere disponibili in base al contesto:
* seleziona per espressione ![exp](https://docs.qgis.org/testing/en/_images/mIconExpressionSelect.png)
* calcolatore di campi ![calc](https://docs.qgis.org/testing/en/_images/mActionCalculateField.png)
* geometry generator ![epsilos](https://docs.qgis.org/testing/en/_images/mIconExpression.png)
* proprietà del layer ![mod](https://docs.qgis.org/testing/en/_images/mIconDataDefine.png)
* compositore di stampe ![print](https://docs.qgis.org/testing/en/_images/mActionNewLayout.png)

In QGIS, puoi utilizzare le variabili per memorizzare dati utili con valori ricorrenti (ad esempio il titolo del progetto o il nome completo dell’utente) che possono essere utilizzati nelle espressioni. Le variabili possono essere definite a livello globale dell’applicazione, a livello di progetto, a livello di layer, a livello di composizione e a livello di elemento del compositore. Proprio come le regole CSS a cascata, le variabili possono essere sovrascritte, ad esempio una variabile a livello di progetto sovrascrive le variabili di livello globale di qualsiasi applicazione impostate con lo stesso nome.

Puoi utilizzare queste variabili per creare stringhe di testo o altre espressioni personalizzate utilizzando il carattere @ prima del nome della variabile.

Riguardano:

 Funzione  | Descrizione|applicazione
----------:|:-----------|-----------:
[atlas_feature](atlas_feature.html)|Ritorna la geometria attuale dell'atlante  (come oggetto geometria)|proprietà del layer, geometry generator
[atlas_featureid](atlas_featureid.html)|Ritorna ID della geometria attuale dell'atlante|proprietà del layer, geometry generator
[atlas_featurenumber](atlas_featurenumber.html)|Returns the current atlas feature number in the layout
[atlas_filename](atlas_filename.html)|Returns the current atlas file name
[atlas_geometry](atlas_geometry.html)|Returns the current atlas feature geometry|proprietà del layer, geometry generator
[atlas_layerid](atlas_layerid.html)|Returns the current atlas coverage layer ID
[atlas_layername](atlas_layername.html)|Returns the current atlas coverage layer name
[atlas_pagename](atlas_pagename.html)|Returns the current atlas page name|proprietà del layer, geometry generator
[atlas_totalfeatures](atlas_totalfeatures.html)|Returns the total number of features in atlas
[cluster_color](cluster_color.html)|Returns the color of symbols within a cluster, or NULL if symbols have mixed colors
[cluster_size](cluster_size.html)|Returns the number of symbols contained within a cluster
[geometry_part_count](geometry_part_count.html)|Returns the number of parts in rendered feature’s geometry|proprietà del layer, geometry generator
[geometry_part_num](geometry_part_num.html)|Returns the current geometry part number for feature being rendered|proprietà del layer, geometry generator
[geometry_point_count](geometry_point_count.html)|Returns the number of points in the rendered geometry’s part|proprietà del layer, geometry generator
[geometry_point_num](geometry_point_num.html)|Returns the current point number in the rendered geometry’s part|proprietà del layer, geometry generator
[grid_axis](grid_axis.html)|Returns the current grid annotation axis (eg, ‘x’ for longitude, ‘y’ for latitude)
[grid_number](grid_number.html)|Returns the current grid annotation value
[item_id](item_id.html)|Returns the layout item user ID (not necessarily unique)
[item_uuid](item_uuid.html)|Returns the layout item unique ID
[layer](layer.html)|Returns the current layer|Calcolatore di campi,Seleziona per espressione,proprietà del layer, geometry generator
[layer_id](layer_id.html)|Returns the ID of current layer|Calcolatore di campi,Seleziona per espressione,proprietà del layer, geometry generator
[layer_name](layer_name.html)|Returns the name of current layer,proprietà del layer, geometry generator
[layout_dpi](layout_dpi.html)|Returns the composition resolution (DPI)
[layout_name](layout_name.html)|Returns the layout name|Calcolatore di campi,Seleziona per espressione
[layout_numpages](layout_numpages.html)|Returns the number of pages in the layout
[layout_page](layout_page.html)|Returns the page number of the current item in the layout
[layout_pageheight](layout_pageheight.html)|Returns the active page height in the layout (in mm)
[layout_pagewidth](layout_pagewidth.html)|Returns the active page width in the layout (in mm)
[map_crs](map_crs.html)|Returns the Coordinate reference system of the current map|proprietà del layer, geometry generator
[map_crs_definition](map_crs_definition.html)|Returns the full definition of the Coordinate reference system of the current map|proprietà del layer, geometry generator
[map_extent](map_extent.html)|Returns the geometry representing the current extent of the map|proprietà del layer, geometry generator
[map_extent_center](map_extent_center.html)|Returns the point feature at the center of the map|proprietà del layer, geometry generator
[map_extent_height](map_extent_height.html)|Returns the current height of the map|proprietà del layer, geometry generator
[map_extent_width](map_extent_width.html)|Returns the current width of the map|proprietà del layer, geometry generator
[map_id](map_id.html)|Returns the ID of current map destination. This will be ‘canvas’ for canvas renders, and the item ID for layout map renders|proprietà del layer, geometry generator
[map_rotation](map_rotation.html)|Returns the current rotation of the map|proprietà del layer, geometry generator
[map_scale](map_scale.html)|Returns the current scale of the map|proprietà del layer, geometry generator
[map_units](map_units.html)|Returns the units of map measurements|proprietà del layer, geometry generator
[parent](parent.html)|Returns attributes and geometry from the parent feature when in the filter of the “aggregate” expression function
[project_abstract](project_abstract.html)|Returns the project abstract, taken from project metadata
[project_author](project_author.html)|Returns the project author, taken from project metadata
[project_creation_date](project_creation_datemd)|Returns the project creation date, taken from project metadata
[project_identifier](project_identifier.html)|Returns the project identifier, taken from project metadata
[project_keywords](project_keywords.html)|Returns the project keywords, taken from project metadata
[project_crs](project_crs.html)|Returns the Coordinate reference system of the project|Calcolatore di campi,Seleziona per espressione, proprietà del layer, geometry generator
[project_crs_definition](project_crs_definition.html)|Returns the full definition of the Coordinate reference system of the project|Calcolatore di campi,Seleziona per espressione|proprietà del layer, geometry generator
[project_filename](project_filename.html)|Returns the filename of current project|Calcolatore di campi,Seleziona per espressione, proprietà del layer, geometry generator
[project_folder](project_folder.html)|Returns the folder for current project|Calcolatore di campi,Seleziona per espressione, proprietà del layer, geometry generator
[project_path](project_path.html)|Returns the full path (including file name) of current project|Calcolatore di campi,Seleziona per espressione, proprietà del layer, geometry generator
[project_title](project_title.html)|Returns the title of current project|Calcolatore di campi,Seleziona per espressione, proprietà del layer, geometry generator
[qgis_locale](qgis_locale.html)|Returns the current language of QGIS|Calcolatore di campi,Seleziona per espressione, proprietà del layer, geometry generator
[qgis_os_name](qgis_os_name.html)|Returns the current Operating system name, eg ‘windows’, ‘linux’ or ‘osx’|Calcolatore di campi,Seleziona per espressione, proprietà del layer, geometry generator
[qgis_platform](qgis_platform.html)|Returns QGIS platform, eg ‘desktop’ or ‘server’|Calcolatore di campi,Seleziona per espressione, proprietà del layer, geometry generator
[qgis_release_name](qgis_release_name.html)|Returns current QGIS release name|Calcolatore di campi,Seleziona per espressione, proprietà del layer, geometry generator
[qgis_short_version](qgis_short_version.html)|Returns current QGIS version short string|Calcolatore di campi,Seleziona per espressione, proprietà del layer, geometry generator
[qgis_version](qgis_version.html)|Returns current QGIS version string|Calcolatore di campi,Seleziona per espressione, proprietà del layer, geometry generator
[qgis_version_no](qgis_version_no.html)|Returns current QGIS version number|Calcolatore di campi,Seleziona per espressione, proprietà del layer, geometry generator
[snapping_results](snapping_results.html)|Gives access to snapping results while digitizing a feature (only available in add feature)
[symbol_angle](symbol_angle.html)|Returns the angle of the symbol used to render the feature (valid for marker symbols only)|proprietà del layer, geometry generator
[symbol_color](symbol_color.html)|Returns the color of the symbol used to render the feature|proprietà del layer, geometry generator
[user_account_name](user_account_name.html)|Returns the current user’s operating system account name|Calcolatore di campi,Seleziona per espressione|proprietà del layer, geometry generator
[user_full_name](user_full_name.html)|Returns the current user’s operating system user name|Calcolatore di campi,Seleziona per espressione, proprietà del layer, geometry generator
[row_number](row_number.html)|Memorizza il numero della riga corrente|calcolatore campi
[value](value.html)|Returns the current value
[with_variable](with_variable.html)|Allows setting a variable for usage within an expression and avoid recalculating the same value repeatedly

Gruppo sul calcolatore di campi,Seleziona per espressione
![](/img/variabili/gruppo_variabili1.png)

Geometry generator - stile ![epsilos](https://docs.qgis.org/testing/en/_images/mIconExpression.png)
![](/img/variabili/gruppo_variabili2.png)

Selezione per espressione ![exp](https://docs.qgis.org/testing/en/_images/mIconExpressionSelect.png)
![](/img/variabili/gruppo_variabili3.png)

Calcolatore di campi,Seleziona per espressione ![calc](https://docs.qgis.org/testing/en/_images/mActionCalculateField.png)
![](/img/variabili/gruppo_variabili4.png)

Compositore di stampe ![print](https://docs.qgis.org/testing/en/_images/mActionNewLayout.png)
![](/img/variabili/gruppo_variabili5.png)
