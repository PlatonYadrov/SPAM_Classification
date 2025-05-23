# Spam Detection NLP Project

Этот проект представляет собой реализацию модели классификации текстов на "спам" и "не спам" с использованием методов обработки естественного языка (NLP) и машинного обучения

## 📂 Структура проекта

- Загрузка и копирование данных с Google Drive
- Предобработка текстов:
  - Очистка от спецсимволов и знаков препинания
  - Приведение к нижнему регистру
  - Удаление стоп-слов
  - Стемминг (Porter Stemmer)
- Визуализация распределения слов и длины сообщений
- Работа с несбалансированными классами
- Обучение двух моделей:
  - Наивный Байесовский классификатор (`CountVectorizer`)
  - Логистическая регрессия (`Sklearn, TfidfVectorizer`)
  - Случайный лес (Sklearn)
  - Бустинг (XGBoost)
  - BERT + полносвязная сеть
- Оценка метрик точности, полноты, ROC AUC

## 📊 Данные

Файл `train_spam.csv` должен содержать два поля:

- `text` — текст сообщения
- `text_type` — `spam` или `ham` (не спам)

## ✅ Результаты

Модель позволяет эффективно определять, является ли сообщение спамом. Модель на основе NLP выдает результаты лучше, чем модели на основе классического машинного обучения

## 📌 Примечания

- Данные несбалансированы — возможно потребуется использование методов балансировки классов для улучшения результатов.
- Код легко расширить для других типов текстовой классификации.
