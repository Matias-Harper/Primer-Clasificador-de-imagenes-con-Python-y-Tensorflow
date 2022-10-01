# Primer-Clasificador-de-imagenes-con-Python-y-Tensorflow
Primer clasificador de imágenes con Python y Tensorflow.

El modelo que tenemos a diferencia del anterior que era de regresión, es de CLASIFICACIÓN.
Recibimos de entrada una imagen y nuestra red tiene que devolver en qué clasificación (de las prefijadas) corresponde.
La pregunta es como ingresar la entrada “imagen” ya que previamente con números podíamos hacerlo más intuitivamente, en este caso pasaremos la imagen a blanco y negro y la dividiremos en píxeles, cada neurona de entrada almacenará un píxel de nuestra imagen de entrada.
Para esto reduciremos la imagen a 28*28 px para tener 784 píxeles totales y 784 neuronas de entrada. Por ende ya sabemos que tendrá 784 neuronas de entrada y 10 de salida (Camiseta, Pantalon, Sueter, Vestido, Saco, Sandalia, Camisa, Tenis, Bolsa, Botin).

¿Qué tipo de red neuronal usar? 
La utilizada generalmente será una Red Neuronal Convolucional, sin embargo consideraremos que no existe, asi que trabajaremos partiendo de una Red Neuronal Densa (nuevamente).

Ya dijimos que esto no será un problema lineal así que deberemos incorporar los conceptos de Capas Ocultas y Funciones de Activación.
Las Capas Ocultas nos aportaran nuevas “perillas” a nuestra consola permitiendo afinar y robustecer nuestro modelo sin embargo sigue buscando una solución lineal aunque las agreguemos (por ej fueron agregadas al problema anterior en el final a modo de prueba)
Para suplir esto utilizaremos las Funciones de Activación, luego de su peso y su sesgo la neurona deberá pasar por la misma. 

Existen muchas Funciones de Activación que no abordaremos en este momento.
A pesar de lo escueto de esta explicación, debemos entender que estas nuevas herramientas le generan a nuestra red posibilidades para resolver problemas complejos.

y cómo entrenamos a nuestra red? 
Utilizaremos un set de imágenes creado por la marca Zalando, donde encontraremos imagenes en blanco y negro de las dimensiones que necesitamos y esta categorizadas como queremos hacerlo (hermoso, asi no fuciona en la vida real jaja). Tendremos 70 mil imágenes.
  
Comencemos en el Google Colab
Arrancaremos con dos capas ocultas de 50 neuronas cada una generando un modelo de 784 neuronas de entrada, 50 capa oculta 1, 50 capa oculta 2 y 10 de salida. (luego agregue más neuronas a las capas intermedias para lograr mejores predicciones)
En el colab se encuentra el código paso a paso 
https://colab.research.google.com/drive/1FcjuflUrXIU2JetfoVZddNbrKWqRhW5c?usp=sharing
