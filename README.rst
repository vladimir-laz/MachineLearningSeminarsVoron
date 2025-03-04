#########################
Machine Learning Seminars
#########################

Информация
==========
- Занятия начнутся с 10го февраля по расписанию.

Полезные ссылки
===============
- Плейлист лекций и семинаров: `2020-2021 <https://www.youtube.com/playlist?list=PLk4h7dmY2eYHHTyfLyrl7HmP-H3mMAW08>`_; `2021-2022 <https://youtube.com/playlist?list=PLk4h7dmY2eYFmowaPqjFDzSokiiLq5TkT>`_
- `Курс лекций К.В. Воронцова. <http://www.machinelearning.ru/wiki/index.php?title=Машинное_обучение_%28курс_лекций%2C_К.В.Воронцов%29>`_
- `Курс Мурата Апишева по python. <https://github.com/MelLain/mipt-python>`_
- `Почта для связи. <grabovoy.av@phystech.edu>`_

Осений семестр
==============

Курсовое домашнее задание:
--------------------------

Первое задание:
************************************************
- Начало: 15:30 26.09.2022
- Дедлайн: 23:59 16.10.2022.
- Писать на почту Андрею. Тема письма [MIPT-2022-ML-fall-1] ФИО. В письме прислать .ipynb файл.
- `Генератор задания <https://github.com/andriygav/MachineLearningSeminars/blob/master/hometask/task1-1/generator.ipynb>`_:
    - В качестве почты нужно ввести почту в домене @phystech.edu.
    - После ввода почты, вам будет предложена выборка с ссылкой для скачивания, а также методы, которые нужно проанализировать для данной выборки.
- Требуется:
    - Провести анализ выборки:
        - Определить тип признаков.
        - Выполнить визуальный анализ данных.
    - Выполнить препроцесинг данных:
        - Преобразовать категориальные признаки в вещественные.
        - Отнормировать признаки.
    - Провести эксперимент для предложеных методов:
        - Выполнить подбор гиперпараметров.
        - Подобрать регуляризаторы.
        - Получить итоговые модели.
    - Описать полученые результаты:
        - Какая модель лучше и почему.
        - С какими проблемами столкнулись во время выполнения, возможно недочеты стандартных библиотек.
        - Совпадают ли полученные результаты с ожидаемыми результатами.
- Оценивание:
    - Качество кода (1б):
        - Код должен работать у проверяющего.
        - Код должен был понятен без автора.
    - Качество анализа (3б):
        - Анализ выборки.
        - Анализ гиперпараметров.
        - Анализ результатов для разных моделей.
    - Качество отчета (1б):
        - Учитывается полнота отчета.

Второе задание:
************************************************
- Начало: 02.12.2022.
- Дедлайн: 23:59 15.12.2022.
- `Ссылка на задание <https://www.kaggle.com/t/8d5817c2d9eb416d827e6ab46d09a750>`_.
- Писать на почту Андрею. Тема письма [MIPT-2022-ML-fall-2] ФИО. В письме прислать .ipynb файл и ник на kaggle.
- Требуется:
    - Отправить свое решение в csv формате на kaggle.com.
    - Отправить ноутбук с решением на почту.

План занятий
------------

Вводный семинар
************************************************
- `Семинар <https://github.com/andriygav/MachineLearningSeminars/blob/master/sem1/main.ipynb>`_:
    - Теореотическая часть:
        - Общие идеи оптимизации, функции ошибки и тд.
    - Практическая часть:
        - При помощи sklearn показать пример Ирисов Фишера.
        - Понятие модели алгоритмов, алгоритм обучения, процесс оптимизации для конкретной задачи.
        - Переход от бинарной к многоклассовой.
        - Переобучение. Борьба с переобучениям (начало).
        - Немного о типах задач машинного обучения: прикладные и исследовательские
