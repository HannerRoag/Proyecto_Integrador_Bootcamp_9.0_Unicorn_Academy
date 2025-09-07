<h1>Proyecto integrador del Bootcamp 9.0 por UNICORN ACADEMY</h1> 

![Static Badge](https://img.shields.io/badge/Own%20Project%20-%20Proyecto%20Propio?style=for-the-badge&color=black)





# Introducción
Proyecto integrador realizado en equipo con Sofía Gonzalez como ejercicio final del Bootcamp 9.0, donde se tomaron datos de una empresa real, datos suministrados por varios documentos en Excel de los meses de enero a julio del 2025. Los datos fueron avalados y por protección de datos , se realizó limpieza, análisis estadistico descriptivo, una visualización mediante dashboard y se realizó propuestas de valor, utilizando Excel, MySQL, Google Colab y Power BI


 
<h3>1. Data source</h3> 
 Empresa colombiana de telecomunicaciones - TELECOM (Empresa creada por protección de datos) 
 
 
### 2. Objectives
#### 2.1 Main objective
- Using external information, development knowledge using python.
#### 2.2. Specific objetives 
- Development libraries and methods on Python.
- Analyze information provided for INE.
- Visualyze relevant information.

### 3. Tecnologies
![SQL](https://img.shields.io/badge/-Sql-f29111?style=for-the-badge&logo=mysql)
![Jupyter](https://img.shields.io/badge/-Jupyter-white?style=for-the-badge&logo=Jupyter)
![Python](https://img.shields.io/badge/-Python-9370DB?style=for-the-badge&logo=Python)

### 4. Key question
##### Do the trends for the male and female groups follow the same pattern?

### 5. Development of analysis
#### 5.1 Connection INE ![Jupyter](https://img.shields.io/badge/-Jupyter-white?style=for-the-badge&logo=Jupyter)
The connection is established with an external data source, the connection is adjusted to the required of the data source.
- Import libraries as pandas, requests, datetime.
- Function that take a code INE, connection and return a Json with requested data.
- Read the archive with the serie code of INE.
- Take the attributes of each data serie.
- Make the dataframe with data lists.
#### 5.2 Daraframe exploration ![Jupyter](https://img.shields.io/badge/-Jupyter-white?style=for-the-badge&logo=Jupyter)
- Use the methods as .rename(), .max(), .min(), .mean(), .unique(), .split(), .groupby(), .agg(), .transform(), .apply(). <br/>
.info(), .year(), .month(), .to_dataframe(), .dir(), .shift(), .assign(), .columns(), .loc(), .cut(), .sample().
#### 5.3. DDSS Connection ![SQL](https://img.shields.io/badge/-Sql-f29111?style=for-the-badge&logo=mysql) ![Jupyter](https://img.shields.io/badge/-Jupyter-white?style=for-the-badge&logo=Jupyter)
- Import or libraries as mysql-connect-python, pymysql, sqlalchemy.
- Configuration of connection.
- Consult data sources.
- Make connections.
- Close connection.
- Save dataframe as .csv using method .to_csv().
#### 5.4 Visualization in python ![Jupyter](https://img.shields.io/badge/-Jupyter-white?style=for-the-badge&logo=Jupyter)
- Import libraries as os, numpy, pandas, datetime, matplotlib.piplot, seaborn.
- Use methods as .read_csv(), .info(), .to_datatime(), .plot(), .figure(), .show(), .xlabel(), .ylabel(), .title().

### 6. Conclusions of analysis
This project involved extracting information from an external data source and integrating it into a local environment using Jupyter. I was able to clean, modify, and adapt the data to answer key questions. I observed variation within the Spanish community over time. <br/>
During the process, I encountered some challenges: the data was not in a clean format, and I had to manage the diversity of the datasets. I included both evident and less evident demographic information, such as gender, age, and customer type.<br/>
I worked with three main data groups: total population, male population, and female population. I first analyzed overall population trends and then focused on gender-specific variations.<br/>
Although I validated the data using semiannual values, I faced some interpretation challenges—typical in analytical work. Eventually, I decided to restructure the data using decades instead of semiannual periods to make the insights clearer.<br/>
After data cleaning, manipulation, analysis, and interpretation, I began to think about long-term improvements. If this data could be uploaded to a collaborative database, it would allow other users to work with clean, structured data. It's important to create backup files so users can return to specific stages of analysis. In the end, I transformed the dataset into a lightweight CSV archive for easier sharing and use.<br/>
Finally, after checking the graph, I observed that from 1970 to 1980, there was a noticeable upward slope, indicating a faster growth rate. It was a period of strong growth, with the population rising from around 34 million to approximately 38 million—this was also confirmed numerically.<br/>
Then, I noticed that the growth rate began to slow down. From 1980 to 1990, when analyzing by decade, the vertical change was minimal, showing almost no variation. This trend continued in the following decade, from 1990 to 2000. I also confirmed these patterns using the numerical data series.<br/>
Later, I identified subtle nuances in the data, which helped me better understand the overall trend. It's important that graphs are always supported by numerical values, and vice versa—numbers should also be visualized through graphs.<br/>
After the year 2000, I noticed a significant increase in growth. However, before 2010, the growth rate began to slow again, with the slope becoming less steep. Then, around 2020, the growth rate increased once more, and the slope became steeper again.

### 7. Acknowledgements
Almudena Alcázar de Velasco, Jesús Adraz, Cristian Lavia, Yohana Lopez, Caterina Abanoni and Unicorn Academy team.
