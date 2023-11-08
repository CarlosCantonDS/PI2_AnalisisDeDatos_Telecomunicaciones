<p align='center'>
<img src ="https://d31uz8lwfmyn8g.cloudfront.net/Assets/logo-henry-white-lg.png">
<p>

<h1 align='center'>
 <b>PROYECTO ANÁLISIS DE DATOS</b>
</h1>

¡Bienvenidos a mi proyecto!, tomando el rol de ***Data Analyst*** sobre las telecomunicaciones en Argentina.<br>
En este README, se explicará de forma general el proyecto desde el EDA, hasta algunas conclusiones sobre
los datos y KPI´s así como el uso de Power BI para el dashboard final.
 
# <h1 align="center">**`Análisis de Telecomunicaciones en Argentina`**</h1>

<p align='center'>
<img src="https://newses.cgtn.com/n/BfJIA-CAA-HAA/BceGDAA.jpg"  height=300>
<p>

### **Descripción y Contexto del Proyecto**

Las telecomunicaciones se refieren a la transmisión de información a través de medios electrónicos, como la telefonía, la televisión, la radio y, más recientemente, el internet. Estos medios de comunicación permiten la transmisión de información entre personas, organizaciones y dispositivos a largas distancias.

El internet, por su parte, es una red global de computadoras interconectadas que permite el intercambio de información en tiempo real. Desde su creación, ha tenido un impacto significativo en la vida de las personas, transformando la manera en que nos comunicamos, trabajamos, aprendemos y nos entretenemos.

La industria de las telecomunicaciones ha jugado un papel vital en nuestra sociedad, facilitando la información a escala internacional y permitiendo la comunicación continua incluso en medio de una pandemia mundial. La transferencia de datos y comunicación se realiza en su mayoría a través de internet, líneas telefónicas fijas, telefonía móvil, y en casi cualquier lugar del mundo. 