- Домашнее задание:
    - В задаче по переходу от бинарной классификации к многоклассовой добавить константу и скорректировать соответстветсвующие разделяющие гиперплоскости.
    - Подсказка: в LogisticRegresion нужно добавить специальный параметр fit_intercept=False, чтобы внутри черного ящика своя константта не добавлялась(влият на результат).


Линейные методы классификации и регрессии: метод стохастического градиента
*******************************************************************************
- `Семинар <https://github.com/andriygav/MachineLearningSeminars/blob/master/sem2/main.ipynb>`_:
    - Теореотическая часть:
        - Анализ стохастического градиента на сходимость.
        - Задача линейной регрессии, МНК в общем случае.
        - Постановка задачи линейной регрессии через правдоподобие, вероятностные предположения о данных + регуляризаций.
    - Практическая часть:
        - Разбор домашнего задания.
        - Метод стохастического градиента на практике.
        - Использования torch framework для нахождения градиента сложной функции.
        - Вероятностная постановка задачи машинного обучения. Регуляризация l1, l2.
        - Анализ решения задачи оптимизации от параметра регуляризации.
        - Выбор параметра регуляризации при помощи LOO.
- Домашнее задание:
    - Используя вероятностную постановку задачи для линейной регрессии с априорным предположением p(w) = N(0, I) получить аналитическое решение на оптимальный вектор параметров w.
    - Использовать метод Cross-Validation вместо метода LOO для выбора оптимального параметра регуляризации gamma.

Нейронные сети: Autograd
*******************************************************************************
- `Семинар <https://github.com/andriygav/MachineLearningSeminars/blob/master/sem3/main.ipynb>`_:
    - Теореотическая часть:
        - Автоматическое диференцирование.
    - Практическая часть:
        - Разбор домашнего задания.
        - Построение простой нейросетевой модели: многослойный персептрон.
        - Обучение персептрона на выборке MNIST.
        - Подбор гиперпараметров модели.
        - Пррореживание сетей (без кода, только графики).
- Домашнее задание:
    - Проделать то, что было на семинаре для выборки FashionMnist: подбор гиперпараметров модели (выполнить более подробно чем на семинаре), также провести анализ полученных результатов.
    - Указать какие минусы вы увидели в подборе гиперпараметров на семинаре (их как минимум 3).

Метрические методы классификации и регрессии
*******************************************************************************
- `Семинар <https://github.com/andriygav/MachineLearningSeminars/blob/master/sem4/main.ipynb>`_:
    - Практическая часть:
        - Разбор домашнего задания.
        - Пример как можно отказаться от признаков в линейном классификаторе.
        - Метод ближайших соседей, анализ разного количества соседей.
        - Ядра в методе ближайших соседей.
        - Метод Парзеновского окна.
        - Метод потенциальных функций (реализация).
        - Отбор эталонных элементов, алгоритм STOLP.
        - Формула Надарая Ватсона.
- Домашнее задание:
    - Выбрать один из метрических классификаторов (классификации или регрессии) и выполнить поиск оптимальных гиперпараметра при помощи кросс валидации.

Линейные методы классификации и регрессии: метод опорных векторов
*******************************************************************************
- `Семинар <https://github.com/andriygav/MachineLearningSeminars/blob/master/sem5/main.ipynb>`_:
    - Практическая часть:
        - SVM для классификации.
        - Примеры использования ядер для SVM.
        - SVM для регрессии.
        - Генерация признаков на основе опорных элементов.
- Домашнее задание:
    - Провести эксперимент с полиномиальным ядром: сгенерировать синтетическую выборку, на которой полиномиальное ядро имеет лучшее качество аппроксимации чем rbf и линейное ядро.
    
Многомерная линейная регрессия. Метод главных компонент
*******************************************************************************
- `Семинар <https://github.com/andriygav/MachineLearningSeminars/blob/master/sem6/main.ipynb>`_:
    - Практическая часть:
        - Многомерная линейная регрессия.
        - Сингулярное разложение.
        - Регуляризация для многомерной регрессии: используя SVD.
        - Зависимость качества аппроксимации от числа обусловлености.
        - Метод главных компонент: визуализация MNIST.
        - Метод главных компонент: для изображений.
