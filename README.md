# Classic ML — Credit Scoring

Предсказание дефолта заемщиков на данных Kaggle "Give Me Some Credit". Полный цикл: EDA, Feature Engineering, WOE, моделирование, бизнес-метрики.

## Результаты

| Метрика | Значение |
|---|---|
| Модель | CatBoost |
| ROC-AUC | **0.8665** |
| Прибыль | 178 млн ₽ |
| Одобрение | 79.4% |
| Bad Rate | 2.26% |

## Что внутри

- Разведочный анализ (выбросы, пропуски, групповой анализ)
- Feature Engineering (6 новых признаков)
- WOE-биннинг и Information Value
- 5 моделей: LR, RF, LightGBM, XGBoost, CatBoost
- Тюнинг гиперпараметров
- Кросс-валидация, бутстреп, PSI
- Оценка бизнес-метрик (прибыль, порог)

## Данные

[Give Me Some Credit — Kaggle](https://www.kaggle.com/competitions/GiveMeSomeCredit)

## Как запустить

```bash
git clone https://github.com/Mikhail-Raver/Classic-ML-credit-scoring-.git
cd Classic-ML-credit-scoring-
pip install -r requirements.txt
```

Скачайте `cs-training.csv` с Kaggle (ссылка выше) и поместите в корень проекта.
В первой ячейке ноутбука замените путь `/kaggle/input/first-project/cs-training.csv` на `cs-training.csv`.
Затем запустите:

```bash
jupyter notebook Project.ipynb
```

## Стек

Python, Pandas, NumPy, Matplotlib, Scikit-learn, CatBoost, XGBoost, LightGBM

## Автор

[Mikhail-Raver](https://github.com/Mikhail-Raver)