En comparación con la media mundial, Argentina está a la vanguardia en el desarrollo de las telecomunicaciones, teniendo para el 2020 un total de [62,12 millones de conexiones](https://www.datosmundial.com/america/argentina/telecomunicacion.php). 

Como tal, el enfoque de este proyecto será relacionado específicamente con Internet y Telefonía, a lo largo de este readme se demostrará porque se escogieron esos dos servicios para este proyecto.


### **Roles principales del Proyecto**

Este proyecto se divide de forma estructurada en los siguientes puntos, que se describen a continuación en este readme:

- EDA (Análisis Exploratorio de Datos):
    - Calidad del dato.
    - Análisis de relaciones y patrones de los datos.

- Enfoque del Storytelling del proyecto:
  Conociendo los datos en el EDA se pudo definir un enfoque sobre el cual se presentarán los dashboards.

- KPI´s (Indicador Clave de Rendimiento):
  Conociendo los datos en el EDA se pudo definir ciertos KPI´s que serán abordados en este readme y que fueron incluidos en los dashboards de Power BI.

- Dashboard con Power BI:
  Finalmente, para presentar las visualizaciones y los KPI´s del proyecto, se realizaron gráficos interactivos utilizando Microsoft Power BI.



`EDA (Análisis Exploratorio de Datos)`

- Calidad del dato:<br>
Se inició el EDA con una fase de preprocesamiento para limpiar el conjunto de datos. Esta etapa implicó la identificación y manejo de valores faltantes o nulos, outliers, la corrección de formatos de datos y la unificación de tablas relevantes para un análisis más profundo. El método utilizado para calcular los outliers fue el del umbral de 3 desviaciones estándar y se consideraron outliers los superiores e inferiores al umbral definido. Para tener mayor prolijidad en el código y mayor orden a lo largo del proyecto, se desarrolló un archivo helper.py que cuenta con funciones para hacer análisis sobre la calidad del dato. <br>
- Análisis de relaciones y patrones de los datos:<br>
Se exploraron diferentes variables presentes en el conjunto de datos, como la cantidad de accesos por tecnología, la distribución de servicios por provincia, la evolución de ingresos a lo largo de los años y otros factores relevantes dentro de la industria de las telecomunicaciones.<br>
Por ejemplo, en el siguiente gráfico se puede observar el cambio que hay entre la cantidad de accesos por año por cada tipo de tecnología: ***Nota:*** Los gráficos presentados en este README son para tener un primer vistazo, se pueden observar con mayor profundidad en el jupyter notebook de este repositorio ***********************INSERTAR GRAFICO*********** <br>

************DESPUES DEL GRAFICO<br>
En un breve vistazo podemos ver que para ADSL fue reduciendo la cantidad de accesos promedio por año y que para fibra óptica comenzó a haber un incremento notable a partir de 2018 en adelante. <br>

Por otra parte, con el EDA se pudo saber cuál es el Top 5 de provincias con mayor cantidad de accesos y con base en ese Top 5 se realizó la siguiente gráfica que presenta la evolución de las velocidades que tiene cada provincia en promedio a lo largo de los últimos años, basado en las provincias del Top 5: ***************INSERTAR GRAFICO <br>

**************DESPUES DEL GRAFICO: 
Un breve análisis con lo que podemos observar es que, hay mucha variación en la velocidad aún habiendo seleccionado el Top 5 con mayor cantidad de accesos por ejemplo, para Tierra de fuego que está en el top 2 de cantidad de accesos, tiene las menores velocidades a lo largo de la gráfica de tiempo. Lo cual, denota que no hay una relación entre la cantidad de accesos y la velocidad promedio por provincia, pero en algunos casos si es congruente como es el caso de Cápital Federal. Para analizar mejor las gráficas se puede ingresar al notebook de este repositorio.

`Enfoque del Storytelling del proyecto`

Con base en el EDA y toda la información que se analizó, se decidió tomar el siguiente enfoque para la narrativa que se va a seguir durante los dashboards y el resto del proyecto: Principalmente, el enfoque se basa en que, los servicios con mayor cantidad de reclamos son los servicios de Internet y Telefonía (como parte de la consigna de este proyecto se dió como fuente de datos obligatoria el Servicio de Internet) por lo cual, se tomó en cuenta la telefonía como un análisis complementario. Tomando en cuenta la cantidad de reclamos y considerando que Internet cuenta con una mayor cantidad de ingresos por este servicio, se decidió presentar KPIs relacionados con estos dos servicios y tomar el enfoque de la mejora de los mismos. Se presentarán KPIs que serán enfocados acorde con esta narrativa.

`KPI´s (Indicador Clave de Rendimiento)`



`Dashboard con Power BI`

Para este dashboard se aplicó el patrón Z para tener una mejor visualización, más clara de los datos. El patrón Z en diseño se refiere a un concepto de diseño que se basa en el seguimiento de la trayectoria natural de la lectura que los ojos humanos tienden a seguir al mirar una página. Esto resulta en una distribución más efectiva de la información, facilitando la comprensión y la interacción con los datos presentados. <br>
A continuación se presenta uno de los gráficos realizados en Power BI pero el dashboard completo con sus distintas pestañas y los KPIs se encuentran en el archivo del dashboard. ************INSERTAR TREEMAP



Debes graficar y medir el KPI propuesto a continuación, representándolo adecuadamente en el dashboard. A su vez, tambíen tienes que proponer, medir y graficar un segundo KPI que consideres relevante para la temática. 
El KPI propuesto es:
- *Aumentar en un 2% el acceso al servicio de internet para el próximo trimestre, cada 100 hogares, por provincia*.
La fórmula es la siguiente:

 $`KPI = ((Nuevo acceso - Acceso actual) / Acceso actual) * 100`$
 
Donde:

- "Nuevo acceso" se refiere al número de hogares con acceso a Internet después del próximo trimestre.
- "Acceso actual" se refiere al número de hogares con acceso a Internet en el trimestre actual.

Esta fórmula te ayudará a calcular el KPI para medir el aumento en el acceso a Internet por cada 100 hogares en cada provincia.

**Ejemplo de uso:**

KPI = ((510 - 500) / 500) * 100 = 2%

Esto indicaría un aumento del 2% en el acceso a Internet en esa provincia para el próximo trimestre.

`MUY IMPORTANTE` repasar qué es un KPI y cómo se diferencia de una métrica convencional. En el material de apoyo tienen lectura que puede ser de ayuda.</small>

`Repositorio de GitHub`

El repositorio debe contener un **Readme** principal donde presenten, en una primera instancia, de forma general **su proyecto** y detallen qué hay en cada archivo/carpeta del propio repositorio. Este Readme no puede ser el mismo de la consigna que nosotros les entregamos.
A su vez, el Readme debe incluir un **reporte de análisis con base en sus dashboards**, así como el análisis y la funcionalidad de los KPIs sugeridos.

### _**Desafíate y no te quedes siendo Junior, sé Junior Advanced**_

Pensando en alcanzar tu Boom 🚀, te recomendamos incorporar los siguientes desafíos para tener un portfolio mucho más completo y competitivo:

- Crear una base de datos en un motor SQL, ingestar el dataset procesado y utilizarla como fuente de datos de su dashboard en Power BI (o la herramienta de visualización que utilice).
- Ejecutar scripts de Python en la herramienta de visualización de datos escogida.
- Cruce de datos con datasets complementarios, ya sea para obtener información nueva o poder comparar la información disponible en el dataset obligatorio. 

<sub> Nota: la realización de uno o más de estos ítems no es intercambiable con los requerimientos mínimos establecidos en la sección anterior "Propuesta de trabajo". Empiece con esta sección una vez haya cumplido con los requerimientos mínimos, a modo de desafiarse a usted mismo y destacar frente al resto.</sub>

## Fuente de datos
**Obligatorio:**

- [Datasets principales](https://datosabiertos.enacom.gob.ar/dashboards/20000/acceso-a-internet/) -se sugiere el uso de la API para traerse los datos-

**Complementario:**
- [Datasets complementarios](https://datosabiertos.enacom.gob.ar/home)

- Cualquier dataset de búsqueda propia que complemente y mejore el análisis.

<h1>Lo que tendremos en cuenta a la hora de evaluar</h1>

Serás evaluado en dos grandes áreas  `Tech` y `Soft`!

Ambas con igual peso entre si y ambas deben ser aprobatorias para tener la calidad de aprobado en este PIDA. Ten presente que una nota mínima para aprobar significa tener TODOS los items como "Bueno" 👌
A continuación te facilitamos nuevamente la [rúbrica de evaluación](https://docs.google.com/spreadsheets/d/e/2PACX-1vTV3zL1aeGRlbXkiy5012GWbDBMseA4iziMXs597TZfgaYgazjxZDx_-q6L4s9io3JW4UPHcZs_XNyz/pubhtml) con la que serás evaluado por tu corrector@. Recuerda que el feedback de tu corrector@ no es en ningun momento un indicativo de tu nota. Si tienes alguna duda durante tu DEMO, pídele a tu corrector@ que te aclare claramente cuales son los objetivos de aprendizaje no cumplidos.

Esperamos que te sirva de guía de aprendizaje, y recuerda que no se trata solo de cumplir requisitos, sino de destacar en cada nivel 🚀 💛


## Material de apoyo

#### Tech
- [Repaso de clase sobre EDA](https://www.students.soyhenry.com/classes/100?cohortId=106&videoOrdinal=1)
- [Code Review: **Interactividad** Dashboard, Patron Z, **Tooltips**](https://www.students.soyhenry.com/classes/93?cohortId=124&videoOrdinal=2)
- [KPI's 4 students](https://docs.google.com/document/d/1DI0ZVgHfOfjgnXGhi8jEKzwCIjtUdgRUDe-qiiGGq8E/edit)
- [Code Review: DAX y **medidas calculadas**](https://www.students.soyhenry.com/classes/96?cohortId=124&videoOrdinal=2)

#### Soft
- ¡Todos los Workshops de esta etapa serán de gran utilidad para tener un proyecto exitoso!


## ***Recomendaciones finales***

¡No debes mostrar nada de código en la exposición! Te recomendamos el workshop *From Data to Viz* para que te quede más claro la dinámica y lo que se espera de tu demo.

Recuerda ser puntual y probar el correcto funcionamiento de las herramientas empleadas ***antes*** de ingresar a la meet.

La **DEMO**, donde defenderás tu proyecto, se realizará el día jueves o viernes. Debes estar atent@ a tu *calendar* para ver qué día y horario te corresponde. 

Esta demo tendrá una duración total máxima de 30 minutos, de los cuales **sólo 10 minutos serán para tu presentación**.  Es importante que sepas **gestionar bien tu tiempo** y tengas un speech ya preparado de 10 minutos, ya que el tiempo restante será dedicado a la corrección, revisión de repositorio y feedback por parte del Henry Mentor.



## Disclaimer
De parte del equipo de Henry se quiere aclarar y remarcar que los fines de los proyectos propuestos son exclusivamente pedagógicos, con el objetivo de realizar proyectos que simulen un entorno laboral, en el cual se trabajen diversas temáticas ajustadas a la realidad. No reflejan necesariamente la filosofía y valores de la organización. Además, Henry no alienta ni tampoco recomienda a los alumnos y/o cualquier persona leyendo los repositorios (y entregas de proyectos) que tomen acciones en base a los datos que pudieran o no haber recabado. Toda la información expuesta y resultados obtenidos en los proyectos nunca deben ser tomados en cuenta para la toma real de decisiones (especialmente en la temática de finanzas, salud, política, etc.).
  
  
<p align='center'>
<img src ="https://media.giphy.com/media/BpGWitbFZflfSUYuZ9/giphy.gif" height=250>
<p>
