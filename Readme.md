<div>
<p align=center><img src="images/logo_a777HD.png" height=200><p>

# <h1 align=center> **PROYECTO INDIVIDUAL Nº 2** </h1>

# <h1 align=center>**`ROAD CASE`**</h1>
</div>
<p align="center">
<img src="images/PazAv_deaths.png"  height=300>
</p>

<hr>  

# ***ESTUDIO SOBRE LA MORTALIDAD VIAL EN CABA***

## CONTEXTO
El Observatorio de Movilidad y Seguridad Vial, el cual depende de la Secretaría de Transporte del Gobierno de CABA, me solicitó la elaboración de un estudio con el fin de generar información muy relevante que le permita a la Secretaría tomar medidas para disminuir la cantidad de víctimas fatales de los accidentes viales en la ciudad esto debido a la elevadísima tasa de mortandad generada por estos hechos. Ya que sin exagerar en BA, las víctimas viales eran mayores que las generadas por cualquier hecho delictivo. Tanto era así que, 11 personas morían diariamente producto de estos accidentes y otras tantas quedaban con lesiones de diversa gravedad.
## DESARROLLO DEL ESTUDIO

Una vez que tenía definido que debía realizar un análisis de datos sobre esta problemática, lo estructuré en 4 etapas bien definidas, las cuales detallo a continuación:

## 1. ETL - Data Engineer
En esta etapa de Ingeniería de Datos, realicé un proceso de ETL, extracción, transformación y carga de datos, donde se recibieron 2 archivos EXCEL con datos de los hechos y las víctimas tanto de los homicidios como de las lesiones generadas en algunos casos.

Al final de esta etapa, se crea un dataset en formato CSV que servirá para trabajar en la siguiente etapa y se guardarán en la carpeta: Datasets.
#### Notebook Links:
- *ETL-Homicidios:* https://github.com/jalcantara777/RoadCase/blob/main2/1_Mandatory_ETL.ipynb
- *ETL-Lesiones:* https://github.com/jalcantara777/RoadCase/blob/main2/1_Supplementary_ETL.ipynb

#### Data Sources:
- *XLS-Homicidios:* https://github.com/jalcantara777/RoadCase/blob/main2/Datasets/homicidios.xlsx
- *XLS-Lesiones:*   https://github.com/jalcantara777/RoadCase/blob/main2/Datasets/lesiones.xlsx
- *XLS-Comunas:*    https://github.com/jalcantara777/RoadCase/blob/main2/Datasets/comunas.xlsx

## 2. EDA - Exploratory Data Analysis
En esta etapa de Análisis Exploratorio de Datos, se realizaron la conversión y completado de los datos, también se verificaron y eliminaron los datos nulos, duplicados, outliers y el cambio en el formato de algunos datos para posteriormente realizar un análisis de correlación entre las variables que están en estos datos depurados. En esta etapa no se crea un dataset para trabajar en la siguiente etapa ya que utilizará el mismo que se uso para esta etapa.

#### Notebook Link: https://github.com/jalcantara777/RoadCase/blob/main2/2_EDA.ipynb
#### Data Source: https://github.com/jalcantara777/RoadCase/blob/main2/Datasets/deadly_acc.csv

## 3. DV - Data Viz
Después de haber realizado un exhaustivo estudio estadístico y de análisis de datos y gráficos, ahora sólo queda plasmar lo encontrado en la etapa anterior en un informe interactivo y visual, es decir, un dashboard, el cual fue realizado con la herramienta de PowerBI.
Luego de realizar un completo análisis gráfico y superpuesto entre las varias variables que se correlacionaban, encontradas en la etapa anterior, se procedió con el desarrollo de los 3 KPI detallados a continuación:
- 1. Reducir en un 10% la tasa de homicidios en siniestros viales de los últimos seis meses, en CABA, en comparación con la tasa de homicidios en siniestros viales del semestre anterior.
- 2. Reducir en un 7% la cantidad de víctimas mortales de motociclistas en el último año, en CABA, respecto al año anterior.
- 3. Reducir en un 15% la cantidad de víctimas fatales de peatones en el último semestre, en CABA, respecto al semestre anterior.

#### Dashboard Link: 
https://app.powerbi.com/view?r=eyJrIjoiOGI3Y2I2MjEtNzM5Ni00ODA2LTgwNDctNDg3ZjE0YTdmNTk4IiwidCI6Ijc1MDRlMzE4LThlMWUtNGQ1NS1iZmZkLTg3NWI0ZGVlODI2MCIsImMiOjR9&embedImagePlaceholder=true&pageName=ReportSectiondb8385b8c9ae951d54a5

#### Demo Dashboard Video Link: https://youtu.be/OJMJCZUxB_U

#### Data Source: 
- Processed data: https://github.com/jalcantara777/RoadCase/blob/main2/Datasets/deadly_acc.csv
- CABA Population data: https://www.indec.gob.ar/ftp/cuadros/poblacion/proy_1025_depto_buenos_aires.xls (fue modificado)
- Death rate KPI calculate: https://github.com/jalcantara777/RoadCase/blob/main2/Datasets/Sem_proy.xlsx

## 4. Conclusiones
- 2 de los 3 objetivos se cumplieron. Se debe monitorear el KPI de víctimas fatales producidas por moto.
- Colocar mayor número de controladores o policías de tránsito, a la vez que, incrementar el número de semáforos, si es necesario, a lo largo de la Av. Gral. Paz, haciendo incidencia en los cruces de las comunas 12, 9 y 8.
- Realizar prevención sobre los conductores Masculinos , teniendo mayor énfasis en los que estén en rango de edad entre 20 a 40 años de las comunas 1, 4 y 9.
- Asignar efectivos policiales adicionales en las horas matutinas de desplazamiento de los trabajadores hacia sus centros laborales.
- Concientizar a los motociclistas y peatones sobre los mayores riesgos de transitar por las avenidas cerca a los cruces de forma despreocupada e irresponsable.
- Monitorear las comunas 1, 4, 9, 8 y 7 en cuanto a los resultados de KPI.
- Colocar controles en horarios nocturnos cercanos a la madrugadas sobre avenidas en los fines de semana.

## 5. Herramientas y plataformas web usadas
- Visual Studio Code: editor de código
- Python: lenguaje de programación (versión 3.11)
- PowerBI Desktop: servicio de análisis de datos (2.128)
- Excel: hoja de cálculo
- GitHub: repositorio del proyecto y fuente para la API
- GitBash: terminal con Linux-core
- Google Maps Platform: mapas satelitales en la web
- Dynamica Labs: servicio Google Maps
- PowerBI service: servicio en la nube de PowerBI

## 6. Datos de CONTACTO
- Nombre: José Alcántara 
<br>
<img src="images/Avatar_DA.png" alt="Imagen no encontrada" height=200px>
- Correo Electrónico: jalcantara777@yahoo.com
<br>
<img src="images/NumWhatsapp2.jpg" alt="Imagen no encontrada" height=50px>
<a href="https://github.com/jalcantara777/"><img src="images/GitHub_logo.jpg" alt="Imagen no encontrada" style="font-size: 30px;height: 50px;"></a>
<a href="https://www.linkedin.com/in/jalcantara777/"><img src="images/Linkedin_logo.png" alt="Imagen no encontrada" style="font-size: 30px;height: 50px;"></a>