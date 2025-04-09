# **Amazon Magazine Recommendation System**  
# **Рекомендательная система по журналам Amazon**

This project focuses on building and evaluating a **recommender system** using the `Magazine_Subscriptions.csv` subset from the **Amazon datasets**.  
Этот проект посвящён созданию и оценке **рекомендательной системы** на подвыборке `Magazine_Subscriptions.csv` из **датасетов Amazon**.

---

## **Goal / Цель**
- Develop and compare recommendation models based on user-item interactions.  
  Разработать и сравнить модели рекомендаций на основе взаимодействий пользователей с журналами.

---

## **Technologies / Технологии**
- Python  
- NumPy  
- Pandas  
- Matplotlib  
- LightFM

---

## **Files / Файлы**
- `main.ipynb`  
  - Main Jupyter Notebook with analysis, models, and evaluation.  
    Основной Jupyter Notebook с анализом, моделями и оценкой.  
- `data/Magazine_Subscriptions.csv`  
  - Contains the **subset of Amazon reviews** related to magazine subscriptions.  
    Содержит **подвыборку отзывов Amazon**, относящихся к подпискам на журналы.

---

## **Models / Модели**
- **Baseline**: Top-N most popular magazines with high ratings  
  **Baseline**: Топ-N самых популярных журналов с высоким рейтингом  
- **LightFM (warp)**: Latent factor model with WARP loss  
  **LightFM (warp)**: модель скрытых факторов с функцией потерь WARP  
- **LightFM (bpr)**: Latent factor model with BPR loss  
  **LightFM (bpr)**: модель скрытых факторов с функцией потерь BPR

---

## **Results / Результаты**
- **LightFM (WARP)** showed the best performance with `HR@10 ≈ 0.34` and ~99% coverage.  
  **LightFM (WARP)** показала наилучший результат с `HR@10 ≈ 0.34` и покрытием около 99%.  
- **BPR** had slightly lower accuracy, but higher novelty.  
  **BPR** показала немного меньшую точность, но более высокую новизну.  
- **Baseline** underperformed across all metrics.  
  **Бейзлайн** уступил другим моделям по всем метрикам.

---

## **Summary / Резюме**
This project explores recommendation approaches on real-world sparse user-item data from Amazon.  
В проекте исследованы подходы к рекомендациям на разреженных пользовательских данных из Amazon.  
The best results were achieved by **LightFM (warp)**, offering a strong balance of accuracy and coverage.  
Наилучшие результаты показала модель **LightFM (warp)**, обеспечив хорошее сочетание точности и охвата.

**Further improvement:** hyperparameter tuning  
**Возможное улучшение:** настройка гиперпараметров модели