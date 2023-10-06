# Proyecto-Siniestros-Viales

**PROYECTO SINIESTROS VIALES**

<p style="text-align:justify">Este repositorio es un análisis de datos de los siniestros viales acaecidos en la Ciudad de Buenos Aires durante el período 2016 – 2021. Se procede a detallar las carpetas que contiene:

                                                                                                                             
-![data](https://github.com/andreasoria2022/PROYECTO-SINIESTRO-VIALES/assets/105015078/de5ff90e-1bfc-481a-9a0c-0ab650f0b0e2)  contiene los siguientes archivos:

<p style="text-align:justify">**homicidios.xlsx**  es un archivo con extensión xlsx brindado por la página Buenos Aires Data que nos informa sobre los siniestros viales con víctimas fatales ocurridas en la Ciudad desde el año 2016 – 2021.  Los datos incluyen fecha y ubicación del hecho y tipo de transporte involucrados.

<p style="text-align:justify">**lesiones.xlsx** es un archivo con extensión xlsx brindado por la pagina Buenos Aires Data que nos informa sobre las lesiones en siniestros viales ocurridos en la Ciudad desde el año 2019 – 2021. Los datos incluyen fecha, ubicación del hecho y tipo de transporte involucrado.

<p style="text-align:justify">**homicidos.csv** este archivo es el resultado de haber realizado el proceso de extracción, transformación y carga de datos  y contiene los datos de los siniestros viales con víctimas fatales ocurridas en la Ciudad de Buenos Aires desde el año 2016 -2021 

<p style="text-align:justify">**lesiones.csv** este archivo es el resultado de haber realizado el proceso de extracción, transformación y carga de datos y contiene los datos de las lesiones de los siniestros viales ocurridas en la Ciudad de Buenos Aires desde el año 2019 -2021 

<p style="text-align:justify">**resumen_EDA.xlsx**: este archivo es un resumen del EDA en Excel.

                                                                                                                             
 ![etl](https://github.com/andreasoria2022/PROYECTO-SINIESTRO-VIALES/assets/105015078/4a4fadf3-cb8f-48a4-a301-00fa5b0cac4c)  contiene el siguiente archivo:
 
<p style="text-align:justify">**ETL.ipynb**: es un archivo notebook en el que se realiza el proceso de extracción, transformación y carga de los datos de los siniestros viales tanto de lesiones como los que tienen víctimas fatales. Los datos de los siniestros viales con víctimas fatales que fueron extraídos de la página Buenos Aires Data no poseían duplicados y pocos nulos en  datos de la ubicación. Se eliminaron  la columna año, la columna mes y también la columna día ya que la columna fecha contenía toda esta información. En cuanto a los datos de las lesiones de los siniestros viales extraídos de la página Buenos Aires Data no poseía duplicados y si muchos nulos en cuanto a los datos de la ubicación del hecho. De este dataset también se eliminaron  la columna año, la columna mes y también la columna día ya que la columna fecha contenía toda esta información. Este proceso de ETL dio origen a los archivos homicidos.csv y lesiones.csv que fueron incorporados en la carpeta Data.


                                                                                                                            
 ![EDA](https://github.com/andreasoria2022/PROYECTO-SINIESTRO-VIALES/assets/105015078/1d15a0ab-3279-43eb-81a8-33f35d830941)  contiene el siguiente archivo:

<p style="text-align:justify">**EDA.ipynb**: es un archivo notebook en los que se realizó el análisis exploratorio de datos de los siniestros viales tanto los que tuvieron víctimas fatales como los que tuvieron lesiones como consecuencia del hecho. Se realizó el análisis de los siniestros por año, según el vehículo que ocupaba la víctima, según el vehículo que ocupaba el acusado del hecho para los cuales se realizaron gráficos de barras también se llevó a cabo el análisis estadístico de las variables numéricas, gráficos de cajas, gráficos de dispersión, mapa de calor, etc.

-	<p style="text-align:justify">**Readme**: es un detalle de lo que vamos a encontrar en el repositorio. Y vamos a encontrar un informe.
  

**INFORME DE LOS SINIESTROS VIALES**

<p style="text-align:justify">En la Argentina los siniestros viales son una de las principales causas de muerte. Según un informe realizado por Dirección de Estadística Vial de Argentina este es el perfil de las víctimas fatales en siniestros que me pareció importante mencionar para crear conciencia sobre la gravedad del problema.

![fra](https://github.com/andreasoria2022/PROYECTO-SINIESTRO-VIALES/assets/105015078/5cf46cfa-acc7-44bb-879c-2daf88640755)

**Causas de accidentes**:

**Uso de teléfonos móviles**:
<p style="text-align:justify">El teléfono celular se ha convertido en una de las principales causales de accidentes de tránsito ya sea para conductores como peatones. Para 2020, mientras que el 18,2% de los peatones cruzan la calle utilizando su teléfono móvil, entre los vehículos particulares que circulan por Buenos Aires a diario (cerca de 1.400.000), el 17,2% de los conductores utilizan un celular mientras conducen.
De acuerdo con las cifras oficiales de la ANSV, los seis segundos que una persona tarda contestar una llamada escribir un mensaje de WhatsApp, a una velocidad de 100 km/h, equivalen a recorrer una distancia de 166 metros, luego de reaccionar y frenar.

**Exceso de alcohol**:
<p style="text-align:justify">El alcohol está presente en uno de cada cuatro siniestros viales y las principales víctimas de este tipo de accidentes son los jóvenes de entre 15 y 34 años, según datos del Observatorio Vial.
Incorrecto uso del casco:
Los motociclistas que usan el casco tienen un 73% menos de mortalidad que los que no lo usan. A su vez, quienes utilizan protección para su cabeza tienen hasta un 85% menos de lesiones graves que aquellos que conducen sus motos sin casco.

**Cinturón de seguridad**:
<p style="text-align:justify">Según cifras del Ministerio de Transporte, en Argentina, la mitad de los vehículos – 49,3% – circulan con todos sus ocupantes protegidos mediante el uso del cinturón de seguridad.
<p style="text-align:justify">Sin embargo, su uso varía de acuerdo a la posición que ocupa cada persona dentro del coche. Es decir, sólo el 55% de los conductores utilizan el cinturón, proporción que se reduce al 42,8% entre los que viajan en el asiento del acompañante y al 19,9% entre ocupantes de las butacas traseras.
<p style="text-align:justify">Un informe de la ANSV revela que, en caso de choque, su uso reduce la posibilidad de sufrir lesiones cerebrales en un 33% en el caso del conductor y de un 56% en el pasajero. También disminuye la posibilidad de sufrir fracturas de cráneo en un 18% y heridas faciales en un 45% para el conductor y 64% para el acompañante. Además, reducen un 45% el riesgo de muerte de los ocupantes de las plazas delanteras y un 44% de los ocupantes de las plazas traseras.

<p style="text-align:justify">Ahora vamos a proceder a estudiar los datos de los siniestros viales que se produjeron en la CABA (Ciudad Autónoma de Buenos Aires). En el periodo 2016-2019 se registró un promedio anual de 145 víctimas fatales a 30 días y un promedio de 1200 heridos graves.
 <p style="text-align:justify">Se realizará el analisis de Kpis de los siniestros viales. 

![siniest](https://github.com/andreasoria2022/PROYECTO-SINIESTRO-VIALES/assets/105015078/02c753fe-a99d-4930-b9f5-8ca000fb9f92)

![moto](https://github.com/andreasoria2022/PROYECTO-SINIESTRO-VIALES/assets/105015078/19228edc-b2e9-4fb3-8974-72b962bacc2c)

<p style="text-align:justify">Los Kpis serán incluidos en un dashboard interativo, con filtros. También se realizará un analisis claro con gráfico coherentes y estéticos.


