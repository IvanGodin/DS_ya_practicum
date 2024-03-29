# Определение стоимости автомобилей

## Описание проекта

Сервис по продаже автомобилей с пробегом разрабатывает приложение для привлечения новых клиентов. 
В нём можно быстро узнать рыночную стоимость своего автомобиля. Для этого необходимо построить модель для определения этой стоимости.
В вашем распоряжении исторические данные: технические характеристики, комплектации и цены автомобилей. 

*Заказчику важны*:
1. качество предсказания;
2. скорость предсказания;
3. время обучения.

## Описание данных

Признаки
- `DateCrawled` — дата скачивания анкеты из базы
- `VehicleType` — тип автомобильного кузова
- `RegistrationYear` — год регистрации автомобиля
- `Gearbox` — тип коробки передач
- `Power` — мощность (л. с.)
- `Model` — модель автомобиля
- `Kilometer` — пробег (км)
- `RegistrationMonth` — месяц регистрации автомобиля
- `FuelType` — тип топлива
- `Brand` — марка автомобиля
- `NotRepaired` — была машина в ремонте или нет
- `DateCreated` — дата создания анкеты
- `NumberOfPictures` — количество фотографий автомобиля
- `PostalCode` — почтовый индекс владельца анкеты (пользователя)
- `LastSeen` — дата последней активности пользователя

Целевой признак
- `Price` — цена (евро)

## Используемые инструменты

`pandas` `matplotlib` `numpy` `sklearn` `lightgbm` `catboost`

### Модели

`LinearRegression` `DecisionTreeRegressor` `LGBMRegressor` `CatBoostRegressor`

### Дополнительно

`StandardScaler` `GridSearchCV`

### Метрики

`mean_squared_error`
