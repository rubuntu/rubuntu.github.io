# Un viaje hacia (Driverless) AI

Me han preguntado cómo se debe hacer para ingresar al área de Ciencia de Datos *(Data Science)*. 
No hay un solo camino de aprendizaje.

_**La respuesta corta:**_   
Recomendaciones:
- Revisar las matemáticas de secundaria y universidad:
  - Álgebra lineal
  - Cálculo
  - Estadística
- Luego tomar un curso de Data Science en un MOOC.
- Asistir a reuniones y conferencias sobre ciencia de datos
- Como lenguaje de programación puedes aprender R o Python, pero también herramientas con GUI como KNIME, RapidMiner, IBM SPSS Modeler, entre otros.  
- Como se trabajaría con bases de datos relacionales, es importantísimo aprender SQL.  

_**La respuesta larga:**_   
Una respuesta larga es contarte acerca de mi viaje a *Data Science*.  
En primer lugar, no me considero un experto, sino una persona que busca aprender continuamente.  
Además, me considero una persona técnica con intereses en los negocios. Mi educación académica es una licenciatura en ciencias de la computación, y estoy estudiando una maestría en administración de empresas (MBA) y todavía tengo que retomar mi maestría en ciencias de la computación.  
Aunque hoy trabajo en el área de *Data Science*, tuve la oportunidad de rotar a otras áreas como: Negocios / Marketing y Riesgos, lo que me dio una visión más amplia de la organización.  
Mi primer contacto con *Data Science* fue cuando estaba tomando el curso de maestría en informática antes mencionado, con asignaciones de *Data Warehousing* y *KDD / Data Mining*, lo que despertó mi interés en esa área. 

_**Almacenamiento de datos y BI**_  
Mientras tanto, aproveché una oportunidad de trabajo en Vision Banco, un banco en mi país, Paraguay, donde me uní a un área especializada en Data Warehousing & Business Intelligence (BI).  
Esta iniciativa analítica funciona en la organización como un puente del área de TI con las otras áreas de la empresa y como una fuente de información consolidada. La metodología de Ralph Kimball fue adoptada para la construcción del Data Warehouse. El conjunto de herramientas de BI que se adoptó es IBM Cognos, y se está utilizando en informes, cubos OLAP, paneles interactivos, aplicaciones de planificación y cuadros de mandos (aplicando los conceptos de Robert Kaplan).  
Los procesos ETL (Extracción, Transformación y Carga) se realizan con el software de código abierto Pentaho Data Integration, hoy parte de la suite Hitachi Vantara. 

_**Analítica predictiva**_  
En 2012, se contrató una consultoría externa para el desarrollo y acompañamiento de la implementación de un modelo de *"Credit Scoring"* . Este modelo predictivo, fue desarrollado usando IBM SPSS usando el algoritmo de Regresión Logística. Al acompañar el desarrollo de este modelo de *credit scoring*, aprendimos, cómo, e incorporamos a nuestra organización el siguiente nivel en Análisis descriptivos (¿Qué?) Y Diagnóstico (¿Por qué?), Cuando comenzamos a hacer también Análisis predictivo (Qué hará). ¿Pasa?) Y prescriptivo (¿Cómo hacer que suceda?).

_**Big Data Pilot**_  
En 2014 hicimos un proyecto piloto de Big Data: Análisis de Sentimiento en Redes Sociales. La infraestructura se contrató en la nube y utilizamos los clusters NoSQL Redis y MongoDB, donde se procesaron los "tweets" de la red social Twitter para monitorear la imagen del banco. En el proceso de minería de texto, se utilizó el algoritmo Naive Bayes, que a pesar de ser sencillo, funcionó muy bien.

_**Ciencia de Datos**_  
Mientras tanto, el área de Data Warehouse / BI del banco pasó a llamarse Data Science.  
Desde 2015 hasta la fecha, dentro de la organización, se desarrollaron modelos internos predictivos con algoritmos más avanzados: Random Forest, GBM, XGBoost, Deep Learning y ensamblajes con estos algoritmos, y se implementaron en producción utilizando openscoring.io (modelos en formato PMML) y últimamente, H2O.ai.

_**H2O.ai**_  
¿Cómo descubrí H2O.ai?, A través de blogs de data science, donde cada vez veía más y más menciones.  
En ese momento solía hacer modelos en R usando Random Forest, pero construir un modelo con este algoritmo con bibliotecas tradicionales de R podría tomar horas. La primera vez que evalué H2O, ¡la construcción del mismo modelo duró minutos en el mismo hardware! ¿Por qué? Debido a que H2O está optimizado y usa todos los núcleos de los equipos multinúcleo presentes en cualquier escritorio hoy.  
¡Otra ventaja de usar H2O es que el código que podría ejecutarse en una computadora portátil es el mismo para ejecutarse en un *cluster* para escalar a Big Data!  
Desde allí, comenzamos a hacer la transición a H2O como la plataforma principal para desarrollar soluciones de aprendizaje automático en la organización.

_**Driverless AI**_  
Hace poco más de un año, tuve la oportunidad de evaluar una nueva propuesta para H2O.ai: Driverless AI, una plataforma que automatiza gran parte del proceso de la ciencia de datos realizando ingeniería de características, capacitación y ensamblaje de modelos, junto con la posibilidad de generar Conductos para el despliegue del modelo final y modelos para la interpretación del mismo.  
Para hacer una prueba de concepto de Driverless AI, alquilé una VM con una GPU en la nube y participé en un concurso de ciencia de datos organizado por AnalyticsVidhya.com: "Data Science Hackathon: Churn Prediction", ¡obteniendo el 8vo lugar!  
Escribí sobre esto en la siguiente publicación: https://www.linkedin.com/pulse/how-get-eighth-place-data-science-competition-using-driverless-diaz/  
Este increíble resultado se debe a que Driverless AI utiliza la experiencia de "Kaggle Grand Masters in a Box". Ver https://www.h2o.ai/blog/kaggle-grand-masters-recipes-production-ready-clicks/  
La prueba de concepto sirvió para demostrar las muchas posibilidades y ventajas de usar Driverless AI.  

_**IBM Power System AC922 + Driverless AI**_  
Mientras tanto, cuando Vision Banco aceptó adquirir el hardware IBM Power System AC922 - con CPUs POWER9 y GPUs NVIDIA Volta GV100 - para respaldar sus iniciativas de aprendizaje automático (ML) e inteligencia artificial (AI), también se adquirió el software H2O Driverless AI.  
Comenzamos a utilizar H2O Driverless AI para casos de uso críticos: propensión a comprar, predicción de incumplimiento, calificación de crédito, etc.  
Los nuevos desarrollos de modelos predictivos de casos de uso con clasificación y regresión ya se están realizando con Driverless AI, y planeamos usarlo en proyectos de pronóstico de series de tiempo y procesamiento de lenguaje natural (PNL).  
Al utilizar Driverless AI en IBM Power System AC922, hemos podido construir nuestras soluciones ML / AI en menos tiempo, con mejor calidad y precisión.  

**PD:** Me siento honrado de ser *Speaker* en H2O World San Francisco ( http://h2oworld.h2o.ai/h2o-world-san-francisco/ ), para hablar sobre el viaje de ML / AI en Vision Banco con H2O Driverless AI en sistemas basados ​​en IBM POWER9 con GPUs. 
Si estás en San Francisco esos días, ¡nos vemos allí!

**PPS:** Echale un vistazo a mi proyecto de código abierto: el servicio web REST Mojo Model & Driverless AI Mojo Pipeline de H2O.ai para *scoring* en tiempo real. https://github.com/rubuntu/h2o_scorer