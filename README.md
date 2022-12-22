# Wine Quality
## Dataset
Ссылка: https://www.kaggle.com/datasets/yasserh/wine-quality-dataset

Набор данных описывает количество различных химических веществ, присутствующих в вине и их влияние на его качество.

Датасет одержит следующие столбцы:
- 1 - fixed acidity
- 2 - volatile acidity
- 3 - citric acid
- 4 - residual sugar
- 5 - chlorides
- 6 - free sulfur dioxide
- 7 - total sulfur dioxide
- 8 - density
- 9 - pH
- 10- sulphates
- 11 - alcohol
- 12 - quality

## Google Collab
https://colab.research.google.com/drive/1QNENs2ELo_nCaiB8jEHI5s1YjS8oFQRT?usp=sharing
## Видео с защитой проекта
## План
- EDA
- Попробовать модели 
    - SGDClassifier
    - DecisionTree
    - RandomForest
    - XGBClassifier
- Датасет несбалансированный, применить методы Oversampling
- Улучшить обучение кросс-валидацией
- Посмотреть важность признаков
- Подвести итоги и сравнить результаты
## Результаты
**SGDClassifier:**

![Image alt](https://github.com/yanarfkv/DataAnalysisProject/raw/master/images/SGDClassifier.png)

Качество получилось довольно низкое. Accuracy и F1-score выглядят плохими.


**DecisionTreeClassifier:**

![Image alt](https://github.com/yanarfkv/DataAnalysisProject/raw/master/images/DecisionTreeClassifier.png)

**RandomForestClassifier:**

![Image alt](https://github.com/yanarfkv/DataAnalysisProject/raw/master/images/RandomForestClassifier.png)

Качество чуть выше, однако всё равно низкое.
**XGBClassifier:**

![Image alt](https://github.com/yanarfkv/DataAnalysisProject/raw/master/images/XGBClassifier.png)

Получилось лучшее качество среди всех моделей. Accuracy и F1-score самые высокие.

## Сравнение моделей:

После применения Oversampling редких классов получилось улучшить прежнее качество.

XGBoost accuracy 0.64 (до) vs RandomForestClassifier accuracy 0.65 (после)