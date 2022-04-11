# Análisis de los Tweets de Elon Musk

## Introducción y Resumen:

Elon Musk es una de las figuras más interesantes de los últimos tiempos es el CEO y jefe ingeniero de SpaceX, padre de familia, CEO de Tesla, billonario, director y usuario habitual de Twitter entre otros.

Twitter es el medio elegido por Elon para expresarse, realizar anuncios sobre sus compañías y compartir sus ideas, opiniones y memes.

Más de 77 millones de seguidores están atentos a sus publicaciones que ya superan las 15000 entradas y muchas de ellas han tenido un gran impacto en el mundo, sobre todo en campos políticos y económicos.

Por medio de sus Tweets se puede tener un vistazo de ideas, su mundo y vida, por lo que analizar sus tweets puede ser de lo más interesante.

En este estudio se realizan las siguientes preguntas: ¿Cuáles son los tweets más populares de Elon? ¿De qué tratan?,¿A qué horas twittea? ¿Qué nos dice de su estilo de vida el momento en que twittea Elon?
También intentar visualizar brevemente la existencia de una relación en el crecimiento de Cripto con sus posts en Twitter. 


## Data
Los archivos utilizados para armar el dataframe con la información de los Tweets históricos fueron proporcionados por la profesora del curso, a excepción del csv 2015-2020 que fue extraído del sitio Kaggle.

El dataframe tweet_df está formado por las siguientes columnas:

| Column        | Data group          | Python obj class |
|---------------|---------------------|------------------|
| index         | Numeric Integer     | int              |
| date          | categorical ordinal | str              |
| time          | categorical ordinal | str              |
| tweet         | categorical nominal | str              |
| replies_count | numeric integer     | int              |
| retweet_count | numeric integer     | int              |
| likes_count   | numeric integer     | int              |
| id            | numeric integer     | int              |

![image](https://user-images.githubusercontent.com/74270973/162850503-f2824270-80df-4c4c-b86d-6b3e5abc6515.png)

Para el dataframe de DogeCoin se utilizó un archivo .csv extraído de Kraggle con valores históricos de la criptomoneda.
 El dataframe contine las siguientes columnas:
| Column        | Data group          | Python obj class |
|---------------|---------------------|------------------|
| open          | Numeric Integer     | int              |
| date          | categorical ordinal | str              |



## Metodología

Se realiza un análisis de los datos para ver si es necesario realizar limpieza, los csv utilizados no contienen campos vacíos en las columnas utilizadas.

Se comprueba que las columnas estén en snake_case y se elimina posibles duplicados utilizando drop duplicates con el subset id que es único a cada tweet.

Se transforma los strings de fecha a datetime para poder utilizar con facilidad estos datos más adelante.

Para responder sus tweets más populares se ordena la df en función de número de likes, número de respuestas y número de Retweets y para cada una de estas se generan 2 gráfico mostrando las 5 mayores filas una en función de tweets y la otra con fecha.

Para visualizar a qué horas twittea Elon se creó una serie en una variable, conteniendo la hora y la cantidad de tweets en la misma.
Se graficó siguiendo el orden de las horas para una comprensión más fácil.

Para vincular los tweets de Elon con los cambios en DogeCoin se graficó los cambios en la moneda y se marcó la fecha de los 5 tweets más comentados de este, ya que se comprobó que sus tweets mas comentados se trataban sobre Criptomonedas.



## Resultados
* Más comentados

La mayoría de sus tweets con más respuesta se tratan de Criptocurrency y ocurrieron en mayo 2021


![image](https://user-images.githubusercontent.com/74270973/162850945-2ec8f961-410e-4bf6-962e-ccfffe19f571.png)

![image](https://user-images.githubusercontent.com/74270973/162850952-aa1bb9ea-57fc-4a0f-88c5-ac6b01dc3379.png)


* Más gustados

Sus tweets con más me-gusta, se tratan de sus opiniones, memes, comentarios positivos o momentos claves de SpaceX-Tesla. También corresponden a años diferentes. 
![image](https://user-images.githubusercontent.com/74270973/162851045-d2b00e4a-b5ac-46bf-b96c-19b7db9cf5d0.png)
![image](https://user-images.githubusercontent.com/74270973/162851051-b0fb84b5-3bca-4a2a-b80c-7b033a80a943.png)


* Más compartidos

![image](https://user-images.githubusercontent.com/74270973/162851265-814e3e5e-137f-4ee7-bdab-435bd5aa443e.png)

![image](https://user-images.githubusercontent.com/74270973/162851275-86b13d4f-0f1f-47de-b298-15dc301177b4.png)

Sus tweets más compartidos tienen más que ver con sus opiniones, aunque también se encuentran algunos graciosos, siendo su más compartido una broma:

![image](https://user-images.githubusercontent.com/74270973/162851436-2b556d46-f957-458f-87b7-91622229b497.png)



## Horas de tweeteo

![image](https://user-images.githubusercontent.com/74270973/162851469-d3803878-b9b2-40ef-abff-437974820ae9.png)

Se comprobó que Elon tweetea en casi cualquier momento, probablemente en el momento en el que se le ocurre la publicación la hace.

Existen CEOs que restringen el uso de redes sociales por parte del día, pero este no es el caso.
 La hora con más publicaciones concuerda con la hora a al que regresa a su hogar tras el trabajo.

Esto nos dice que la mayoría de las noches se duerme a la 1 de la madrugada y no tiene el régimen de sueño más ejemplar.


## Cripto

![image](https://user-images.githubusercontent.com/74270973/162851560-dfd2fd43-750f-4b73-9bc6-b3ab2afea5e3.png)

Las fechas de sus publicaciones más comentadas coinciden con el gran crecimiento de la moneda en 2021.
Por lo que se puede determinar que tuvo un impacto en la moneda, pero para establecer bien la relación y ver si Doge se hizo popular porque Musk lo twiteo o si Elon lo twiteo porque la moneda se hizo popular se necesita un análisis más profundo.


## Comentarios

Se realizaron descubrimientos interesantes como las diferencias entre los tweets más comentados y más gustados/compartidos, los mismos pueden inspirar una exploración para comprobar si sucede lo mismo con otras figuras.

Lo averiguado ante el estudio de las horas de publicación de Elon Musk también puede impulsar la búsqueda de mayor información sobre su vida y para intentar comprobar si otros CEOs/celebridades son como él.

Link a artículo sobre un día de Elon: https://finty.com/us/daily-routines/elon-musk/

Link a un buen análisis sobre los tweets de Elon Musk y sus temas: https://www.visualcapitalist.com/a-decade-of-elon-musks-tweets-visualized/

Link a análisis histórico de DogeCoin con phyton: https://blog.jovian.ai/exploratory-data-analysis-on-dogecoin-using-python-1ddc1ab550c3 







