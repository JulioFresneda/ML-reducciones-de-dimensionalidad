# Machine Learning - Reducciones de dimensionalidad
Este proyecto va a consistir principalmente en la **comparación de clasificaciones realizadas empleando técnicas de reducción de dimensionalidad**.
Se van a usar las imágenes de caras obtenidas con el método de scikit-learn *fetch_olivetti_faces*.
Con estas imágenes, se van a realizar varias tareas relacionadas con reducciones de dimensionalidad:

   1. Comprimir las imágenes aplicando PCA de manera que se preserve el 95 % de la varianza y mostrar las 8 primeras imágenes originales y descomprimidas. Crear un nuevo dataset con las imágenes comprimidas. ¿Qué número de píxeles quedan al comprimir?
   2. Lo mismo que en 1. usando LDA.
   3.  Dividir los datos en conjunto de entrenamiento y test de manera que el conjunto de test sea un 20 % del total, tanto para los datos originales como para los comprimidos con PCA y LDA. Repasar la documentación de scikit-learn referida a SVM para ver si es conveniente aplicar transformaciones a los datos.
   4. Realizar una afinación de hiperparámetros para LinearSVC y SVC con kernel ’rbf’ para la clasificación de los datos originales, realizando la búsqueda de parámetros como se comentó en las subsecciones 7.4.1 y 7.4.2 (cambiando SVR por SVC). Usar para el parámetro ’cv’ de GridSearchCV el valor 10. Medir los tiempos en milisegundos de las dos ejecuciones de GridSearchCV. Se recomienda usar multiproceso.
   5. Realizar 4. usando los datos comprimidos mediante PCA.
   6. Realizar 4. usando los datos comprimidos mediante LDA.
   7. Comparar los parámetros resultantes para los mejores estimadores obtenidos en 4., 5. y 6. así como sus accuracies y los tiempos de ejecución totales de las búsquedas y la media de las búsquedas de cada GridSearchCV teniendo en cuenta el número de valores de los parámetros en cada GridSearchCV.
