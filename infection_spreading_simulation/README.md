# **Simulation of Infection Spread in Airports**  
# **Симуляция распространения инфекции в аэропортах**  

This project presents a model of infection spread through airports based on real flight data, using graph-based methods to identify key nodes and transmission pathways.  
В этом проекте представлена модель распространения инфекций через аэропорты на основе реальных данных о перелётах, используя метод графов для выявления ключевых узлов и путей распространения.  

---

## **Goal / Цель**  
- Simulate the spread of infections using real-world airport connections.  
  Смоделировать распространение инфекции с использованием реальных связей между аэропортами.  
- Analyze the impact of different infection probabilities on the rate of transmission.  
  Проанализировать влияние вероятности заражения на скорость распространения.  
- Determine key factors affecting infection spread.  
  Определить ключевые факторы, влияющие на распространение инфекции.  

---

## **Technologies / Технологии**  
- Python  
- Pandas  
- NumPy  
- NetworkX  
- Matplotlib / Seaborn  
- Scipy  
- Requests  

---

## **Files / Структура файлов**  
- `main.ipynb`:  
  - Contains data preprocessing, infection spread simulation, and result analysis.  
    Содержит предобработку данных, симуляцию распространения инфекции и анализ результатов.  
  - Uses real flight data to construct an airport network.  
    Использует реальные данные о перелётах для построения сети аэропортов.  
- `data/` (excluded from GitHub):  
  - Contains flight data for simulation, representing all flights in the United States during the year 2008.  
    Содержит данные о перелётах для симуляции, охватывающие все рейсы в США за 2008 год.  
  - Due to file size limitations, the dataset is not included and should be downloaded separately from [Kaggle](https://www.kaggle.com/datasets/vikalpdongre/us-flights-data-2008/data?select=2008.csv).  
    Из-за ограничений размера файлов, набор данных не включён в репозиторий и должен быть загружен отдельно с [Kaggle](https://www.kaggle.com/datasets/vikalpdongre/us-flights-data-2008/data?select=2008.csv).  

---

## **Results / Результаты**  
- **Infections spread rapidly, even with low probabilities.**  
  **Инфекция распространяется быстро, даже при низкой вероятности заражения.**  
- **Connectivity (degree) is the strongest factor influencing infection speed.**  
  **Количество рейсов (degree) – главный фактор, влияющий на скорость заражения.**  
- **The probability factor (`p`) has a non-linear impact on speed, with diminishing returns beyond `p=0.5`.**  
  **Фактор вероятности (`p`) оказывает нелинейное влияние, с уменьшением эффекта при `p > 0.5`.**  

---

## **Key Findings / Ключевые выводы**  
1. **Чем больше рейсов у аэропорта, тем быстрее распространяется инфекция.**  
2. **После определённого значения `p` (примерно 0.5) дальнейшее увеличение вероятности заражения не даёт значительного прироста в скорости распространения.**  

---

## **Conclusion / Заключение**  
This study highlights the critical role of flight connectivity in infection spread, demonstrating the advantages of using graph-based methods to identify crucial nodes and analyze transmission pathways, enabling more effective strategies for controlling and preventing the spread of infections.  
Данное исследование подчёркивает ключевую роль авиасообщений в распространении инфекции, демонстрируя преимущества использования графовых методов для выявления критически важных узлов и анализа путей передачи инфекции, что даёт возможность более эффективно разрабатывать стратегии контроля и предотвращения распространения.