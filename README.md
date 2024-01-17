## Homicidios por Accidentes Viales en la Ciudad Autonoma de Buenos Aires Argentina

#### Introduccion
En este proyecto se simula el rol de un Data Analyst que forma parte de una consultora, a la cual el Observatorio de Movilidad y Seguridad Vial (OMSV), 
centro de estudios que se encuentra bajo la órbita de la Secretaría de Transporte del Gobierno de la Ciudad Autónoma de Buenos Aires, le va a solicitar
la elaboracion de un proyecto de analisis de datos, con el proposito de generar informacion que ayude a la disminucion de victimas fatales en los accidentes viales.

El entregable es un Dashboard que debe facilitar el analisis y la interpretacion de la informacion proporcionada por esta misma entidad.

#### Definicion
Los siniestros viales, también conocidos como accidentes de tráfico o accidentes de tránsito, son eventos que involucran vehículos en las vías públicas y que pueden tener 
diversas causas, como colisiones entre automóviles, motocicletas, bicicletas o peatones, atropellos, choques con objetos fijos o caídas de vehículos. Estos incidentes pueden 
tener consecuencias que van desde daños materiales hasta lesiones graves o fatales para los involucrados.

#### Justificacion
En Argentina, cada año mueren cerca de 4.000 personas en siniestros viales. Aunque muchas jurisdicciones han logrado disminuir la cantidad de accidentes de tránsito, esta sigue 
siendo la principal causa de muertes violentas en el país. Los informes del Sistema Nacional de Información Criminal (SNIC), del Ministerio de Seguridad de la Nación, revelan que 
entre 2018 y 2022 se registraron 19.630 muertes en siniestros viales en todo el país. Estas cifras equivalen a 11 personas por día que resultaron víctimas fatales por accidentes de tránsito.

Solo en 2022, se contabilizaron 3.828 muertes fatales en este tipo de hechos. Los expertos en la materia indican que en Argentina es dos o tres veces más alta la probabilidad de que 
una persona muera en un siniestro vial que en un hecho de inseguridad delictiva.

#### Informacion
El dataset fue proporcionado por el Observatorio de Movilidad y Seguridad Vial (OMSV), el cual es una archivo de excel con varias pestañas, varias de ellas contiene informacion sobre las columnas 
de las tablas. 

Una de las pestañas tiene por nombre HECHOS y alli se encuentra informacion como la fecha, la ubicacion, cantidad de victimas, la victima y el acusado. 

La otra tiene por nombre VICTIMAS, en ellal se encuentra informacion sobre el sexo, edad, rol de los fallecidos en el siniestro.

En este link puede encontrar el dataset y toda la informacion relacionada https://data.buenosaires.gob.ar/dataset/victimas-siniestros-viales

#### Programas Usados
Para este proyecto se uso  python con junto con varias librerias como Seaborn, Pandas, Numpy etc. para el procesamiento de los datos.
Para la Elaboracion del Dashboard interactivo se uso Power BI.

### Desarrollo
#### ETL - EDA
En el Jupyter Notebook llamamdo EDA se encuentra todo el proceso que se le hizo al dataset dado.
En primer lugar el ETL, donde se procesaron los datos duplicados, faltantes, nulos, se estandarizó el nombre de las columnas, se eliminaron columnas y se imputaron algunos valores. 
En segundo lugar el EDA, donde se hizo el analisis exploratorio de los datos, alli se analizo el numero de victimas por año, mes, dia de la semana y por intervalos de tiempo de horas durante el dia, 
para ver el comportamiento y entender algunas tendencias. Tambien se hicieron analisis de numero de victimas por tipo de calle, se era un cruce o no, los medios o situacion de las victimas y de los acusados al momento del accidente,
cantidad de victimas segun el sexo, rol y la edad.

#### Dashboard
En el archivo de PowerBI PI2 Data Analytics homicidios se encuentran todas la graficas necesarias para mostrar los hallazgos que hicieron sobre los datos.
Tambien se calcularon algunos KPI's como la tasa de homicidios en siniestros viales, su fórmula es: 

(Número de homicidios en siniestros viales / Población total) * 100,000,

la cantidad de accidentes mortales de motociclistas en siniestros viales cuya formula es: 

(Número de accidentes mortales con víctimas en moto en el año anterior - Número de accidentes mortales con víctimas en moto en el año actual) / (Número de accidentes mortales con víctimas en moto en el año anterior) * 100

y por ultimo la cantidad de accidentes mortales en los cruces y su formula es:

(Número de accidentes mortales con víctimas en los cruces en el año anterior - Número de accidentes mortales con víctimas en los cruces en el año actual) / (Número de accidentes mortales con víctimas en los cruces en el año anterior) * 100

Finalmente se sacaron varias conclusiones y se hicieron varias recomendaciones.



