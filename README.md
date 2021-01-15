# 12SquaresCipher
Archivo de excel con macros para encriptar/desencriptar el cifrado de 12 cuadros

Hoja de excel uitlizada para resolver el cifrado llamado "six-squarecipher" propuesto por el usuario ExecutionByFork en puzzling.stackexchange.com, basado en el cifrado original "four-squares" de Delastelle.
Link original: https://puzzling.stackexchange.com/questions/105719/expanding-on-a-classic

Creo que ExecutionByFork lo llamó "six-squarecipher" por que la forma en que el lo propuso veía menos cuadros, pero al trabajarlo completamente la cantidad de cuadros a utilizar es en realidad 12, por eso mismo a este archivo le he puesto "Cifrado de 12 cuadros".

La hoja de excel puede ser utilizada tanto como para encriptar, como para desencriptar, agregando funcionalidades originales encontradas en el cifrado de Delastelle como son: uso de palabras clave para los cuadros 1, 2 y 3, posibilidad de detallar el listado de caracteres y símbolos a utilizar (abecedario original).
Además, permite detallar la rotación a utilizar en cada uno de los ejes de las coordenadas (x, y, z).

El archivo de excel muestra originalmente solo dos hojas: "Config" (donde la magia ocurre) y "Original Statement" que contiene el texto original detallado por el usuario ExecutionByFork.
Se han escondido otras hojas donde se muestra el detalle de trabajo del cifrado, dichas hojas pueden ser fácilmente mostradas al darle "Click derecho / Mostrar" sobre cualquier hoja.
De igual forma, se han protegido las celdas de la hoja "Config" para solo permitir modificar las celdas destinadas para este propósito.

Detalle de uso
--------------
En la hoja Config se pueden detallar los siguientes campos:

Abecedario a utilizar (Celda O2):
Deben ser 27 caracteres. Por ej. pueden ser 26 letras + 1 simbolo, o 27 letras incluyendo la letra Ñ, etc.

Rotación en X, Y y Z (Celdas P3, P4 y P5):
Pueden detallarse la cantidad de veces que se van a rotar los caracteres en el eje X, Y y Z.  Solo puede tomar valores 0, 1 y 2 (ya que solo son 3 caracteres), donde 0 representa que no va efectuarse ninguna rotación.

Clave para Cuadro 1, Cuadro 2 y Cuadro 3 (Celdas O9, O13 y O17):
Se puede detallar una clave a utilizarse para comenzar a llenar los cuadros, si la clave utilizada es menor de 27 caracteres, el sistema va a rellenar los espacios restantes con los caracteres detallados en el abecedario a utilizar.

Texto plano a cifrar (Celda S21)
Texto plano que desea cifrar, sin signos de puntuacion ni espacios, unicamente pueden utilizarse los caracteres detallados en el abecedario a utilizar.  La respuesta cifrada se muestra en la celda S22.

Texto plano a desencriptar (Celda S25)
Texto cifrado a desencriptar.  El texto desencriptado se mostrará en la celda S26.
