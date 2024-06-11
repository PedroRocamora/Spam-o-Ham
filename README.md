# Clasifica entre Spam o Ham usando Deep Learning

## Estructura del repositorio
- `Colab Notebooks/`: Tenemos los 2 cuadernos de Jupyter ClasificadorSpam.ipynb y ExtraeCaracteristicasCorreos.ipynb
- `datasets/`: Tenemos 5 archivos csv. Los 2 archivos enron1spam_ham.csv y gitHub_spam.csv contienen los emails. Podemos subirlos para ejecutar el cuaderno ExtraeCaracteristicasCorreos.ipynb. Por otro lado los otros 3 archivos contienen las 57 características de los emails. Estos los podemos subir para ejecutar el cuaderno ClasificadorSpam.ipynb
- `modelo/`: Tenemos 3 archivos. Hay 2 ficheros con el modelo exportado, listo para usar en javascript, y hay 1 fichero html que lleva el código para usar el modelo para hacer predicciones.

## Ejecución
Para ejecutar el cuaderno ExtraeCaracteristicasCorreos.ipynb hay que seguir los siguientes pasos:
1. Abrimos el cuaderno en Google Colab.
2. Al lanzar la primera celda de código te aparecerá la opción de subir ficheros y se deben subir los 3 archivos enron1spam_ham_pedro.csv, gitHub_spam_pedro.csv y spambase_pedro.csv que se encuentran en `datasets/`.
3. Lanzamos todas las celdas de código en orden.
4. Dentro del propio cuaderno, se explica que se pueden hacer diversas pruebas comentando y descomentando algún código.
5. Descargamos el modelo si lo hemos llegado a exportar.

Para ejecutar el cuaderno ClasificadorSpam.ipynb hay que seguir los siguientes pasos:
1. Abrimos el cuaderno en Google Colab.
2. Al lanzar la primera celda de código te aparecerá la opción de subir ficheros y se debe subir uno de los 2 archivos enron1spam_ham.csv o gitHub_spam.csv.
3. Según si hemos subido uno u otro hay una parte del código que hay comentar o descomentar, que está explicado en el propio cuaderno.
4. Lanzamos todas las celdas de código en orden.
5. Descargamos el fichero final.

Para ejecutar el modelo y hacer predicciones hay que seguir los siguientes pasos:
1. Descargamos la carpeta `modelo/` con sus 3 ficheros en nuestro ordenador.
2. Abrimos CMD (línea de comandos).
3. Nos ubicamos en la ruta donde hemos dejado la carpeta con el comando `cd`. A modo de ejemplo: `cd Desktop\modelo`.
4. Si no tenemos python instalado tendremos que instalarlo.
5. Lanzamos el comando `python -m http.server 8000`.
6. Abrimos un navegador y escribimos `localhost:8000/index.html`.
7. Ya podemos probar las predicciones escribiendo texto y dándole a predecir.
