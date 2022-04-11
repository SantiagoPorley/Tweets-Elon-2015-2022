Análisis de los Tweets de Elon Musk

Introducción y Resumen:
Elon Musk es una de las figuras más interesantes de los últimos tiempos es el CEO y jefe ingeniero de SpaceX, padre de familia, CEO de Tesla, billonario, director y usuario habitual de Twitter entre otros.

Twitter es el medio elegido por Elon para expresarse, realizar anuncios sobre sus compañías y compartir sus ideas, opiniones y memes.
Más de 77 millones de seguidores están atentos a sus publicaciones que ya superan las 15000 entradas y muchas de ellas han tenido un gran impacto en el mundo, sobre todo en campos políticos y económicos.

Por medio de sus Tweets se puede tener un vistazo de ideas, su mundo y vida, por lo que analizar sus tweets puede ser de lo más interesante.


En este estudio se realizan las siguientes preguntas: ¿Cuáles son los tweets más populares de Elon? ¿De qué tratan?,¿A qué horas twittea? ¿Qué nos dice de su estilo de vida el momento en que twittea Elon?
También intentar visualizar brevemente la existencia de una relación en el crecimiento de Cripto con sus posts en Twitter. 

Data
Los archivos utilizados para armar el dataframe con la información de los Tweets históricos fueron proporcionados por la profesora del curso, a excepción del csv 2015-2020 que fue extraído del sitio Kaggle.

El dataframe tweet_df está formado por las siguientes columnas:

nombre
Id
date
time
tweet
retweet_count
replies_count
likes_count
descripción
Número de identificación del tweet, único.
Fecha del tweet A/M/D
Hora del tweet, inicialmente H/M/S
String conteniendo el tweet
Cantidad de retweets
Número de respuestas al tweet
Cantidad de likes
Data group
Numeric integer
Categorical ordinal
Categorical ordinal
Categorical nominal
Numeric integer
Numeric integer
Numeric integer
Python obj class
int
Str 
str
str
int
int
int





Para el dataframe de DogeCoin se utilizó un archivo .csv extraído de Kraggle con valores históricos de la criptomoneda.
 El dataframe contine las siguientes columnas:

nombre
date
open
descripción
Fecha A/M/D.

Valor de la moneda al comienzo del día
Data group
Categorical
ordinal
Numeric
float
Python obj class
str
float


Metodología
Se realiza un análisis de los datos para ver si es necesario realizar limpieza, los csv utilizados no contienen campos vacíos en las columnas utilizadas.

Se comprueba que las columnas estén en snake_case y se elimina posibles duplicados utilizando drop duplicates con el subset id que es único a cada tweet.

Se transforma los strings de fecha a datetime para poder utilizar con facilidad estos datos más adelante.

Para responder sus tweets más populares se ordena la df en función de número de likes, número de respuestas y número de Retweets y para cada una de estas se generan 2 gráfico mostrando las 5 mayores filas una en función de tweets y la otra con fecha.

Para visualizar a qué horas twittea Elon se creó una serie en una variable, conteniendo la hora y la cantidad de tweets en la misma.
Se graficó siguiendo el orden de las horas para una comprensión más fácil.

Para vincular los tweets de Elon con los cambios en DogeCoin se graficó los cambios en la moneda y se marcó la fecha de los 5 tweets más comentados de este, ya que se comprobó que sus tweets mas comentados se trataban sobre Criptomonedas.







Resultados


 Más comentados




La mayoría de sus tweets con más respuesta se tratan de Criptocurrency y ocurrieron en mayo 2021
.
Más gustados




Sus tweets con más me-gusta, se tratan de sus opiniones, memes, comentarios positivos o momentos claves de SpaceX-Tesla. También corresponden a años diferentes. 

Más compartidos





Sus tweets más compartidos tienen más que ver con sus opiniones, aunque también se encuentran algunos graciosos, siendo su más compartido una broma:







Horas de tweeteo



Se comprobó que Elon tweetea en casi cualquier momento, probablemente en el momento en el que se le ocurre la publicación la hace.

Existen CEOs que restringen el uso de redes sociales por parte del día, pero este no es el caso.
 La hora con más publicaciones concuerda con la hora a al que regresa a su hogar tras el trabajo.

Esto nos dice que la mayoría de las noches se duerme a la 1 de la madrugada y no tiene el régimen de sueño más ejemplar.












Cripto



Las fechas de sus publicaciones más comentadas coinciden con el gran crecimiento de la moneda en 2021.
Por lo que se puede determinar que tuvo un impacto en la moneda, pero para establecer bien la relación y ver si Doge se hizo popular porque Musk lo twiteo o si Elon lo twiteo porque la moneda se hizo popular se necesita un análisis más profundo.

Comentarios


Se realizaron descubrimientos interesantes como las diferencias entre los tweets más comentados y más gustados/compartidos, los mismos pueden inspirar una exploración para comprobar si sucede lo mismo con otras figuras.

Lo averiguado ante el estudio de las horas de publicación de Elon Musk también puede impulsar la búsqueda de mayor información sobre su vida y su día a día: https://finty.com/us/daily-routines/elon-musk/

O para intentar comprobar si otros CEOs/celebridades son como él.

Link a un análisis interesante de los tweets de Elon Musk y sus temas: https://www.visualcapitalist.com/a-decade-of-elon-musks-tweets-visualized/

Link análisis de DogeCoin con phyton: https://blog.jovian.ai/exploratory-data-analysis-on-dogecoin-using-python-1ddc1ab550c3