- Домашнее задание:
    - Доказать лемму из семинара.
    - Для синтетически сгенерированной выборки  (beta=2, mu=0.01) построить график зависимости качества аппроксимации контрольной вбыорки от коэффициента регуляризации. Сравнить скорость работы в случае использования SVD разложения и без него. 

Нелинейная регрессия. Обощенные линейные модели. Нестандартные функции потерь.
*******************************************************************************
- `Семинар <https://github.com/andriygav/MachineLearningSeminars/blob/master/sem7/main.ipynb>`_:
    - Практическая часть:
        - Нелинейная регрессия: пример задачи.
        - Сравнение градиентного спуска, метода Ньютона-Рафсона, метода Ньютона-Гауса.
        - Обобщенно линейные модели: оптимальный размер выборки.
        - Функция потерь для задачи поиска близких предложений.
        - Визуализация сходимости метода Ньютона Рафсона и стохастического градиента.
- `Домашнее задание <https://forms.gle/9oYB7KVaJUndL7L26>`_:
    - Использовать модель для векторизации предложений из семинара. На основе полученных векторов решить задачу сентимент анализа для выборки Twitter (задача бинарной классификации). В качестве модели рассмотреть логистическую регрессию. Рекомендуется использовать модель Perceptron с третьего семинара, а также функцию ошибки torch.nn.BCELoss. Ссылка на данные: https://drive.google.com/file/d/1k4JrnVcoePEENCYt5iy17dyV_h133j2X/view?usp=sharing (предложения для классификации это последний столбец, а целевая переменная это второй столбец).
    
Критерии выбора моделей и методы отбора признаков.
*******************************************************************************
- `Семинар <https://github.com/andriygav/MachineLearningSeminars/blob/master/sem8/main.ipynb>`_:
    - Практическая часть:
        - Оценка качества моделе: внешний и внутрений критерии.
        - Отбор признаков: полный перебор, алгоритм Add, алгоритм Add-Del.
        - Качество классификации: Precision, Recall.
        - Пример задачи information retrieval.
        - О составлении выборки для постановки задачи ML.
- Домашнее задание:
    - реализовать метода отбора признаков Add-Del.
    - предложения внешний критерий качества для задачи поиска ошибок в текстах.

Логические методы классификации.
*******************************************************************************
- `Семинар <https://github.com/andriygav/MachineLearningSeminars/blob/master/sem9/main.ipynb>`_:
    - Практическая часть:
        - Логический классификатор реализация.
        - Примеры задач для решения логичеким классификатором.
        - Критерии информативности.
        - Решающий список, простая реализация.
        - Решающее дерево.
        - Случайный лес.
- Домашнее задание:
    - в реализованый метод построение логистического классификатора добавить возможность оптимизации по критерию Джини.

Поиск ассоциативных правил.
*******************************************************************************
- `Семинар <https://github.com/andriygav/MachineLearningSeminars/blob/master/sem10/main.ipynb>`_:
    - Практическая часть:
        - Постановка задачи ассоциативных правил.
        - Синтетичекий пример.
        - Пример реальных данных из kaggle.
        - Алгоритм APriory.
        - Алгоритм FP-growth.
        - Обобщение для вещественных данных.
        - Обобщенные ассоциативные правила.
- Домашнее задание:
    - выполнить анализ ассоциативных правил, которые получены алгоримом FP-growth. Расмоттреть только те правила, которые содержат более 3 элементов
    
Композиции классификаторов.
*******************************************************************************
- `Семинар <https://github.com/andriygav/MachineLearningSeminars/blob/master/sem11/main.ipynb>`_:
    - Практическая часть:
        - DummyEnsemble.
        - AdaBoost.
        - Градиентный бустинг, XGBoost.
        - Пример реальных данных из kaggle.
        - RandomForest.
        - Mixture Of Expert.
