# Lab3 - Ciclo de vida de una aplicación #

## Descripción del problema ##
Para entender el diagrama de estados del ciclo de vida de una activity vamos a crear una aplicación que estará formada por una única actividad en la que sobreescribiremos todos los métodos del ciclo de vida de una aplicación y detectaremos su lanzamiento mediante el uso de Toast.

## GIFs de la aplicación ##

**Lanzamiento de la aplicación**

Al lanzar la aplicación ésta lanza los métodos onCreate(), onStart() y onResume().

<img src="https://dl.dropboxusercontent.com/u/52992573/PGL/Lab3/Lab3_1_001.gif" width="350">

**Pulsamos el botón Home**

Al pulsar el botón Home los métodos que se ejecutan son onPause() y onStop().

<img src="https://dl.dropboxusercontent.com/u/52992573/PGL/Lab3/Lab3_1_002.gif" width="350">

**Relanzamos la aplicación**

Al relanzar la aplicación se ejecutan los métodos onCreate(), onStart() y onResume().

<img src="https://dl.dropboxusercontent.com/u/52992573/PGL/Lab3/Lab3_1_003.gif" width="350">

**Pulsamos el botón Atrás**

Cuando pulsamos el botón Atrás de nuestro dispositivo se ejecutan los métodos onPause(), onStop() y onDestroy().

<img src="https://dl.dropboxusercontent.com/u/52992573/PGL/Lab3/Lab3_1_004.gif" width="350">

**Giramos el dispositivo**

Girando nuestro dispositivo lo que pasa es que la Activitie que tenemos lanzada se cierra y se vuelve a ejecutar, por lo que los métodos que se lanzan son onPause(), onStop(), onDestroy(), onCreate(), onStart() y onResume().

Debido a la particularidad mencionada anteriormente, al girar el dispositivo podemos perder nuestros datos de aplicación si no les asignamos a los elementos de la interfaz identificadores.

Sin ID asignado

<img src="https://dl.dropboxusercontent.com/u/52992573/PGL/Lab3/Lab3_1_005.gif" width="500">

Con ID asignado.

<img src="https://dl.dropboxusercontent.com/u/52992573/PGL/Lab3/Lab3_1_006.gif" width="500">

**Pulsamos el botón Finalizar de nuestra aplicación**

Hemos programado el botón Finalizar con el método finish(). Al pulsarlo se lanzan los métodos onPause(), onStop() y onDestroy().

<img src="https://dl.dropboxusercontent.com/u/52992573/PGL/Lab3/Lab3_1_007.gif" width="350">

