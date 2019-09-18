Загрузить датасет по url:

url="http://yustiks.ru/dataset/world-happiness-report-2019.csv"
df=pd.read_csv(url)
World happiness gauged by technologies, social norms, and government policies. Dataset created by PromptCloud's web crawling solution.

Country (region) Name of the country.
Ladder Cantril Ladder is a measure of life satisfaction.
SD of Ladder Standard deviation of the ladder.
Positive affect Measure of positive emotion.
Negative affect Measure of negative emotion.
Social support The extent to which Social support contributed to the calculation of the Happiness Score.
Freedom The extent to which Freedom contributed to the calculation of the Happiness Score.
Corruption The extent to which Perception of Corruption contributes to Happiness Score.
Generosity The extent to which Generosity contributed to the calculation of the Happiness Score.
Log of GDP per capita The extent to which GDP contributes to the calculation of the Happiness Score.
Healthy life expectancy The extent to which Life expectancy contributed to the calculation of the Happiness Score.
Посмотреть первые несколько рядов таблицы

​
Построить частотный график для двух параметров: Freedom и positive affect. Какое это распределение?

​
Найти медиану, моду, математическое ожидание, стандартное отклонение, дисперсию, минимум и максимум, найти выбросы (если есть), размах для колонки Freedom

​
Посмотреть корреляцию между Freedom и positive affect (графически и математически). Графически - plt.scatter, математически - посчитать коэффициент Пирсона. О чем говорит знак коэффициента?

​
Нормализовать данные колонки Freedom (централизация + масштабирование)

​
Построить матрицу корреляций для всех колонок таблицы

​
Загрузить следующую таблицу:

import io
import requests
url="http://yustiks.ru/avocado.csv"
df=pd.read_csv(url)
df[:3]
Unnamed: 0	Date	AveragePrice	Total Volume	4046	4225	4770	Total Bags	Small Bags	Large Bags	XLarge Bags	type	year	region
0	0	2015-12-27	1.33	64236.62	1036.74	54454.85	48.16	8696.87	8603.62	93.25	0.0	conventional	2015	Albany
1	1	2015-12-20	1.35	54876.98	674.28	44638.81	58.33	9505.56	9408.07	97.49	0.0	conventional	2015	Albany
2	2	2015-12-13	0.93	118220.22	794.70	109149.67	130.50	8145.35	8042.21	103.14	0.0	conventional	2015	Albany
Сделать частотный график колонки AveragePrice. Какое это распределение?

​
Найти корреляцию в следующих колонках:

Корелляция между: 4046 - Total number of avocados with PLU 4046 sold и например Average Price. Если корелляция есть, то скорее всего, данный вид авокадо дорогой по цене и он влияет на среднюю стоимость.