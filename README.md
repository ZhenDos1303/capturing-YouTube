# Проект конверсии пользователей из YouTube в VK video с максимальной эффективностью

## Выполнили
- Борисов Евгений ББИ2406
- Лебедев Фёдор ББИ2406
- Точилкина Екатерина ББИ2406

## Описание проекта

Проект направлен на анализ и оптимизацию конверсии пользователей из YouTube в VK video путем анализа данных о видео, каналах и их характеристиках.

## Этапы проекта

### 1. Создание датасета по ВК API
- **Ноутбук:** `VK_Video_Data_Collection.ipynb` (для запуска нужен ключ VK)
- **Результат:** `vk_videos_dataset_extended_15k.xlsx`
- Сбор данных о видео из VK через API

### 2. Сопоставление видео с YouTube
- **Ноутбук:** `YouTube_Video_Parsing.ipynb` (для запуска нужен Google Chrome)
- **Результат:** `youtube_videos_dataset.xlsx`
- Поиск и сопоставление видео из VK с соответствующими видео на YouTube

### 3. Объединение датасетов
- **Результат:** `merged_vk_youtube_dataset_with_categories.xlsx`
- Объединение данных из VK и YouTube в единый датасет

### 4. Добавление категорий и очистка данных
- **Ноутбук:** `Add_YouTube_Categories.ipynb` (для запуска нужен ключ YouTube)
- **Результат:** `final_vk_youtube_dataset.xlsx`
- Добавление категорий к каждому видео через YouTube API
- Удаление пропусков и дубликатов

### 5. EDA и анализ данных
- **Ноутбук:** `Combined_Analysis.ipynb`
- Проведение exploratory data analysis
- Анализ полученных данных для выявления закономерностей

### 6. Определение параметров видео
- Получение параметров видео, наиболее подходящих для VK video
- На основе результатов EDA

### 7. Поиск каналов по параметрам
- **Ноутбук:** `Find_Gaming_Channels.ipynb`
- **Результат:** `all_channels_stats.xlsx`
- Поиск каналов YouTube, соответствующих определенным параметрам
- Получение статистики по найденным каналам

### 8. Фильтрация каналов
- **Результат:** `Podhodyashie_channels.xlsx`
- Фильтрация каналов по нужным параметрам
- Отбор наиболее подходящих каналов

### 9. Получение детальной статистики по каналам
- **Ноутбук:** `Process_Channels_Stats.ipynb` (для запуска нужен ключ YouTube)
- **Результат:** `Podhodyashie_channels_with_stats.xlsx`
- Получение информации из YouTube API:
  - Количество подписчиков
  - Количество просмотров
  - Другие метрики

### 10. Анализ результатов и рекомендации
- Анализ полученного датасета
- Формулирование конкретных рекомендаций для оптимизации конверсии

## Структура файлов

```
VK_Video_Data_Collection.ipynb
YouTube_Video_Parsing.ipynb
Add_YouTube_Categories.ipynb
Combined_Analysis.ipynb
Find_Gaming_Channels.ipynb
Process_Channels_Stats.ipynb
vk_videos_dataset_extended_15k.xlsx
youtube_videos_dataset.xlsx
merged_vk_youtube_dataset_with_categories.xlsx
final_vk_youtube_dataset.xlsx
all_channels_stats.xlsx
Podhodyashie_channels.xlsx
Podhodyashie_channels_with_stats.xlsx
```


