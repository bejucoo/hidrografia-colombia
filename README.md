# Hidrografía de Colombia
Archivos geoJSON de la hidrografía de Colombia.

Se crearon usando [QGIS v3.32.3-Lima](https://www.qgis.org/en/site/) con datos de [OpenStreetMap](https://www.openstreetmap.org/) descargados de [Geofabrik](https://download.geofabrik.de/south-america/colombia.html) y datos del [DANE](https://www.dane.gov.co/) descargados del [Metabolism of Cities Data Hub](https://data.metabolismofcities.org/library/35646/).

Filtros utilizados: ```'waterway' = ['canal', 'dam', 'ditch', 'dock', 'drain', 'river', 'stream', 'tidal_channel', 'waterfall', 'weir', 'yes']```

Hasta ahora se organizaron tres archivos por cada departamento:

- **Fronteras:** ```departamento_fronteras.geojson```
- **Ríos estrictamente dentro del área de la frontera** creado con la herramienta *Intersection*: ```departamento_rios_Clip.geojson```
- **Ríos con alguna influencia en el área de la frontera** creado con la herramienta *Select by Location*: ```departamento_rios_noClip.geojson```

Por hacer:
- Archivo con polígonos y líneas de otros cuerpos de agua como lagos, lagunas y siénagas.