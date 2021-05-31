### Reporte bisemanal 30-05-2021
### Autor:  Pablo Cheng Galdamez 
### Carné: B72182 


* ## Resumen de los temas
    * Redes neuronales
        * Modelos lineales, buscan aproximar los datos con ayuda de los coeficientes o pesos. Sin embargo, no tiene buen desempeño cuando hay baja dimensionalidad en el *dataset*. Por el contrario funciona bien cuando hay muchas variables. No tienen parámetros, por lo que lo hace sencillo de programar. Para minimizar 

        * Regresión logística
        
            &nbsp;&nbsp;&nbsp;&nbsp; Es una forma de combinar los modelos lineales, quitando la linealidad, con técnicas no lineales. 
        
        * Red Neuronal 

            &nbsp;&nbsp;&nbsp;&nbsp; Investiga como modelos simples pueden resolver problemas computacionales complicados. Lo que se pretende es crear algoritmos robustos capaces de modelar estos problemas. 

            &nbsp;&nbsp;&nbsp;&nbsp; Las ventajas de las redes neurales proviene de su habilidad de aprender del *dataset* y poder relacionar estos datos con los resultados. Una red neuronal se compone de una red de Neuronas. 

            * Neuronas, son unidades que asignan pesos a las entradas y producen una salida correspondiente a su función de activación. La función de activación es un método que mapea los pesos y produce una salida.

            &nbsp;&nbsp;&nbsp;&nbsp; En una red neuronal existen *layers*, o capas, lo cuales son conjuntos de neuronas acomodados en fila. Existen las capa visibles o *input layers*, las ocultas o *hidden layers* y *output layer*. La *input layer* es la primera capa con la que se encuentran los datos de *dataset*, por lo general cada entrada tiene una neurona. Mientras que las *hidden layers* son aquellas otras que no están expuestas. Finalmente están las *output layers*, estas son aquellas que producen la salida de la red neural. 

            &nbsp;&nbsp;&nbsp;&nbsp; Un *output layer* puede variar según el tipo de problema. 
             * *Regression*, en este caso la salida solo es una y la neurona no tiene una función de activación. 

             * Binario, la salida como lo dice es binaria, para este problema se puede usar una función sigmoide.

             * *Multiclass*, aquí se pueden tener múltiples neuronas, una por cada clase. 

            &nbsp;&nbsp;&nbsp;&nbsp;Entre los métodos más comunes para programar una red neuronal está la de *Stochastic Gradient Descent*. Se basa en tener un *input layer* por cada entrada activando las neuronas y finalmente obteniendo una salida. Luego esta salida se compara con la esperada y se calcula el error, para posteriormente ser distribuido por la red neural, así sucesivamente se entrena el modelo. 

            &nbsp;&nbsp;&nbsp;&nbsp; Actualización de pesos, en este método se recalculan los pesos de acuerdo al error, para luego producir una salida 

    * Análisis de asociaciones

        &nbsp;&nbsp;&nbsp;&nbsp;Predicciones acerca de las acciones de un usuario en particular. Esta información es valiosa para diseñar páginas, sugerir navegación, dirigir anuncios, etc. También se pueden detectar fraudes. 

        &nbsp;&nbsp;&nbsp;&nbsp;Existen los itemsets, conjunto de items de cantidad k. Entre mayor sea el valor de confianza, mayo posibilidad es que aparezca en alguna regla. 
         
        &nbsp;&nbsp;&nbsp;&nbsp;Al principio se generan los itemset, para crearlos se empiezan por subconjuntos. Existe el principio a priori, cuando existe algún item x que no es frecuente, se pueden podar todo el superconjunto de x. Luego se hacen reglas con los conjuntos obtenidos. 
         
    
    

* * *
* ## Comentarios
&nbsp;&nbsp;&nbsp;&nbsp;No conocía que hubieran conjuntos y se pudieran predecir de esta manera, lo cual me pareció muy ingenioso. Me parece que tiene un sentido práctico muy útil. 


* * *
* ## Dudas
&nbsp;&nbsp;&nbsp;&nbsp;Me quedó la duda acerca de cómo funcionan los pesos en las neuronas, y el sesgo.
* * *
* ## Posible uso
&nbsp;&nbsp;&nbsp;&nbsp;En la actualidad los conjuntos pueden ser de gran ayuda, dado que cada vez como consumidor se busca la comodidad. Y eso es algo que se puede lograr cuando se tienen predicciones de la compra completa. También del lado del vendedor puede aumentar sus ventas, al sugerir productos que puede que lleven los consumidores, inclusive hacer paquetes aún más llamativos.


* * *
* ## Material extra
* * *








