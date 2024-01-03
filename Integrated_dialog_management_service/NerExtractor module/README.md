# NerExtractor 📘

## Описание 🌐

`NerExtractor` - это класс для извлечения именованных сущностей (NER) из текста, использующий предобученные модели из библиотеки `transformers`.

## Основные характеристики 📌

- Использование пайплайна `transformers` для классификации токенов и извлечения сущностей.
- Объединение соседних сущностей одного типа в одну сущность для повышения точности.

## Установка и зависимости 🛠️

Требуется Python 3.6+ и следующие библиотеки:
- `transformers`

## Использование 🔍

```python
from NerExtractor import NerExtractor

# Создание экземпляра NerExtractor
ner_extractor = NerExtractor(model_checkpoint="path_to_model_checkpoint")

# Извлечение сущностей из текста
entities = ner_extractor.get_entities("Ваш текст здесь")
