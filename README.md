Schritte zur Verortung der Scanner im Gelände:

    1.  Sichtbarkeitsindex der Gebiet mit dem QGIS-Plugin Visibility analysis kalkulieren, Digitales Geländemodel mit Auflösung 10m, Quelle: https://www.data.gv.at/katalog/dataset/d88a1246-9684-480b-a480-ff63286b35b7
    
    2. ZWei Positionen für den Scanner bestimmen – eine Zentral beim Teich und eine mit hohem Sichtbarkeitsindex
    
    3. Scanner-Standorte Sichtbarkeitspunkte mit 2m Höhe und 3000m Radius machen, QGIS-Plugin Visibility analysis -> Create viewpoints
    
    4. Koordinaten zu den Punkten eingeben über QGIS Vector geometry tool -> Add geometry (für x, y coords). Höhe mit dem DGM bestimmen über QGIS Raster analysis tool -> Sample raster values 
       
    5. Erstellung von 30 zufälligen Sichtbarkeitspunkten über QGIS Vector -> Research Tools -> Random points in extent
    
    6. Koordinaten zu den 30 zufälligen Sichtbarkeitspunkten eingeben über QGIS Vector geometry tool -> Add geometry (für x, y coords). Höhe mit dem DGM bestimmen über QGIS Raster analysis tool -> Sample raster values
       
    6. Erstellung von Sichtbarkeitsnetzwerk zwischen den Scanner und den zufälligen Sichtbarkeitspunkten über QGIS-Plugin Visibility analysis -> Intervisibility Network
       
    7. Bestimmung der Reflektoren über QGIS Vector -> Research Tools -> REgular Network mit Abstand zwischen Punkten 300 m
       
    8. Erstellung der Datenbank über QGIS Database tool -> Package Layers tool -> select all files as a geopackage
       Die Datenbank Datei befindet sich im Ordner geopackage/vector_geopackage.gpkg
