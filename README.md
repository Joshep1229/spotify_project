
# Spotify Project

**Integrantes**

**Joshep Andersson Blanco Reyes**



Estudiantes de Maestría en Inteligencia Artificial. 

### **Alcance General del proyecto**

 **Éste proyecto contiene una solución end to end en la nube** para ejecutar desde la extracción hasta la visualización y el modelo de recomendación de forma automática usando VertexAI.


## **Link de demostración práctica del flujo. -10 min- [Flujo Youtube](https://youtu.be/52CaeujRUC4)**
## **Link del dashboard y el modelo de recomendación en producción [Google Datastudio](https://lookerstudio.google.com/reporting/86e0b128-1eda-4927-ae03-42a04ea3a4d0).**

## **El código contiene el modelo y el pipeline está Google Collab -Tercera entrega.-,  está explicado paso a paso el flujo que se realizó** (Ver file Pipeline_Spotify.) [Google Collab](https://github.com/Joshep1229/spotify_project/blob/main/Pipeline_Spotify.ipynb)

## **En la carpeta entregas, están todas las entregas realizadas en el semestre** 

**Las playlists usadas fueron el top 50 global, el top 50 Brazil y el top 50 Corea del sur.** Los datos generados y el modelo, se actualizan **semanalmente**.
Esto permite que  el sistema **siempre generará recomendaciones nuevas y personalizadas de las mejores 50 canciones de los 3 países.** Tomando en cuenta las canciones que ingresen o salgan del top.


![alt text](https://github.com/Joshep1229/spotify_project/blob/main/Images/Pipeline%20Grafico.JPG?raw=true)

### **Flujo en la nube**
1. Cargar Información desde la **API de spotify**.
2. Preprocesarla y generar cuatro datasets (Artistas, canciones, género y datos de modelo.)
3. Procesar **modelo de recomendaciones** y guardar los resultados como un csv (Recomendaciones)
3. Guardar los dataset como formato .csv en un **bucket en GCP**. (Previa conexión configurada en el notebook.)
4. Con SQL cargar el archivo de csv guardado en el bucket en la base de datos de **Google Bigquery de GCP** (que está en postgres).
5. Conectar la base de datos de Google Bigquery a **Google Datastudio (Visualizador)** 
6. Visualizar los resultados en Google datastudio para visualizar la información.

    6.1 La primera hoja contiene el dashboard.
    
    6.2 La segunda hoja contiene el modelo de recomendaciones generadas por el modelo.

Para mayor detalle, se puede revisar el código o el trabajo escrito.





	


