# Entrenamiento de los modelos en Google Colab
Este proyecto esta dedicado a la personalización de un modelo de detección gracias a las prestaciones que ofrece YOLOv8. La deteccion se realiza sobre jitomates, por lo que se tiene un enfoque al cuidado fitosanitario, por lo que se parte de la detección del estado de madurez del fruto en 3 estados.

- Maduro
- Semimaduro
- Verde

El dataset correspondiente, se le aplicó una técnica de muestreo llamado **K-FOLD CROSS VALIDATION (K-FCV)**, por lo que se obtuvieron 5 splits. En este sentido, se tienen 5 particiones que se pueden entrenar independientemente, ya que, estos tienen diferentes datos, especialmente la carpeta de validación. Cada carpeta de validación es única entre cada 5 split.

Con los 5 folds, se procedió a un entrenamiento individual, por lo que se recurrió a Google Colab con su GPU Tesla T4 para el entrenamiento de cada particición, puesto que el equipo de cómputo personal no era suficiente. Finalmente, el proceso realizado de los entrenamientos se guardan como cuadernos de jupyter, permitiendo su consulta en cualquiero momento.
