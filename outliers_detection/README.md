# **Anomaly Detection in Component Representations of Data**  
# **Выявление аномалий в компонентных представлениях данных**  

This project focuses on detecting anomalies in component-based data representations using various anomaly detection algorithms.  
Этот проект посвящён выявлению аномалий в компонентных представлениях данных с использованием различных алгоритмов обнаружения аномалий.  

---

## **Goal / Цель**  
- Compare different anomaly detection methods.  
  Сравнить различные методы поиска аномалий.  
- Analyze the impact of low anomaly rates on detection performance.  
  Проанализировать влияние низкой доли аномалий на качество обнаружения.  

---

## **Technologies / Технологии**  
- Python  
- Scikit-learn  
- Pandas  
- Matplotlib / Seaborn  
- Jupyter Notebooks  

---

## **Files / Структура файлов**  
- `main.ipynb`:  
  - Contains data preprocessing, anomaly detection experiments, and evaluation.  
    Содержит предобработку данных, эксперименты по поиску аномалий и их оценку.  
  - Comparison of **IsolationForest**, **One-Class SVM**, and the **method of frequent deviations**.  
    Сравнение **IsolationForest**, **One-Class SVM** и **метода частых отклонений**.  
  - Analysis of anomaly detection performance based on different component representations.  
    Анализ эффективности выявления аномалий в зависимости от представления данных.  
- `data/` (excluded from GitHub):  
  - **Dataset:** The dataset used for anomaly detection is based on the [Credit Card Fraud Detection dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud#creditcard.csv).  
    **Данные:** Используется [набор данных о мошенничестве с кредитными картами](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud#creditcard.csv).  
  - Due to GitHub's file size limits, the dataset is not included in this repository. Download it from Kaggle and place it in the `data/` folder.  
    Из-за ограничений GitHub на размер файлов, этот набор данных не включён в репозиторий. Скачайте его с Kaggle и поместите в папку `data/`.


---

## **Results / Результаты**  
- **Anomalies in data are less than 1%**, making detection a challenging task.  
  **Доля аномалий в данных менее 1%**, что усложняет их обнаружение.  
- **Traditional methods (IsolationForest, One-Class SVM) showed limited effectiveness**, detecting only ≈35% of anomalies (recall), indicating weak separation of outliers in the component space.  
  **Классические методы (IsolationForest, One-Class SVM) показали ограниченную эффективность**, обнаружив лишь ≈35% аномалий (recall), что может указывать на слабое разделение выбросов в компонентном пространстве.  
- **The method of frequent deviations produced similar results**, confirming the difficulty of anomaly detection in this dataset.  
  **Метод частых отклонений показал аналогичные результаты**, что подтверждает сложность выявления аномалий в данных.  
- **Anomaly detection methods did not yield precise results due to the low anomaly ratio (<1%) and weak outlier separation in components.**  
  **Методы поиска аномалий не дали точного результата из-за низкой доли аномалий (<1%) и слабого разделения выбросов в компонентах.**  
- **Further improvements may involve deeper component analysis, neural networks, or gradient boosting for anomaly detection.**  
  **Для улучшения качества детекции стоит глубже анализировать компоненты, использовать нейронные сети или градиентный бустинг.**  

---

## **Summary / Резюме**  
This project explores anomaly detection in component-based data representations, highlighting the challenges posed by low anomaly rates and weak separation of outliers. Further research may involve advanced techniques to enhance detection accuracy.  
Проект исследует поиск аномалий в компонентных представлениях данных, подчёркивая сложности, вызванные низкой долей аномалий и слабым разделением выбросов. Дальнейшие исследования могут включать более продвинутые методы для повышения точности обнаружения.  
