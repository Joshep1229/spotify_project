# spotify_project

Éste proyecto contiene una solución end to end **en la nube** para ejecutar python desde la extracción hasta la visualización y el modelo de recomendación.

Para mayor detalle, se puede revisar el código o el trabajo escrito.

Flujo en la nube
1. Cargar Información desde la app de spotify.
2. Preprocesarla y generar cuatro datasets (Artistas, canciones, género y datos de modelo.)
3. Procesar modelo de recomendaciones y guardarlo como un csv (Recomendaciones)
3. Guardar los dataset como formato .csv a un bucket en GCP
4. Cargar el archivo de csv a la base de datos en bigquery.
5. Conectar Google Datastudio (Visualizador) a Google Bigquery. 
6. Visualizar los resultados en Google datastudio para visualizar la información de los datos, más el modelo de recomendación.
