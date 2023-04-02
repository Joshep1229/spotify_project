# spotify_project

Éste proyecto contiene una solución end to end **en la nube** para ejecutar python desde la extracción hasta la visualización y el modelo de recomendación.

Para mayor detalle, se puede revisar el código o el trabajo escrito.

El flujo completo se ejecuta semanalmente usando el orquestador **Vertex AI**

Flujo en la nube
1. Cargar Información desde la **API de spotify**.
2. Preprocesarla y generar cuatro datasets (Artistas, canciones, género y datos de modelo.)
3. Procesar **modelo de recomendaciones** y guardar los resultados como un csv (Recomendaciones)
3. Guardar los dataset como formato .csv a un **bucket en GCP**. (Previa conexión configurada en el notebook.)
4. Cargar el archivo de csv guardado en el bucket a la base de datos en **Google Bigquery de GCP** (que está en postgres).
5. Conectar la base de datos de Google Bigquery a **Google Datastudio (Visualizador)** 
6. Visualizar los resultados en Google datastudio para visualizar la información.
    6.1 La primera hoja contiene el dashboard.
    6.2 La segunda hoja contiene las recomendaciones generadas por el modelo. 
