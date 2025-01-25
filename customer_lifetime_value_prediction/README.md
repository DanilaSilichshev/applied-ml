# Customer Lifetime Value Prediction with Gradient Boosting  
# Прогнозирование значения жизненного цикла клиента с помощью градиентного бустинга  

This project focuses on predicting Customer Lifetime Value using gradient boosting algorithms.  
Этот проект посвящён прогнозированию значения пожизненной ценности клиента с использованием алгоритмов градиентного бустинга.

---

## Goal / Цель  
- Compare different implementations of gradient boosting algorithms.  
  Сравнить различные реализации алгоритма градиентного бустинга.  
- Select the best model based on quality metrics after hyperparameter tuning.  
  Выбрать лучшую модель на основе метрик качества после подбора гиперпараметров.  

---

## Technologies / Технологии  
- Python  
- LightGBM  
- CatBoost  
- XGBoost  
- Pandas  
- Jupyter Notebooks  

---

## Files / Структура файлов  
- `main.ipynb`:  
  - Contains data preprocessing, model training, and evaluation.  
    Содержит предобработку данных, обучение моделей и их оценку.  
  - Comparison of CatBoost, LightGBM, and XGBoost models.  
    Сравнение моделей CatBoost, LightGBM и XGBoost.  
  - Hyperparameter tuning and metrics comparison.  
    Подбор гиперпараметров и сравнение метрик.

---

## Results / Результаты  
- Best model: **LightGBM**.  
  Лучшая модель: **LightGBM**.  
- **Key metrics**:  
  - **Mean Absolute Error (MAE)**: LightGBM achieved the lowest MAE compared to other implementations.  
    **Средняя абсолютная ошибка (MAE)**: LightGBM показала наименьшее значение MAE среди других моделей.  
  - **R² (Coefficient of Determination)**: LightGBM also achieved the highest R², indicating the best model fit.  
    **R² (коэффициент детерминации)**: LightGBM также достигла наивысшего значения R², что указывает на лучшую аппроксимацию модели.  
- After hyperparameter tuning, LightGBM outperformed CatBoost and XGBoost on both metrics.  
  После подбора гиперпараметров LightGBM превзошла CatBoost и XGBoost по обеим метрикам.

---

## Summary / Резюме  
This project demonstrates the use of gradient boosting for customer lifetime value prediction, highlighting the importance of hyperparameter tuning in achieving the best results.  
Проект демонстрирует использование градиентного бустинга для прогнозирования значения пожизненной ценности клиента и подчёркивает важность подбора гиперпараметров для достижения лучших результатов.