- Домашнее задание:
    - Рассматривается две выборки: `выборка <https://archive.ics.uci.edu/ml/datasets/Shill+Bidding+Dataset>`_ и `выборка <https://archive.ics.uci.edu/ml/datasets/Speaker+Accent+Recognition>`_. Для обоих выборок построить AdaBoost, GradientBoosting, RandomForest, Bagging. Сравнить качество на обоих выборках. Отличается ли результат? Почему?

Композиции классификаторов (градиентный бустинг).
*******************************************************************************
- `Семинар <https://github.com/andriygav/MachineLearningSeminars/blob/master/sem12/main.ipynb>`_:
    - Практическая часть:
        - ComBoost.
        - Gradient Boosting.
        - XGBoost.
        - CatBoost.
- Домашнее задание:
    - Реализовать комитетный бустинг для задачи регрессии.
    
Байесовская теория классификации.
*******************************************************************************
- `Семинар <https://github.com/andriygav/MachineLearningSeminars/blob/master/sem13/main.ipynb>`_:
    - Практическая часть:
        - Принцип максимума правдоподобия: визуализация.
        - Востановление плотности по империческим данным.
        - LOO для ввыбора ширины окна.
        - Наивный байесовский классификатор.
- Домашнее задание:
    - Получить оценку параметров нормального распределения из принципа максимума правдоподобия.

Методы кластеризации и обучение на неразмеченных данных.
*******************************************************************************
- `Семинар <https://github.com/andriygav/MachineLearningSeminars/blob/master/sem14/main.ipynb>`_:
    - Практическая часть:
        - Задача кластеризации.
        - Примеры кластеров.
        - K-means.
        - DBSCAN.
        - Иерархическая кластеризация.
        - Частичное обучение.
        - Self-training, 1970.
        - Неразмеченные данные в глубоком обучении.
- Домашнее задание:
    - Самому сравнить разные методы кластеризации для трех концентрических окружностей.

Весений семестр
===============

Курсовое домашнее задание:
--------------------------

Первое задание:
************************************************
- Дедлайн: 23:59 02.04.2023. Жесткий дедлайн 09.04.2022, каждый день оценка по каждой задаче уменьшается на 0.05. Суммарное количество баллов за каждую задачу 1.
- Задание доступно по `ссылке <https://github.com/andriygav/MachineLearningSeminars/blob/master/hometask/task2-1/>`_.
- Писать на почту Андрею. Тема письма [MIPT-2022-ML-spring-1] ФИО. В письме прислать .ipynb файлы (или ссылку на диск --- проверьте что есть доступ на чтение!!!).

Второе задание:
************************************************
- Дедлайн: 23:59 07.05.2023. Жесткий дедлайн 14.05.2023, каждый день оценка по каждой задаче уменьшается на 0.05.
- Задание доступно по `ссылке <https://github.com/andriygav/MachineLearningSeminars/blob/master/hometask/task2-2/>`_.
- Писать на почту Андрею. Тема письма [MIPT-2022-ML-spring-2] ФИО. В письме прислать .ipynb файлы  (или ссылку на диск --- проверьте что есть доступ на чтение!!!).

План занятий
------------

Глубокие Нейронные Сети. Сверточные нейросети и Рекурентные сети.
*******************************************************************************
- `Семинар <https://github.com/andriygav/MachineLearningSeminars/blob/master/sem15/main.ipynb>`_:
    - Практическая часть:
        - Сверточные нейронные сети.
        - Отслеживание обучения при помощи tensorboard.
        - Рекурентные нейронные сети.
        - Использование предобученных моделей.
        - Интерпретируемость ответов нейросети.
        
