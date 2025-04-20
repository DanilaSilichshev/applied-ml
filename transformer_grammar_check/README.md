# **Grammatical Acceptability Classification using Transformer Models**  
# **Оценка грамматической корректности предложений с использованием трансформерных моделей**

This project focuses on evaluating different approaches to grammatical acceptability classification in Russian using the RuCoLA dataset.  
Этот проект посвящён тестированию различных подходов к определению грамматической корректности предложений на русском языке на основе корпуса RuCoLA.

---

## **Goal / Цель**
- Test both fine-tuned transformer models and zero-/few-shot generative models.  
  Протестировать как дообученные трансформерные модели, так и генеративные модели в zero-/few-shot режимах.

---

## **Technologies / Технологии**
- Python  
- Hugging Face Transformers  
- PyTorch  
- Scikit-learn  
- Google Colab

---

## **Files / Файлы**
- `main.ipynb`  
  Main Jupyter Notebook with data loading, training, generation, evaluation.  
  Основной Jupyter Notebook с загрузкой данных, обучением, генерацией и анализом.
- `data/in_domain_train.csv`, `data/in_domain_dev.csv`  
  Labeled data from RuCoLA corpus.  
  Размеченные данные из корпуса RuCoLA.

---

## **Models / Модели**
- **RuBERT (DeepPavlov/rubert-base-cased)**: fine-tuned for binary classification  
  Дообученная модель RuBERT (DeepPavlov) для классификации предложений.
- **RuGPT3 (sberbank-ai/rugpt3large_based_on_gpt2)**: zero-/few-shot generation using different prompt styles  
  Модель RuGPT3 для генерации ответов в zero-/few-shot режиме с разными стилями затравок.

---

## **Results / Результаты**
- **RuBERT** achieved best F1 ≈ 0.87 on validation set (epoch 2).  
  Модель RuBERT показала наилучший F1 ≈ 0.87 на валидации (2-я эпоха).
- **Recall** for incorrect sentences was low → model tends to miss ungrammatical cases.  
  Recall для класса "некорректные" оказался низким — модель склонна их пропускать.
- **Weighted F1-score on the test set was ≈ 0.77**, even **without hyperparameter tuning**, which indicates a decent generalization.  
  Средневзвешенный F1-score на тестовой выборке составил ≈ 0.77, даже **без подбора гиперпараметров**, что говорит о неплохом качестве обобщения.  
- **RuGPT3** performed reasonably with 1–2 few-shot examples.  
  RuGPT3 даёт адекватные ответы уже при 1–2 затравках.

---

## **Summary / Резюме**
This project demonstrates that transformer-based models can effectively distinguish grammatical correctness in Russian.  
Проект демонстрирует, что трансформерные модели способны эффективно различать грамматически корректные и некорректные предложения на русском языке.

Fine-tuned models outperform generative ones in accuracy, but zero-/few-shot inference is flexible and useful in low-resource settings.  
Дообученные модели дают лучшее качество, однако генеративный подход более гибкий и применим при ограниченных данных.

---

## **Further Improvements / Возможные улучшения**
- Add class weighting to the loss function to improve recall on minority class.  
  Добавить веса классов в функцию потерь для повышения recall у минорного класса.
- Improve prompt templates for RuGPT3 to reduce ambiguity.  
  Улучшить шаблоны затравок для RuGPT3, чтобы повысить однозначность.
- Try alternative models (both generative and classification) to improve performance.  
  Протестировать альтернативные модели (как генеративные, так и классификационные), чтобы повысить итоговое качество.