# **Neural Network for Function Approximation**  
# **Использование нейросети для приближённого вычисления функции**  

This project presents a neural network-based approach for function approximation in a given range for both \(x\) and \(y\). The dataset is generated randomly, and a PyTorch model is trained to learn this function.  
В этом проекте представлена нейросетевая модель для аппроксимации функции в заданном диапазоне по \(x\) и \(y\). Данные генерируются случайным образом, а модель обучается в среде PyTorch.  

---

## **Goal / Цель**  
- Find an optimal neural network architecture that accurately approximates the target function on test data.  
  Найти такую архитектуру нейронной сети, которая бы очень точно на тестовых данных аппроксимировала исходную функцию.  
- Compare the model’s predictions with actual values.  
  Сравнить предсказания модели с реальными значениями.  

---

## **Technologies / Технологии**  
- Python  
- PyTorch  
- NumPy  
- Matplotlib / Seaborn  
- Scikit-learn  

---

## **Files / Структура файлов**  
- `main.py`:  
  - Implements the full process of function approximation, including data generation and splitting, model training and evaluation, and comparison of the real and approximated functions.  
    Реализован полный процесс аппроксимации функции, включая: генерацию и разбиение данных, обучение и оценку качества модели, сравнение реальной и аппроксимирующей функций.  

---

## **Results / Результаты**  
- **Final MSE on test set: 0.00134**  
  **Итоговая MSE на тесте: 0.00134**  
- **Training time: 3 min 22 sec**  
  **Время обучения: 3 мин 22 сек**  
- **Visualization: The graph is very similar to the original function, meaning the neural network successfully approximated the target function.**  
  **Визуализация: графики очень похожи, значит нейросеть успешно аппроксимировала целевую функцию.**