# Customer Segmentation for a German Bank Using Clustering and Dimensionality Reduction  
# Сегментация клиентов немецкого банка при помощи методов кластеризации и уменьшения размерности  

This project focuses on segmenting customers of a German bank using clustering algorithms and dimensionality reduction techniques.  
Этот проект посвящён сегментации клиентов немецкого банка с использованием методов кластеризации и уменьшения размерности.

---

## Goal / Цель  
- Perform customer segmentation to identify distinct customer groups.  
  Провести сегментацию клиентов для выявления различных групп.  
- Use clustering algorithms (KMeans, DBSCAN, Hierarchical Clustering) and dimensionality reduction techniques (PCA, t-SNE, UMAP).  
  Использовать алгоритмы кластеризации (KMeans, DBSCAN, иерархическая кластеризация) и методы уменьшения размерности (PCA, t-SNE, UMAP).

---

## Technologies / Технологии  
- Python  
- KMeans  
- DBSCAN  
- Hierarchical Clustering  
- PCA  
- t-SNE  
- UMAP  
- Pandas  
- Matplotlib / Seaborn  

---

## Files / Структура файлов  
- `main.ipynb`:  
  - Contains data preprocessing, clustering implementation, and visualization of results.  
    Содержит предобработку данных, реализацию кластеризации и визуализацию результатов.  
  - Includes comparison of clustering algorithms.  
    Включает сравнение различных алгоритмов кластеризации.  
- `data/german_credit_data.csv`:  
  - The dataset used for segmentation.  
    Набор данных, использованный для сегментации.  

---

## Results / Результаты  
The analysis yielded the following insights:  
Анализ дал следующие результаты:  

1. **Clustering Performance / Результаты кластеризации**  
   - All three clustering algorithms (KMeans, DBSCAN, and Hierarchical Clustering) achieved comparable silhouette scores.  
     Все три алгоритма кластеризации (KMeans, DBSCAN и иерархическая кластеризация) показали схожие значения коэффициента силуэта.  
   - Among them, **DBSCAN** demonstrated a slightly higher silhouette score, making it the best performer in terms of this metric.  
     Среди них **DBSCAN** продемонстрировал немного более высокий коэффициент силуэта, что делает его лучшим по этой метрике.  

2. **Dimensionality Reduction / Уменьшение размерности**  
   - The **PCA** technique proved to be the most effective for visualizing clusters, clearly separating distinct groups in a reduced dimensional space.  
     Метод **PCA** оказался наиболее эффективным для визуализации кластеров, чётко разделяя группы в уменьшенном пространстве.  
   - Techniques like t-SNE and UMAP were also explored but did not provide as clear separation as PCA for this dataset.  
     Также были исследованы методы t-SNE и UMAP, но они не дали столь чёткого разделения, как PCA, для данного набора данных.  

3. **Cluster Interpretation / Интерпретация кластеров**  
   - DBSCAN initially identified **8 clusters** along with a group of outliers.  
     DBSCAN изначально выделил **8 кластеров** и группу выбросов.  
   - For better interpretability, similar clusters were combined into **4 major groups**, simplifying analysis and enhancing insights.  
     Для улучшения интерпретации похожие кластеры были объединены в **4 основные группы**, что упростило анализ и позволило получить более ценные инсайты.  


---

## Summary / Резюме  
The project highlights the importance of interpreting clustering results beyond metrics like silhouette score. Combining clustering with dimensionality reduction (e.g., PCA) and domain knowledge helps derive actionable insights for better customer segmentation.  
Проект подчёркивает важность интерпретации результатов кластеризации, выходящей за рамки метрик, таких как коэффициент силуэта. Комбинация кластеризации с уменьшением размерности (например, PCA) и использованием экспертного знания помогает получать практические инсайты для улучшения сегментации клиентов.
