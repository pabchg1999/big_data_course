### Reporte bisemanal 11-07-2021
### Autor:  Pablo Cheng Galdamez 
### Carné: B72182 
 
 
* ## Resumen 
    * # Clustering

    Es una técnica no supervisada que permite dividir un data set en grupos. El objetivo de separar los datos en grupos, es crear clases que comparten ciertas características y lograr comprender mejor el mundo. Ya sea recuperar información, identificar variaciones en enfermedades, nuevos clientes, rotaciones, etc. 

    Para elaborar un cluster se necesita una métrica de similitud, métrica utilizada para identificar las características en común.  

    ### Tipos de clustering

    * Partitioning methods

    Mutuamente exclusivas, este método tiende a encontrar métodos de forma esférica. Se basa en una métrica de distancia, típicamente en un centro representativo o un medoide. Son efectivos en dataset de tamaño pequeño o mediano. Los algoritmos que existen son k-means, k-modes y k-medoids.

    * Métodos jerárquicos

    Basados en un orden de los elementos. Una vez ordenados los elementos en una específica jerarquía, no se puede reacomodar en otra. Existen varios tipos, entre ellos están los algoritmos, probabilísticos y bayesianos.

    * Métodos basados en densidad

    Se basa en regiones más pobladas, con base a este parámetro se crean clusters. La forma de separarlos no es necesariamente una distancia. Es una de las técnicas más utilizadas por su robustez, hacia los *outliers*. Alguno de estos algoritmos son DBSCAN, OPTICS, DENCLUE

    * Grid-based methods

    Es un método en el que se puede visualizar un dataset de alta dimensionalidad de manera bidimensional. Entre los algoritmos que existen, están STING y CLIQUE.


    ### Evaluación de clusters 
    * *Silhouette*.
    Maximiza la distancia entre clusters y minimiza la distancia dentro de los elementos del cluster. El valor promedio de *Silhouette* puede evidenciar 3 cosas:

        * $$ x \geq  0.5$$ 
        Buena evidencia que existen los clusters
        * $$ 0.25 \leq x <  0.5$$ 
        Evidencia regular de la existencia de clusters.
        * $$ x \leq  0.5$$ 
        Evidencia débil de los clusters.

    ### SOM (*self organizing maps*)

    Está basado en redes neuronales, es un método no supervisado. Su principal uso es para la reducción de dimensionalidad. Para SOM se usa la primera capa externa de la red neuronal 
    Los clusters se forman de acuerdo a cada centroide. El algoritmo se agrupa por una métrica de similitud.

    Primero se busca un punto cualquiera, luego se encuentra el centroide más cerca. Seguidamente se selecciona el vecindario de este centroide, finalmente se ajustan estos puntos(vecindario) para que convergan a los puntos.

    La escogencia del vecindario se hace a partir de una función. Esta función usa una métrica con respecto a un radio.

    Ventajas
    
    * Facilita la interpretación y visualización 
    * Se puede usar SOM para describir la estructura de los datos 
    * Reduce la dimensionalidad

    Desventaja
    * Requiere selección de parámetros(vecindario, tipo de retícula y cantidad de centroides)
    * Carece de una función objetivo específica para diferenciar clusters, lo que dificulta diferenciarlos.

    ### Análisis de flujos de datos
    ## Stream 
    El procesamiento de los datos se hace en tiempo real, y sin almacenar estos. Los datos son de alto volumen y cambio pequeño, denominado *datasets* infinitos.
    Latencia baja 

   
    
* * *
* ## Comentarios

Me interesó la idea del stream, el hecho de poder manejar *datasets* infinitos me parece de gran utilidad.
 
* * *
* ## Dudas
 No tengo dudas.
 
 
* * *
* ## Posible uso
 
* * *
* ## Material extra
* * *
 
 
 



