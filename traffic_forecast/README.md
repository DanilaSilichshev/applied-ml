## **Highway Traffic Forecasting**  
## **Прогнозирование трафика на автомагистрали**  

This project focuses on forecasting highway traffic volume using time series analysis, identifying seasonal patterns, and optimizing predictions.  
Этот проект посвящён прогнозированию объёма трафика на автомагистрали с использованием временного ряда, выявлению сезонных закономерностей и оптимизации предсказаний.  

---

## **Goal / Цель**  
- Analyze the time series structure to detect seasonality and trends.  
  Проанализировать структуру временного ряда для выявления сезонности и трендов.  
- Compare different forecasting methods and identify the best-performing approach.  
  Сравнить различные методы прогнозирования и определить наиболее эффективный.  
- Forecast future traffic trends based on the best model.  
  Экстраполировать модель для предсказания будущего трафика. 

---

## **Technologies / Технологии**  
- Python  
- Scikit-learn  
- Pandas / NumPy  
- Matplotlib / Seaborn  
- Statsmodels (ACF/PACF analysis)  
- RandomForestRegressor  
- XGBoost  
- Theta Model  

---

## **Files / Структура файлов**  
- `main.ipynb`:  
  - Data preprocessing, time series analysis, model training, and evaluation.  
    Предобработка данных, анализ временного ряда, обучение модели и её оценка.  
  - Visualization of time series data and ACF/PACF plots for seasonality detection.  
    Визуализация временного ряда и построение ACF/PACF для выявления сезонности.  
  - Comparison of multiple models, selection of the best-performing one.  
    Сравнение нескольких моделей и выбор наилучшей.  
  - Traffic forecasting based on the best model.  
    Прогнозирование трафика с использованием лучшей модели.  
- `Metro_Interstate_Traffic_Volume.csv`:  
  - **Dataset** containing traffic volume data for a major interstate highway.  
    **Датасет**, содержащий данные о трафике на крупной автомагистрали.  
  - Used for training and testing models.  
    Используется для обучения и тестирования моделей.  

---

## **Results / Результаты**  
- **Best Model: Theta (504 hours)** – achieved the lowest **MAPE (8.35)**, making it the most accurate forecasting model.  
  **Лучшая модель: Theta (504 часов)** – показала наименьшую ошибку **MAPE (8.35)**, став наиболее точной моделью прогнозирования.  
- **Time series visualization and ACF/PACF analysis revealed seasonality**, which improved model selection and performance.  
  **Визуализация временного ряда и анализ ACF/PACF выявили сезонность**, что помогло улучшить выбор модели и её качество.