Нейронные сети. Автокодировщик. Transfer Learning. Генеративно-Состязательные сети.
*******************************************************************************
- `Семинар <https://github.com/andriygav/MachineLearningSeminars/blob/master/sem16/main.ipynb>`_:
    - Практическая часть:
        - Автокодировщик.
        - Линейный автокодировщик.
        - Автокодировщик на основе CNN.
        - Вариационный автокодировщик.
        - Перенос обучения с предварительно обученой модели.
        - Генеративно состязательные сети.
        
Векторное представления текстов.
*******************************************************************************
- `Семинар <https://github.com/andriygav/MachineLearningSeminars/blob/master/sem17/main.ipynb>`_:
    - Практическая часть:
        - Пример классификации твитов.
        - Зачем нужна векторизация?.
        - Токенизация текстов.
        - Word2Vec (на основе модели FastText).
        - FastText модель (сжатая до emb-dim=10 для легковестности).
        - Задачи для unsupervise training моделей векторизации.
        
Attention is all you need. Трансформеры.
*******************************************************************************
- `Семинар <https://github.com/andriygav/MachineLearningSeminars/blob/master/sem18/main.ipynb>`_:
    - Практическая часть:
        - Модель внимания в рекурентных нейронных сетях.
        - Трансформеры.
        - T2T переводчик.
        - BPE токенизация.
        - BERT.
        - LaBSE.
        
Тематическое моделирование.
*******************************************************************************
- `Семинар <https://github.com/andriygav/MachineLearningSeminars/blob/master/sem19/main.ipynb>`_:
    - Практическая часть:
        - Модель LDA.
        - Модель PLSA (bigartm).

Пояснение к домашнему заданию.
*******************************************************************************
- `Семинар <https://github.com/andriygav/MachineLearningSeminars/blob/master/sem20/main.ipynb>`_:
    - Практическая часть:
        - Задачи из ДЗ.

Задача ранжирования.
*******************************************************************************
- `Семинар <https://github.com/andriygav/MachineLearningSeminars/blob/master/sem21/main.ipynb>`_:
    - Практическая часть:
        - Базовые понятие.
        - Пример задачи ранжирования.
        - Пример рекомендательной системы.
        - Обучение поисковика на базе pyserini.
        
Рекомендательные системы.
*******************************************************************************
- `Семинар <https://github.com/andriygav/MachineLearningSeminars/blob/master/sem22/main.ipynb>`_:
    - Практическая часть:
        - Константная модель.
        - Кореляционная система.
        - SLIM.
        - SVD.

Временные ряды.
*******************************************************************************
- `Семинар <https://github.com/andriygav/MachineLearningSeminars/blob/master/sem23/main.ipynb>`_:
    - Практическая часть:
        - Авторегрессионая модель.
        - Экспоненциальное сглаживание.
        - Кластерный анализ временных рядов.
        
Онлайновое обучение.
*******************************************************************************
- `Семинар <https://github.com/andriygav/MachineLearningSeminars/blob/master/sem24/main.ipynb>`_:
    - Практическая часть:
    
Обучение с подкреплением.
*******************************************************************************
- `Семинар <https://github.com/andriygav/MachineLearningSeminars/blob/master/sem25/main.ipynb>`_:
    - Практическая часть:
        - Стационарный многорукий бандин.
        - Нестационарный многорукий бандин.
        - Задача о заплыве.
        
Активное обучение.
*******************************************************************************
- `Семинар <https://github.com/andriygav/MachineLearningSeminars/blob/master/sem26/main.ipynb>`_:
    - Практическая часть:
        - Активное обучение со случайным добавлчющим элементом.
        - Активное обучение с добавлением элемента с максимальной дисперсией.
        
Заключительное занятие.
*******************************************************************************
- `Семинар <https://github.com/andriygav/MachineLearningSeminars/blob/master/sem27/main.ipynb>`_:
    - Теоретическая часть:
        - Разбор Posterior Sampling
