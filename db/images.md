# Изображения
Универсальная таблица не принадлежащая другим таблицам. В базе данных храним локальную ссылку на оригинал изображения, на сайте автоматически генерируются необходимые размеры. Рекомендуем обрабатывать изображения с помощью двух пакетов: сначала [spatie/image-optimizer](https://github.com/spatie/image-optimizer) оптимизировать вес а потом [imagine/imagine](https://github.com/avalanche123/Imagine) генерировать в указанный размер.
## images
- `id` - integer - технический id
- `image_id` - integer - основной id
- `site_id` - integer - сайт
- `table_name` - string - название таблицы `product`
- `unit_id` - integer - id записи
- `image_path` - string - локальный URL
- `alias` - string - алиас для URL
- `sort` - integer - сортировка
- `state` - integer - статус
- `score` - integer - количество запросов
### `images` schema - структура таблицы
```json
{
"image_id": "integer",
"site_id": "integer",
"table_name": "string",
"unit_id": "integer",
"image_path": "string",
"sort": "integer",
"alias": "string",
"state": "integer",
"score": "string"
}
```
