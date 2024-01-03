# NLU Classifier 📚

## Описание 🌟

`NLU_Classifier` - это классификатор для обработки естественного языка (NLU), специализирующийся на поиске и классификации терминов и запросов.

## Особенности 🛠️

- Использует предобученные модели для извлечения контекстной информации и классификации запросов.
- Поддерживает обработку синонимов для более точного поиска.
- Вычисляет векторные представления для списка данных.

## Установка 📦

Для работы классификатора требуется Python 3.6+ и следующие библиотеки:
- `torch`
- `sentence_transformers`
- `transformers`
- `docx`
- `re`

## Использование 🔍

```python
from NLU_Classifier import NLU_Classifier

# Инициализация классификатора с путем к предобученной модели NLU
classifier = NLU_Classifier(nlu_model="path_to_model")

# Инициализация контекста диалога
classifier.init_context_dialog(file_path="path_to_data_file")

# Получение контекста для заданного вопроса
context = classifier.get_context(question="your_question_here")
