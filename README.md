# Analisis de plataformas de cursos online masivos

En el presente proyecto se analiza la data provista sobre las plataformas de cursos online masivos edX, Udemy y Coursera.
Dentro de los directorios del repositorio se encuentra:
 - la carpeta EDA se encuentra el analisis exploratorio de los datos y su transformacion. Dentro esta la subcarpeta Dataset con la data y el archivo EDA_transformacion.ipynb donde se realiza y se explica el EDA y las transformaciones.
 - En la carpeta Presentacion_Power_BI se encuentra el archivo de power BI Analytics.pbix que contiene una precentacion con el dashboard realizado para el proyecto.

## Analisis
A continuacion vamos a analizar la informacion disponible de las compañias de cursos online masivos edX, Udemy y Coursera. con el objetivo de aconsejar a una nueva empresa de esta area cuales son los cursos mas recomendados para que comience a ofrecer.

<br>***Nota**: todas las graficas y visualizaciones que se describan aca pueden ser encontradas en la presentacion de power BI **Analytics.pbix** dentro de la carpeta **Presentacion_Power_BI**.*

### edX
Con edX hay que tener en cuenta que los cursos son gratuitos, y solo pagan los estudiantes que quieran adquirir el certificado, y ya que no se tienen datos de cuantos de los matriculados pagaron o van a pagar el certificado, las cifras de ventas corresponden a ventas potenciales, que es el producto de los matriculados por el costo del certificado.

En la primera grafica se puede ver que dentro del top 5 de cursos con mas nivel de ventas, 3 pertenecen a areas de computacion/programacion, y en este caso de edX no hay mucha variacion al filtrar por el nivel del curso:
- en el nivel introductorio, 3 son de computacion y web
- en intermedio, 3 son de programacion
- en avanzado, 2 son de data, 1 de IA y 1 de machine learning

### Udemy
Con udemy tenemos que 4 del top 5 son de desarrollo web, filtrando de acuerdo al nivel de los cursos:
- en principiante las 5 son de desarrollo web
- en intermedio 4 son de programacion y software.
- en el caso del nivel experto tenemos un cambio a lo que veniamos viendo y es que las 5 pertenecen al area de finanzas y manejo de stock

### Coursera
En el caso de coursera vamos a mirar la cantidad de reviews, donde se observa un comportamiento similar a los del nivel de ventas, podemos ver que en el top 5 de los cursos con mas reviews, y que por ello podemos asumir son tambien los mas concurridos, 4 pertenecen a tecnologia

## Wordclouds
En los wordclouds podemos ver las palabras mas frecuentes en los titulos de los cursos, para el caso de edX encontramos introduction, data, science y en menor medida managemnt, python, programing. Estas palabras concuerdan con las graficas anteriores donde vimos que los cursos con mas ventas son los relacionados con programacion y computacion, por lo que tiene logica que edX cuente con gran cantidad de este tipo de cursos.
Al realizar filtros por nivel de los cursos vemos que desaparecen las palabras del tipo introduction y fundamentals, pero las palabras relacionadas con tecnologia siguen destacando.

En Udemy llama la atencion que hay varias palabras relacionadas con diseño web, como javascript, html y html5, wordpress. filtrando por nivel principiante vemos que estas mismas palabras toman mas relevancia, pero curiosamente dos de las palabras mas grandes son piano y guitarra que serian de musica. en experto la palabra mas grande quitando advanced y options que no son muy especificas, es la palabra trading, que como ya vimos los cursos con mas ventas en udemy son de comercio.

En Coursera se sigue la misma tendencia en cuanto a que los cursos con mas reviews son los relacionados con tecnologia, y no hay mucha variacion si filtramos por rating, por lo que no parece haber una relacion muy directa entre algun tema especifico con el buen o mal rating.

## KPI
Como KPI se propone realizar un seguimiento cada cierto tiempo al promedio de estudiantes por curso, si el resultado en muy pequeño, teniendo en cuenta la cantidad total de alumnos, podria ser un indicativo de dos situaciones:
- por un lado que se estan ofreciendo muchos cursos que atraen pocas personas
- y que exista una alta dependencia de unos pocos cursos, es decir que un porcentaje muy alto de las ventas este concentrado en un numero reducido de cursos, algo que vuelve mas suceptible a la empresa ante los cambios de las tendencias o modas, ya que si el tema de estos cursos pierde popularidad en corto plazo y se reduce drasticamente las inscripciones, los ingresos de la empresa podrian recibir un fuerte golpe, al depender en exceso de estos cursos especificos. Por ello tambien se aconseja no solo sacar el promedio de estudiantes por curso, sino tambien por las areas en las que estan catalogadas los cursos.

Una segunda KPI recomendada, aunque ajena a la data proporcionada, es la del promedio de estudiantes por cursada de cada curso por separado, en determinado tiempo, como puede ser anual o semestral por ejemplo, esto permite llevar un mejor control del crecimiento o decrecimiento del curso, asi como compararlo con el de los demas cursos, y tambien permite determinar si hubo una anomalia con la cantidad de inscripciones en determinado periodo.