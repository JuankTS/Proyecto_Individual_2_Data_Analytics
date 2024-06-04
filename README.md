# <div align='center'> Proyecto Individual 2 Data Analytics </div>
# <div align="center">Análisis de Siniestros Viales en Buenos Aires</div>
# <div align='center'> ![alt text](/Imagenes/image.png) </div>


## Tabla de Contenido
- [Introducción](#introducción)
- [Los Datos y su Análisis](#los-datos-y-el-análisis)
- [Conclusiones](#conclusiones)
- [Explicación del Repositorio](#explicación-del-repositorio)
- [KPIs](#kpis)
- [Visualización](#visualización)

## Introducción.
Los siniestros viales, conocidos también como accidentes de tráfico o accidentes de tránsito, son eventos que involucran vehículos en las vías públicas y que pueden tener diversas causas, como colisiones entre automóviles, motocicletas, bicicletas o peatones, atropellos, choques con objetos fijos o caídas de vehículos. Estos incidentes pueden tener consecuencias que van desde daños materiales hasta lesiones graves o fatales para los involucrados.

Las tasas de mortalidad relacionadas con siniestros viales suelen ser un indicador crítico de la seguridad vial en una región. Estas tasas se calculan, generalmente, como el número de muertes por cada cierto número de habitantes o por cada cierta cantidad de vehículos registrados. Reducir estas tasas es un objetivo clave para mejorar la seguridad vial y proteger la vida de las personas en la ciudad.

Para este proyecto, se nos pide desarrollar el rol de un analista de datos con el fin de generar información que permita tener una visión general de cómo se ha venido desarrollando la situación de los siniestros viales y obtener información valiosa para poder hacer frente a este escenario que ocurre en la ciudad de Buenos Aires, Argentina. Para ello, se dispone de un dataset sobre homicidios en siniestros viales acaecidos en la Ciudad de Buenos Aires durante el periodo 2016-2021. Este dataset se encuentra en formato xlsx y contiene dos hojas llamadas: **hechos** y **víctimas**.

## Los Datos y su Análisis.
Para el análisis de los datos se abordan desde distintas perspectivas, ya que en la base de datos hay variedad de tipos de datos que nos permiten hacer un análisis tanto cualitativo como cuantitativo. Los datos vienen divididos de la siguiente forma:
- **HOMICIDIOS_BUENOS_AIRES**: Contiene la información de ambas bases.
- **HECHOS**: Contiene una fila por hecho con id único y las variables temporales, espaciales y participantes asociadas al mismo.
- **VICTIMAS**: Contiene una fila por cada víctima de los hechos y las variables edad, sexo y modo de desplazamiento asociadas a cada víctima. Se vincula a los HECHOS mediante el id del hecho.
- **Diccionario de Datos Siniestros Viales**: Contiene la información de cada variable en las bases de datos.

Una vez entendida la composición de los datos, se realizó el cargue, limpieza y análisis, en el cual se analizaron desde múltiples puntos de vista y se focalizaron en variables que pueden ser útiles, tales como la edad, como muestra la siguiente gráfica.

# <div align='Center'> ![alt text](/Imagenes/Edades.png) </div>

Este histograma nos muestra en qué intervalo de edad están concentradas las personas que se ven involucradas en siniestros viales. Como se puede observar, la edad de las personas que mayoritariamente se ven involucradas en este tipo de accidentes ronda entre los 20 y 38 años.

Otro dato importante que se pudo extraer de los datos es el siguiente:

# <div align='Center'> ![alt text](/Imagenes/Horas.png) </div>
Este histograma nos muestra las horas en las que más ocurren accidentes en la ciudad de Buenos Aires. Se puede ver que la mayor incidencia de accidentes se encuentra entre las 5 de la mañana y casi las 9 de la mañana.

Tambien podemos ver la cantidad de accidentes por años, lo cual nos puede dar una visión de como se comportan las tendensias, en el tiempo y dentro de los mismos años.
#  <div align='Center'> ![alt text](/Imagenes/Años.png) </div>


Estos son algunos de los datos claves que se pudieron extraer del análisis. Para ver el análisis completo puede dirigirse al archivo **EDA.ipynb**.

## KPIs.

Para este análisis se propuso crear 2 KPIs (Indicadores Claves de Rendimiento):

1. ***Reducir en un 10% la tasa de homicidios en siniestros viales de los últimos seis meses, en CABA, en comparación con la tasa de homicidios en siniestros viales del semestre anterior***.

    > *Definimos a la tasa de homicidios en siniestros viales como el número de víctimas fatales en accidentes de tránsito por cada 100.000 habitantes en un área geográfica durante un período de tiempo específico. Su fórmula es:* <center>
$\frac{\text{Número de homicidios en siniestros viales}}{\text{Población total}} * 100000$<br><br>
</center >

2. ***Reducir en un 7% la cantidad de accidentes mortales de motociclistas en el último año, en CABA, respecto al año anterior***.

    > *Definimos a la cantidad de accidentes mortales de motociclistas en siniestros viales como el número absoluto de accidentes fatales en los que estuvieron involucradas víctimas que viajaban en moto en un determinado periodo temporal. Su fórmula para medir la evolución de los accidentes mortales con víctimas en moto es:*<center>
$\frac{\text{Víctimas en moto del año anterior - Víctimas en moto del año actual}}{\text{Víctimas en moto del año anterior}}*100$<br>
<br></center>

## Conclusiones.
A partir de un análisis rudimentario de los datos se pudo extraer:
- Las personas que se ven mayoritariamente involucradas en siniestros viales se encuentran entre los 20 y 38 años de edad.
- Las horas en las que más se registran accidentes viales en Buenos Aires son entre las 5:00 am y casi las 9:00 am.
- En el año 2019 se evidencia un claro descenso en el número de accidentes viales, pero el pico más bajo se registra en el año 2020, lo cual puede ser una situación dada por la pandemia que produjo el COVID-19.
- El 61,64% de los accidentes se producen en avenidas.
- En el cuarto trimestre del año los siniestros viales tienden al alza, esto puede ser producido por un aumento en la densidad poblacional momentáneo producido por el turismo u otros factores.
- El 76,65% de las víctimas son del sexo masculino.
- La comuna 1 tiene el mayor número de siniestros registrados.

## Explicación del Repositorio.
- **Carpeta Data**: Contiene las bases de datos usadas para el proyecto.
- **EDA.ipynb**: Contiene el cargue, las transformaciones y el análisis que se realizaron a los datos.
- **DashBoards.pbix**: Contiene el dashboard interactivo hecho con los datos.
- **Imagenes**: Contiene las imagenes usadas.

## Visualización.
Puedes ver el dashboard interactivo generado descargando el archivo `DashBoards.pbix`.

<div align="center">
  <a href='https://www.linkedin.com/in/juan-camilo-torres-salas-907749265/'>
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"alt="Linkedin"/>
  </a>
</div>

