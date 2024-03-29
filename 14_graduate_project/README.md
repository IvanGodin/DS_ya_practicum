# Финальный проект. Промышленность.

Чтобы оптимизировать производственные расходы, металлургический комбинат ООО «Так закаляем сталь» решил уменьшить потребление электроэнергии на этапе обработки стали.

## Цель исследования:

Построить модель, которая предскажет температуру стали.

## Описание данных

Данные состоят из файлов, полученных из разных источников:

- `data_arc.csv` — данные об электродах;
- `data_bulk.csv` — данные о подаче сыпучих материалов (объём);
- `data_bulk_time.csv` — данные о подаче сыпучих материалов (время);
- `data_gas.csv` — данные о продувке сплава газом;
- `data_temp.csv` — результаты измерения температуры;
- `data_wire.csv` — данные о проволочных материалах (объём);
- `data_wire_time.csv` — данные о проволочных материалах (время).

Во всех файлах столбец key содержит номер партии. В файлах может быть несколько строк с одинаковым значением key: они соответствуют разным итерациям обработки.

## Используемые инструменты

`pandas` `matplotlib` `seaborn` `numpy` `sklearn` `catboost` `lightgbm`

### Модели

`LinearRegression` `RandomForestRegressor` `CatBoostRegressor` `LGBMRegressor`

### Дополнительно

`StandardScaler` `GridSearchCV` `cross_val_score`

### Метрики

`mean_squared_error`
