### Reporte bisemanal 16-05-2021
### Autor:  Pablo Cheng Galdamez 
### Carné: B72182 


* ## Resumen de los temas
    * Árboles de decisión, tienden a ser bastante intuitivos
        * Construcción
            * Puede ser multiclase, mientras más, se vuelve *high branching*.
            * Si el dato es continuo, se agrupan en umbrales.
        * Enfoque sistémico, se usa inducción, luego se aplica un algoritmo y se obtiene un modelo resultante. 
        * Típicamente en las hojas quedan las observaciones y en los nodos las preguntas.
        * *Underfit*, el arbol no esta totalmente entrenado
        * *Overfit*, el árbol se termina aprendiendo todo el *dataset*. Ocurren cuando:
            * El *dataset* contiene ruido
            * El *dataset* no tiene muestras representativas
            * Múltiples comparaciones entre tests
        * Ventajas:
            * Siempre de interpretar
            * No es sensible a datos extremos, ni datos faltantes
            * Algoritmos para entrenar eficientes
            * Es posible prevenir overfitting con parámetros
        * Ventajas:
            * Sensible a cambios del *dataset* 
            * Si aumenta el tamaño es difícil de interpretar
            * Tienden a hacer overfit
    
    * Random Forests, se crean varios árboles y se entrenan todos con diferentes porciones del *dataset*(Ya sea selección de atributos o selección de observaciones). Se revisa el promedio de las respuestas de los árboles.
        * *n_estimators*: cantidad de árboles del bosque
        * *bootstrap samples*: Muestra del *dataset* para cada árbol
        * *max_features*: Cantidad de features para el split
            * *max_features* = *n_features*: no hay aleatoriedad.
            * *max_features* = 1: Reduce el overfitting, solo distinguen con un feature.
        * *Clasificación* Cada árbol predice una probabilidad para cada clase.
        * *Regresión*: se promedian todos los árboles.
    * Gradient Boosting, son árboles dispuestos en serie, en la que cada árbol corrige el error anterior. Se caracterizan por ser árboles pequeños. Dado que están apilados, un cambio en algún parámetro puede generar un gran impacto. 
        * Suelen ser más rápidos que los random Forests
        * Robustos en escala de datos
    
    * Estrategias de entrenamiento


        &nbsp;&nbsp;&nbsp;&nbsp;*Train_test_splits*, se denomina a la separación del *dataset* entre entrenamiento y *test*. Existen desventajas dado que todo depende de un solo split, tampoco garantiza que haya representatividad de cada clase. 


        &nbsp;&nbsp;&nbsp;&nbsp;*Cross-validation*, en este caso se crean más *splits* de un *dataset*, y se entrenan mas modelos. Luego se iteran entre los *splits*, una forma conocida es *k-fold*.  Este método sirve tanto para probar diferentes combinaciones de parámetros, o para probar diferentes partes del *dataset*. Para evitar que haya algún tipo de sesgo en los *splits*, hay una variable; *stratified k-fold Cross-validation*. 


        &nbsp;&nbsp;&nbsp;&nbsp;Existe otra variable *leave one out Cross-validation*(LOOCV). Itera sobre el mismo dataset y se usa un pequeña fracción para *test*. Es útil cuando la información es escasa. También está el caso contrario, existe el *shuffle split Cross-validation*, se hacen muchos *splits* y se determina cuántos *splits* se quieren usar para entrenamiento, cuantos para pruebas. Es práctico cuando se tiene mucha información. De igual manera existe su variante estratificada. 
        
        &nbsp;&nbsp;&nbsp;&nbsp;Cuando existen ciertos datos que tienen importancia para unos pero no para los otros, por lo que no siempre se puede realizar de manera aleatoria. Este método es; *Cross-validation with groups*. Eg, usando información de pacientes, no se pueden mezclar los síntomas entre otros pacientes. 








* * *
* ## Comentarios
Me sorprendió como de un mismo método existen tantas variantes. Y como cada variante puede ayudar a resolver un problema en específico. 
* * *
* ## Dudas
No tengo dudas acerca de la materia.
* * *
* ## Posible uso
Su uso en el área, no solo de *big data*, sino también en el aprendizaje de máquina es de crucial importancia. Dado que nos permite tener una gama extensa de métodos y sus usos recomendados. Esto nos permite tener más control con el modelo elegido, y que este corresponda a los datos esperados. 
* * *
* ## Material extra
* * *






