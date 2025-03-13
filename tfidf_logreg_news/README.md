# **News Classification Based on Their Textual Content**  
# **Классификация новостей по тегам на основе их текстового содержимого**  

This project focuses on **news classification** using web parsing, text processing, and machine learning techniques.  
Этот проект посвящён **классификации новостей**, включая парсинг, обработку текста и машинное обучение.  

---

## **Goal / Цель**  
- Train a machine learning model to classify news articles by tags based on their textual content.  
  Обучить модель машинного обучения для классификации новостей по тегам на основе их текстового содержимого.  
- Identify key words and phrases that contribute most to tag prediction.  
  Определить ключевые слова и фразы, наиболее значимые для предсказания тегов.  

---

## **Technologies / Технологии**  
- Python  
- Selenium  
- BeautifulSoup  
- Scapy  
- Scikit-learn  
- Pandas  
- NumPy  
- TF-IDF  
- Logistic Regression (OneVsRestClassifier)  

---

## **Files / Структура файлов**  
- `parser.py`  
  - Parses news articles from **[media.ssmu.ru](https://media.ssmu.ru/news/)**.  
    Выполняет парсинг новостей с **[media.ssmu.ru](https://media.ssmu.ru/news/)**.  

- `news_data.xlsx`  
  - Contains the **parsed dataset** of news articles.  
    Содержит **распарсенные данные** новостей. 

- `ml_model.py`  
  - Preprocesses text and applies **TF-IDF vectorization**.  
    Выполняет предобработку текста и применяет **TF-IDF**.  
  - Trains a **logistic regression model** (OneVsRestClassifier).  
    Обучает **логистическую регрессию** (OneVsRestClassifier).  
  - Extracts the **top 50 most important words for each tag**.  
    Выделяет **50 самых значимых слов для каждого тега**.  
  - Evaluates model performance using **F1-score, precision, recall, and Hamming Loss**.  
    Оценивает качество модели с помощью **F1-score, precision, recall и Hamming Loss**.  

---

## **Results / Результаты**  
- **TF-IDF with logistic regression successfully classified news articles** into multiple tags.  
  **TF-IDF и логистическая регрессия успешно классифицировали новости по тегам.**  
- **Hamming Loss remained low**, indicating a relatively small number of misclassified tags.  
  **Hamming Loss оказался низким**, что говорит о небольшом количестве ошибок.  
- **Precision and recall varied across different tags**, with some tags being more easily identifiable.  
  **Точность и полнота варьировались для разных тегов**, некоторые из них классифицировались лучше.  
- **The model extracted the most significant words for each tag**, helping in interpretability.  
  **Модель выделила ключевые слова для каждого тега**, что улучшает интерпретацию результатов.  

---

## **Summary / Резюме**  
This project integrates **web parsing, text analysis, and machine learning** to classify news articles. The model demonstrates **reliable performance** and extracts **meaningful keywords for each tag**. Future improvements may include **hyperparameter tuning, alternative classifiers, or expanding the dataset**.  
Этот проект объединяет **парсинг веб-страниц, анализ текста и машинное обучение** для классификации новостей. Модель **показывает стабильные результаты** и выделяет **значимые слова для тегов**. Возможные улучшения включают **оптимизацию гиперпараметров, использование других моделей или расширение данных**.