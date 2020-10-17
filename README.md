# Amgd1

Schritte zur Verortung der Scanner im Gelände

    1.  Sichtbarkeitsindex der Gebiet mit dem QGIS Plugin Visibility analysis kalkulieren, Digitales Geländemodel mit Auflösung 10m 
    2. 2 Positionen für den Scanner bestimmen – eine Zentral beim Teich und eine mit hohem Visibility-Index
    3. make scanner position visibility points with 2m height and 3000m radiud
    4. Add geometry (x, y coords) + sample raster values for elevation
       
    5. Scatter 30 random points for the visibility analysis, make visibility points too, add geom (x, y coords) +sample raster values for elevation
       
    6. create intervisibility network between the scanners and random points
       
    7. Reflektoren – create regular points, add geom (x, y coords) + sample raster values 
       
    8. Database – Package Layers tool, select all files as a geopackage
