<h1>Proyecto integrador del Bootcamp 9.0 por UNICORN ACADEMY</h1> 

![Static Badge](https://img.shields.io/badge/Own%20Project%20-%20Proyecto%20Propio?style=for-the-badge&color=black)





# Introducción
Proyecto integrador realizado en equipo con Sofía Gonzalez como ejercicio final del Bootcamp 9.0, donde se tomaron datos de una empresa real, datos suministrados por varios documentos en Excel de los meses de enero a julio del 2025. Los datos fueron avalados y por protección de datos , se realizó limpieza, análisis estadistico descriptivo, una visualización mediante dashboard y se realizó propuestas de valor, utilizando Excel, MySQL, Google Colab y Power BI


 
<h3>1. Data source</h3> 
 Empresa colombiana de telecomunicaciones - TELECOM (Empresa creada por protección de datos) 
 
 
### 2. Objetivos
#### 2.1 Objetivo principal
- Desarrollar un proyecto completo donde seamos capaces de analizar una información bruta y generar propuestas de valor al stakeholder.
#### 2.2. Objetivos específicos
- Recibir la información y realizar un primer filtrado en Excel.
- Transformar la información y generar un segundo filtrado en MySQL.
- Analizar la información en Google Colab desarrollando un análisis estadístico descriptivo.
- Conectar con SQLite para dar respuesta a las preguntas del stakeholder.
- Visualizar los resultados obtenidos en Power BI.
- Desarrollar propuestas de valor.
  
### 3. Tecnologies
![Static Badge](https://img.shields.io/badge/Excel%20-%20p?style=for-the-badge&logo=Excel&logoColor=white&label=Microsoft%20Office&labelColor=%23007C3C&color=black) |
![Static Badge](https://img.shields.io/badge/SQL%20-%20p?style=for-the-badge&logo=MySQL&logoColor=white&label=MySQL&labelColor=%234479A1&color=black) |
![Static Badge](https://img.shields.io/badge/Python%20-%20p?style=for-the-badge&logo=Google%20Colab&logoColor=white&label=Google%20Colab&labelColor=%23F9AB00&color=black) |
![Static Badge](https://img.shields.io/badge/SQL%20-%20p?style=for-the-badge&logo=SQLite&logoColor=white&label=SQLite&labelColor=%23003B57&color=black) |
![Static Badge](https://img.shields.io/badge/DAX%20-%20p?style=for-the-badge&logo=PowerBi&logoColor=white&label=Power%20BI&labelColor=%23F99F1C&color=black) |
![Static Badge](https://img.shields.io/badge/PDF-%20p?style=for-the-badge&logo=Canva&logoColor=white&label=canva&labelColor=%2300C4CC&color=black)


### 4. Preguntas del Stakeholder
#### Rendimiento por planes: 
● Requerimos saber el volumen de venta e ingresos generados de los planes según su tipo de servicio. <br/>
● ¿Cómo se distribuyen los ingresos y la cantidad de transacciones entre los diferentes tipos de servicio como Mobile y B2B?<br/>
● ¿Cuál es el valor promedio de cada transacción para Mobile y B2B?<br/>
● ¿Cuál es el valor MAX y MIN del servicio B2B y Mobile?<br/>
● ¿Qué planes específicos son los más rentables dentro de cada tipo de servicio?<br/>
● ¿Cuál es la relación entre ingresos totales y ventas totales por plan?<br/>
● Teniendo en cuenta el nombre del plan, ¿Qué consultores están llevando las ventas del servicio B2B?<br/>
● ¿Qué canal es más efectivo para vender planes B2B que para Mobile?<br/>
● ¿Cuál es la rentabilidad de los servicios por canal?<br/>
● ¿Cuál es el estado de cada plan?<br/>
#### Rendimiento cruzado de canales y asesores
● Requerimos el volumen de venta e ingresos totales por los diferentes canales de venta.<br/>
● ¿Qué asesor son los más rentables por tienda?<br/>
● ¿Cuántos consultores trabajan para los diversos canales de venta?<br/>
● ¿Por mes cuántos asesores tiene cada estado?<br/>
● ¿Cuántos consultores hay por tienda?<br/>
● ¿Qué tiendas son las más rentables para la venta de los servicios B2B y mobile?<br/>
● ¿Cuál es la relación entre el volumen de venta e ingresos generados por almacén?<br/>
#### Rendimiento del Equipo de Ventas (Consultores)
● ¿Cuál es el ingreso promedio y el volumen de venta por asesor?<br/>
● ¿Qué planes de datos vende cada asesor?<br/>
● ¿Cuántos consultores hay por estado y quienes son?<br/>
● ¿Cuántas ventas mensuales llevan a cabo los asesores solamente en estado Active? (Meta 2 diarias)<br/>
● ¿Cuántas ventas trimestrales llevan a cabo los asesores solamente en estado Active? (Meta 180 trimestral)<br/>
● Realizar una evaluación del rendimiento vs. la meta según el estado Active.<br/>
● ¿Cuál es la tasa de abandono para el estado Termination?<br/>
● Evaluación del rendimiento vs. la meta en estado Termination.<br/>
● Evaluación del rendimiento vs. la meta en estado One-Way Block<br/>
● Evaluación del rendimiento vs. la meta en estado Two-Way Block<br/>
#### Evaluación de los operadores antiguos.
● ¿Qué planes están asociados a los antiguos operadores?<br/>
● ¿Existe alguna correlación entre el operador del cliente y el tipo de plan que contratan (B2B o Mobile)?<br/>

### 5. Desarrollo
#### 5.1 Recepción de la información en: ![Static Badge](https://img.shields.io/badge/Excel%20-%20p?style=for-the-badge&logo=Excel&logoColor=white&label=Microsoft%20Office&labelColor=%23007C3C&color=black)
Como consultora Data-Consulting SH, nos contactamos con una empresa de telecomunicaciones de Colombia, la cuál el stakeholder no se encontraba satisfecho con las métricas que le enviaba el soporte IT de la empresa. Por protección de datos, le cambiamos el nombre a Telecom. La información fue recibida a principios de julio del 2025 en varios archivos separados por meses desde enero a junio del mismo año, esta información fue entregada en formato Excel (.xlsm) mostrando una tabla dinámica. Cada archivo tenía 26 columnas con información entre relevante y no relevante, así mismo, cada archivo era por mes, por lo tanto, debíamos realizar una concatenación de la información que se pudiera manipular de forma inicial. En comunicación constante con el stakeholder, para mejorar la productividad del proyecto, por propuesta del mismo, tomó como decisión manejar los meses de abril, mayo y junio, los cuales son el segundo trimestre del 2025, meses a desarrollar y analizar como un análisis trimestral. El stakeholder hace parte de la región Eje Cafetero pospago, lo cuál por autorización del mismo y al reducir la cantidad de datos de más de 300.000 filas a 7.019 ayudaría en el proceso de limpieza, análisis y desarrollo del mismo.
#### 5.2. Desarrollo modelo relacional en MySQL ![Static Badge](https://img.shields.io/badge/SQL%20-%20p?style=for-the-badge&logo=MySQL&logoColor=white&label=MySQL&labelColor=%234479A1&color=black)
Para desarrollar el modelo relacional, se transformó la información y la redireccionamos en 4 tablas las cuales son: <br/>
1. Tabla dim_planes.xlsm<br/>
2. Tabla dim_consultores.xlsm<br/>
3. Tabla dim_operadores.xlsm<br/>
4. Tabla dim_canales_de_ventas.xlsm<br/>
5. Tabla fact_transacciones.xlsm<br/>

La creación del modelado de datos fue realizada en MySql, donde creamos un primer script_telecom y desarrollamos mediante código en lenguaje SQL las distintas tablas dimensionales con su tabla de hechos.
#### 5.3. Análisis exploratorio y limpieza inicial ![Static Badge](https://img.shields.io/badge/SQL%20-%20p?style=for-the-badge&logo=MySQL&logoColor=white&label=MySQL&labelColor=%234479A1&color=black)
Al validar la información de cada tabla, iniciamos el análisis exploratorio y limpieza inicial de los datos importados desarrollando en el script_limpieza.
Lo primero que hacemos en la es usar el database telecom_base para trabajarlo durante esta etapa. Luego, se procede a: <br/>
● Consulta de cada tabla.<br/>
● Limpieza inicial.<br/>
● Identificación y modificación de nombres mal escritos.<br/>
● Identificación y modificación de operador sin nombre.<br/>
● Ajuste a valores enteros de variables cuantitativas.<br/>
● Creación archivo .csv. <br/>

#### 5.4. Análisis estadístico descriptivo ![Static Badge](https://img.shields.io/badge/Python%20-%20p?style=for-the-badge&logo=Google%20Colab&logoColor=white&label=Google%20Colab&labelColor=%23F9AB00&color=black)

Encontramos amigable para nuestro desarrollo usando la herramienta que tiene Google, que es Google Colab, que es una herramienta muy similar a Jupyter de Anaconda las cuales se codifica en lenguaje Python y que se puede realizar el desarrollo de manera online entre los participantes de este proyecto. Luego de haber creado los data frames correspondientes, iniciamos consultado la información, la cantidad de valores en el array y definiendo si existen nulos en los datos, con esto, comprobamos que la limpieza en Mysql fue efectiva. Luego se procede a hacer:<br/>

 ● Resumen estadístico.<br/>
 ● Distribución de variables.<br/>
 ● Distribución outliers.<br/>
 ● Validación de fechas.<br/>
 ● Chequeo de integridad.<br/>

 #### 5.5. Desarrollo de preguntas de negocio ![Static Badge](https://img.shields.io/badge/SQL%20-%20p?style=for-the-badge&logo=SQLite&logoColor=white&label=SQLite&labelColor=%23003B57&color=black)
 Se realiza conexión con SQLite desde Google Colab realizando:
 ● Importe de librerías myprettytable y sqlalchemy<br/>
 ● Modificación de dataframes. <br/>
 ● Se realiza codificación para dar respuesta a cada pregunta de negocio obtenida por el stakeholder.<br/>

 #### 5.6 Visualización de informes y problemáticas encontradas. ![Static Badge](https://img.shields.io/badge/DAX%20-%20p?style=for-the-badge&logo=PowerBi&logoColor=white&label=Power%20BI&labelColor=%23F99F1C&color=black)
Teniendo en cuenta que el stakeholder desea conocer los insights encontrados, hemos desarrollado mediante Power BI una visualización clara, sencilla y eficaz de lo que nosotros como analistas hemos encontrado, visualizando los siguientes informes:
● Informe general <br/>
● Informe de tiendas <br/>
● Informe de asesor <br/>
● Informe de Insights <br/>
● Ranking asesor <br/>

#### 5.7. Propuestas de valor ![Static Badge](https://img.shields.io/badge/PDF-%20p?style=for-the-badge&logo=Canva&logoColor=white&label=canva&labelColor=%2300C4CC&color=black)

Hemos desarrollado las siguientes propuestas: <br/>
Propuesta de Marketing<br/>
● En servicio Mobile ya que es un pilar en ingresos, seguir potenciando los planes más rentables.<br/>
● Listado de precios donde se diferencien los planes y sus beneficios debido a que genera confusión tanto a nivel empresa como masivo. <br/>
● Sugerimos realizar una auditoría a nivel precio/plan, consultores y a nivel cliente (jurídico) en el plan XL para el servicio B2B, para evaluar el rango de precios con el que se están efectuando las ventas debido a que no generan el volumen e ingresos rentables. Como consultora creemos que podría existir renegociaciones con el cliente jurídico producto en el rango de precio descubierto, debido al alto rango de precio existente, el cuál se sugiere analizar la situación actual de la competencia para evaluar el precio al cliente y evaluar su impacto en la cartera de clientes con el objetivo de seguir potenciando las ventas contratadas por las empresas, reduciendo así precios no competentes al mercado.<br/> 
● Estrategia para el PLAN M: Diseñar una campaña de marketing dirigida para el PLAN M para impulsar su volumen de ventas. Dado que es el más rentable por unidad, un aumento en sus ventas tendría un impacto significativo en las ganancias generales de la empresa.<br/>

Propuesta Gobierno de datos <br/>
● Sugerimos implementar procesos para poder limpiar y unificar los registros de los consultores, con el fin de evitar sesgos en la información y duplicados por errores internos. <br/>
● Detectamos planes que no tienen ingresos de volumen trimestral en la región Eje cafetero y en el servicio Pospago, sugerimos realizar las transacciones de pospagos y prepago en formatos separados para no generar confusión con registros nulos o sesgos en la misma información.<br/>

Propuesta canal de ventas 
● Sugerimos validar que los kioskos se encuentren en lugares estratégicos con el fin de generar mayor foco de marketing de la empresa y de las tiendas cercanas, y generar mayor tráfico de clientes, con la finalidad que los consultores puedan generar mayores ventas a público masivo. <br/>
● En Tiendas Express encontramos una rentabilidad baja por venta, evaluar la productividad de los consultores, analizar el plan de acción con objetivo de mejorar la productividad y las ventas.<br/>

Propuesta para el equipo de ventas <br/>
● Sugerimos darle foco a capacitaciones y meta, programa de capacitación de consultores que no se encuentran cumpliendo la meta mensual de 2 ventas diarias (99 consultores), evaluar si es necesario ajustar la meta ya que son 104 consultores, eso significa que la mayoría de los vendedores no cumplen la meta por ser un valor elevado en el tiempo de análisis. <br/>
● Teniendo en cuenta que encontramos consultores con rentabilidad óptima de planes B2B, sugerimos que los mejores consultores trabajen en las tiendas con foco a venta B2B (cliente jurídico), para enfatizar su labor y generar mayores crecimientos en este servicio. De igual manera, se requerirá de un plan de motivación por venta. <br/>
● Determinar los valores máximos en estado de Termination ya que no se tiene una meta donde se evalúe al asesor por termination, así mismo evaluar las causas de este estado, la consultora propone que no debe de ser mayor a tres (3) transacciones por mes con este estado. <br/>
● Para los estados de One-way Block y Two-Way Block, se sugiere hacer un seguimiento detallado de estos clientes, con el fin de que no sobrepasen el tiempo de mora y evitar su cambio de estado a Termination.<br/>

Propuestas evaluación competencia<br/>

● Realizar un análisis de mercado quincenalmente de las estrategias que tiene la competencia, evidenciamos que TELECOM ha obtenido buenos resultados de venta en comparación con empresas conocidas, esto significa que los clientes prefieren TELECOM por la relación precio/calidad, por el marketing abarcado en la región y campañas de masificación en los eventos realizados. Al tener un conocimiento constante de las estrategias de la competencia da lugar a que TELECOM pueda estar a la vanguardia y evite causalidad de termination por pérdidas significativas por precio.

 
### 6. Conclusiones del análisis
La consultora Data-Consulting SH ha desarrollado una evolución constante de la información obtenida por la empresa TELECOM, que desde la información abarcada de un excel de transacciones durante el segundo semestre del 2025, se logró desarrollar un análisis detallado de la información, pasando por un modelado de datos, la limpieza y validación de los mismo, un análisis estadístico, la solución de preguntas de negocio propuestas por el stakeholder y finalmente las propuestas relevantes que como consultora se desarrollaron para la empresa TELECOM con el fin de mostrar insight destacables y finalmente generar mayor rentabilidad.<br/>
Al cierre de este proyecto, nos llevamos una gran lección sobre la importancia del análisis de datos para la toma de decisiones en una empresa. Los meses que analizamos (abril, mayo y junio) Nos permitió ir más allá de los números superficiales para entender la realidad detrás de la operación de la empresa TELECOM.
Nuestro análisis mostró que las Tiendas son, sin duda, la columna vertebral del negocio, generando la mayoría de las ventas e ingresos. Sin embargo, el punto analizado más revelador fue descubrir que el segmento Mobile es más rentable por unidad que el B2B. Esto desafía la intuición y subraya la necesidad de revisar las estrategias de precios y los costos asociados a las ventas B2B.<br/>
Además, el bajo rendimiento general de los consultores y los problemas con los datos, como los múltiples IDs antes de buscar nuevas estrategias de venta, la empresa necesita solucionar sesgos en la información internos con un modelo de Gobierno de Datos.<br/>
En resumen, este proyecto nos enseñó que la rentabilidad no es solo una cuestión de volumen, sino de eficiencia. La empresa tiene una base sólida, pero necesita optimizar sus procesos, su equipo y sus estrategias de precios para garantizar un crecimiento sostenible. Finalmente, estamos convencidos de que las propuestas que hemos desarrollado son un primer paso crucial como consultoría Data-Consulting SH.<br/>

### 7. Agradecimientos
Almudena Alcázar de Velasco, Alex Ayala, Jesús Adraz, Cristian Lavia, Yohana Lopez, Caterina Abanoni y Unicorn Academy team.
