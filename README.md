# TFG - Mejora de un Sistema de Auto-escalado para Sistemas Distribuidos
## Resumen
Uno de los principales pilares de la computación en la nube es la elasticidad, es decir, la capacidad de ajustar los recursos necesarios de forma automática para cubrir la demanda en cada instante. Los sistemas de auto-escalado son los encargados de dotar de elasticidad a los sistemas escalables. Dichos sistemas de auto-escalado están recibiendo gran atención en los últimos años debido a la expansión de las arquitecturas basadas en micro-servicios (e.g. Kubernetes y Docker) y al auge de la computación en la nube.

En el contexto de este proyecto, se está desarrollando un sistema de auto-escalado que combina las técnicas de auto-escalado reactivas y predictivas mediante la aplicación de modelos estadísticos.
Este Trabajo de Fin de Grado aborda la mejora del auto-escalado de sistemas distribuidos por medio del estudio del comportamiento de E-SilboPs bajo una carga de trabajo real a través de la obtención y monitorización de las métricas de rendimiento relevantes.

Con este fin, se ha llevado a cabo una búsqueda de una carga de trabajo que se haya usado en un contexto de uso real. La carga escogida, procedente del sistema PADRES, un sistema publicador/subscriptor basado en contenido ampliamente usado en literatura, ha de ser traducida al formato de E-SilboPS. Para esto, se ha diseñado e implementado un generador de cargas de trabajo reales, que traducirá los eventos de dicha carga, manteniendo el contexto y contenido de cada uno de ellos (usuario, parámetros de las subscripciones y publicaciones, etc.).
Una vez traducida la carga de trabajo, para medir el rendimiento del sistema con esta, se han diseñado e implementado diferentes pruebas para obtener estas métricas de rendimiento, lo que permite identificar la saturación y comportamiento del sistema.
Esto ha permitido la generación de otras cargas basadas en la real para llevar al sistema a situaciones especiales y medir su respuesta de forma más detallada.
A continuación, se han diseñado e implementado diferentes modelos predictivos basados en Machine-Learning y Deep-Learning, que se aplicarán a los resultados de las pruebas realizadas, con el objetivo de predecir el comportamiento del sistema y así aplicar estas predicciones al sistema de auto-escalado.

Los resultados obtenidos en este Trabajo de Fin de Grado muestran el correcto funcionamiento del generador de cargas de trabajo, al haber traducido la carga de PADRES de forma satisfactoria; y la utilidad de dicha carga, al comprobar que E-SilboPS llega a saturar parcialmente, posibilitando la aplicación de los modelos predictivos para predecir futuras situaciones de saturación

**Palabras Clave:** Auto-escalado, Sistemas Distribuidos, Cloud, Modelos Estadísticos.
