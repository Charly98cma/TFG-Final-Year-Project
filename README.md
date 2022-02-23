# Mejora de un Sistema de Auto-escalado para Sistemas Distribuidos
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

# Improving an Auto-scalling System for Distributed Systems
## Abstract
One of the main pillars of cloud computing is elasticity, i.e. the ability to automatically adjust the resources needed to meet the demand at any given time. Auto-scaling systems are responsible of providing elasticity to scalable systems. This auto-scaling systems are getting increasing attention in recent years thanks to the growth of micro-services based architectures, e.g. Kubernetes and Docker, and the rise on popularity of cloud computing.

In the context of this project, an auto-scaler system is being developed, that combines both reactive and predictive auto-scaling techniques by applying statistical models.

This Trabajo de Fin de Grado addresses the improvement of the auto-scaling of distributed systems by studying the behaviour of E-SilboPS under a real-world workload, obtaining the relevant performance measurements.

To this end, a search has been carried out for a workload that has been used in a real-world context. This workload must be compatible with the E-SilboPS system, analysing its content to obtain statistical data, and verifying  the completeness and compatibility of this workload data.

The chosen real-world workload, extracted from PADRES, a content-based publish/subscribe system widely used on literature; must be translated to the E-SilboPS format. To achieve this, a real workload generator has been designed and implemented, that performs this translation by interpreting each event and its content, and transforming it to the E-SilboPS syntax, keeping its original context (user, subscription and publications parameters, etc.).

With the workload already translated, to test the system performance using it, different tests have been developed to obtain its system performance metrics, allowing detection of situations in which the system saturates. This allowed the creation of other workloads, based on the real-world one, that tests the system on special situations and measure the system response in more detail.


Once the system has been tested, different predictive models have been designed and implemented, based on Machine-Learning and Deep-Learning, that will be applied to the results of the tests carried out, in order to predict the behaviour of the system and then apply these predictions to the auto-scaling system.

The results obtained of this Trabajo de Fin de Grado reflect the real workload generator working correctly, since it translated the PADRES real-world workload; and the usefulness of said workload through verifying that E-SilboPS partially saturates, which opens the door to the possibility of implementing improvements on FLAS if new predictive models are applied.

**Keywords:** Auto-scaling, Distributed Systems, Cloud, Statistical Models.
