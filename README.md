# 🇷🇺 Russian Sentiment Classifier (PyTorch, GRU)

Проект по классификации тональности текстов на русском языке — `positive`, `neutral`, `negative` — с использованием нейросети на PyTorch.

## 🚀 Основные возможности

- ✅ Классификация тональности русскоязычных текстов
- 🧠 Нейросеть с Embedding → GRU → Linear
- 🗃 Собственный словарь и кодирование токенов
- 🧼 Preprocessing: очистка текста, токенизация
- 🏎 Обучение на GPU (если доступно)
- 📉 Scheduler для управления learning rate
- 💬 Поддержка ручного ввода и интерактивного `predict()`

## 📦 Стек технологий

- Python
- PyTorch
- pandas, tqdm
- TorchText не используется — всё вручную

## 🧠 Архитектура модели

```python
Input → Embedding → GRU → Linear → Softmax
