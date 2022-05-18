# Desafío de clasificación de insectos nocturnos

Los insectos nocturnos representan uno de los grupos más diversos de organismos, por lo que es de suma importancia estudiarlos.  Es por ello que un grupo de prestigiosos entomólogos han construido un ecosistema aislado con múltiples especies para poder estudiarlos en mayor detalle. Para este estudio están diseñando un sistema de sensores para poder trackear de forma automática las dinámicas y hábitos de estos insectos.

El objetivo de esté desafio es obtener un modelo que sea capaz de clasificar los tipos de insectos a partir de los datos obtenidos con los sensores.

# Exploración de los datos

En la libreta "data_exploration.ipnyb" es donde se visualizan los datos. En esta libreta se puede ver como los las 3 categorias de insectos a clasificar estan desvalanceadas, y que la distribución de los insectos a lo largo del dia se ve como la mayoria de los avistamientos són entre las 18 y las 23.

# Selección del modelo

Para escoger el modelo se han probado varios modelos. Los modelos que se han probado han sido KNN, CNN, LSTM y Random Forest Classifier. De entre ellos el que obtenia unas métricas mejores era el Random Forest Classifier, por eso motivo se optó por el.

# Preprocesado de los datos y parámetros del modelo elegido

Los datos se separaron en un 70 % para el entrenamiento y 30 % para el test. Debido a que los datos estan desbalanceados se aplicó oversampling a los datos de entrenamiento para intentar compensar el desbalanceo. Una vez preparados los datos se entrenó el Random Forest Classifier con 800 estimadores y una profuncidad máxima de 300.

# Resultados y valoración

