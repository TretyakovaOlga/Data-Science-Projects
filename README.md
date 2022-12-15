# Учебные проекты
_______

## ML: Оптимизация производственного процесса легирования стали
[Prom_optimization_final.ipynb](Prom_optimization_final.ipynb) </br>


**Задача:** построить модель, которая будет прогнозировать температуру конечного расплава в зависимости от заданных параметров производственного процесса. Оптимизация достигается путем снижения энергозатрат за счёт предварительного подбора оптимальных условий легирования.
</br>
</br>
Модель разрабатывается на базе исторических данных о процессах легирования сталей. Целевой признак изменяется в диапазоне от 1500 до 1704 градусов Цельсия. Используется метрика МАЕ, на финальной модели получен результат 5,68. В процессе работы проведен исследовательский анализ данных, заполнены пропуски, объединены данные из разных источников, добавлены признаки. Рассмотрены два набора признаков для обучения.  Рассмотрена линейная модель с регуляризацией, случайный лес, CatBoost и LGBM. Лучшая модель - Catboost, проведено тестирование.</br>
Библиотеки: sklearn, lightgbm, catboost</br>
</br>
</br>

## NLP: Определение токсичности комментариев
[Toxic_comments_predict.ipynb](Toxic_comments_predict.ipynb)


**Задача:** построить модель для отсева токсичных комментариев. Метрика f1 - не менее 0.75.</br>
</br>
Для создания словаря используется размеченный набор с комментариями. Лемматизация проводится с помощью nltk. Для получения признаков использованы мешок слов, TF-IDF, биграммы и word2vec.</br>
Использованные модели: логистическая регрессия, LGBM, LinearSVC, метод ближайших соседей. Лучший результат получен на CountVectorizer + bigrams + LogisticRegression.
На базе трёх лучших моделей составлен решающий ансамбль, проведено тестирование. Итоговое f1 - 0.77.</br>
Библиотеки: nltk, sklearn, gensim, lightgbm </br>
</br>
</br>

## ML: Определение рыночной стоимости автомобиля
[Predict_of_car_prices.ipynb](Predict_of_car_prices.ipynb) </br>
**Задача:** разработать модель, которая будет предсказывать рыночную автомобиля в зависимости от его характеристик (сервис по размещению объявлений о продаже авто).
</br></br>
Модель разрабатывается на базе исторических данных о продажах автомобилей. Проведено исследование данных и предобработка: заполнение пропусков и удаление некорректных данных. Метрика RMSE. Рассмотрены линейные модели, метод ближайших соседей, CatBoost и LGBM, точность работы, скорость обучения и предсказания. Проведено тестирование.</br>
Библиотеки: sklearn, lightgbm, catboost</br>
</br>
</br>
## EDA: Исследование рынка недвижимости в Санкт-Петербурге 2014-2019 гг
[EDA_Real_estate_final.ipynb](EDA_Real_estate_final.ipynb) </br>
**Задача:** необходимо проанализировать взаимосвязь цены квартиры и её параметров. </br></br>
Проведен исследовательский анализ объявлений о продаже квартир в Санкт-Петербурге и соседних населённых пунктах за несколько лет. Проведена предобработка и очистка данных. Изучено влияние на цену следующих параметров: общей и жилой площади, площади кухни, высоты потолков, количества комнат, этажа, близости парков, водоемов и аэропорта. Изучено изменение цены в различных населенных пунктах Ленинградской области, а также особенности ценообразования в центре Санкт-Петербурга и влияние на него параметров квартир.
</br>
Библиотеки: pandas, matplotlib.
</br>
</br>
## Стат анализ: Анализ тарифов для оператора связи
[Telecom_tariffs_analysis.ipynb](Telecom_tariffs_analysis.ipynb) </br>
**Задача:** необходимо проанализировать поведение пользователей и определить более прибыльный тариф </br></br>
Проведен анализ поведения пользователей при пользовании услугами связи. Проверены гипотезы о различии средней выручки тарифов, а также о различии выручки в Москве и других регионах.
</br>
Библиотеки: numpy, scipy, matplotlib, статистический тест, критерий Стьюдента
