# Обзор готового курса: Аналитика и ML в E-commerce

Мы успешно разработали полный набор учебных материалов (сквозной проект), который покрывает все 30 тем из `data_analysis_plan.md` и `ml_plan.md`. 

Все файлы сохранены в директории `ecommerce_project/`.

---

## 📂 Структура проекта

### 1. Данные (`data/`)
Сгенерирован синтетический датасет реалистичного магазина:
- **`customers.csv`** (клиенты)
- **`products.csv`** (товары)
- **`transactions.csv`** (покупки)
- **`ecommerce.db`** (локальная SQLite база данных для отработки SQL-запросов)

### 2. Часть 1: Data Analysis (Темы 1-15)
- **Введение и Excel/Sheets:** [da_topic_01_02_intro.md](/ecommerce_project/da_topic_01_02_intro.md), [da_topic_03_04_sheets.md](/ecommerce_project/da_topic_03_04_sheets.md)
- **Python и Pandas:** [da_topic_05_python_intro.ipynb](/ecommerce_project/da_topic_05_python_intro.ipynb), [da_topic_06_07_pandas.ipynb](/ecommerce_project/da_topic_06_07_pandas.ipynb)
- **Очистка данных:** [da_topic_08_data_cleaning.ipynb](/ecommerce_project/da_topic_08_data_cleaning.ipynb)
- **Визуализация (Matplotlib/Seaborn):** [da_topic_09_10_viz.ipynb](/ecommerce_project/da_topic_09_10_viz.ipynb)
- **SQL (sqlite3):** [da_topic_11_12_13_sql.ipynb](/ecommerce_project/da_topic_11_12_13_sql.ipynb)
- **Статистика:** [da_topic_14_statistics.ipynb](/ecommerce_project/da_topic_14_statistics.ipynb)
- **Финальный отчет:** [da_topic_15_da_report.md](/ecommerce_project/da_topic_15_da_report.md)

### 3. Часть 2: Machine Learning (Темы 1-15)
- **Предобработка:** [ml_topic_03_preprocessing.ipynb](/ecommerce_project/ml_topic_03_preprocessing.ipynb)
- **Регрессия (Linear, Multiple, Polynomial):** [ml_topic_04_05_simple_regression.ipynb](/ecommerce_project/ml_topic_04_05_simple_regression.ipynb), [ml_topic_06_08_multiple_poly_regression.ipynb](/ecommerce_project/ml_topic_06_08_multiple_poly_regression.ipynb)
- **Классификация (Отток клиентов):** [ml_topic_09_11_classification.ipynb](/ecommerce_project/ml_topic_09_11_classification.ipynb)
- **Кластеризация (Сегментация K-Means):** [ml_topic_12_14_clustering.ipynb](/ecommerce_project/ml_topic_12_14_clustering.ipynb)
- **Анализ корзины (Association Mining):** [ml_topic_15_association.ipynb](/ecommerce_project/ml_topic_15_association.ipynb)

---

## 👨‍🏫 Как с этим работать?
Для всех практических `.ipynb` файлов сгенерированы **версии с ответами** (они заканчиваются на `_solutions.ipynb`).
- Студентам вы выдаете базовые файлы, где в коде есть комментарии `# Ваш код здесь`.
- Для проверки или демонстрации вы используете файлы `_solutions`, где уже написан работающий код (Pandas-трансформации, обучение моделей scikit-learn и вывод графиков).

