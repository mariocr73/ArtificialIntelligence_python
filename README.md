**Red Neuronal Convolucional**
Es una red feedforward adaptada para el reconocimiento de imágenes utilizado en nuestro caso debido a la utilización de imágenes en el experimento.  

![Red neuronal convolucional](http://deeplearning.net/tutorial/_images/mylenet.png)
 
Se definen por las siguientes propiedades:  

* Las capas convolucionales aplican una serie de filtros a la entrada. 
* Las capas submuestreo reducen el tamaño de la entrada. 
* Existen múltiples maneras de submuestra, pero los más populares son el pooling máximo, pooling promedio, y pooling estocástico. 
* La última capa de submuestreo (o convolucional) suele estar relacionada con una o más capas totalmente conectadas, la última de las cuales representa los datos de objetivo.
* El entrenamiento se realiza usando propagación hacia atrás modificada, la cual toma en cuenta las capas de submuestreo y actualiza los pesos de filtro convolucional, basándose en todos los valores a los que se aplica dicho filtro.

**La función de Activación**  

La función de activación más utilizada para este tipo de redes neuronales es la llamada ReLu por Rectifier Linear Unit  y consiste en f(x)=max(0,x).

**Capa de submuestro**
Una capa de submuestreo se coloca después de la primera capa convolucional con el fin de disminuir el tamaño de los datos. La operación que se realiza es max-pooling 

**Capa completamente conectada**
3 capas Convolucionales + ReLU + MaxPool | 8 Filtros x Capa
2 capas Fully Connected | 256 Neuronas x Capa
3 salidas: Celular & Vaso & Cara

Se utilizan dos capas completamente conectadas en la parte final de la red, con una unidad en la capa de salida y L-unidades en la capa oculta.
