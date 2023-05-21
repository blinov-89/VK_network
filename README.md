# Привет всем ![](https://github.com/blackcater/blackcater/raw/main/images/Hi.gif)

# VK_network
Предсказание интенсивности взаимодействия между пользователями, основываясь на информации об интенсивности других связей и пользовательской информации

#### Качество социального взаимодействия между пользователями ВКонтакте – почти всей аудиторией рунета

#### Типичный граф для конкретного ego_id

![image](https://github.com/blinov-89/VK_network/assets/61515881/6bb0f592-4386-4b02-8349-3ae33fd9d772)

## Задача регрессии

Базовая модель была улучшена путем генерации новых и дополнительных признаков

- 'time_sum_mean' - суммарное время эго-графа
- 'time_std' - стандартное отклонение эго-графа
- 'count' - количество связей в эго-графе
- 'mean' - среднее количество связей в эго-графе
- 'median' - медиану связей в эго-графе
- 'count_mean' - среднее количество связей в эго-графе
- 'time_sum_mean' - среднее количество связей в эго-графе на единицу времени


В рамках решения кейса от VK произведена обработка данных , произведен необходимый Feature engineering для более точного предсказания. Разработана модель предсказания интенсивности взаимодействия между пользователями

- Обработка категориальных признаков
- Работа с разнородными данными
- Работа с большими наборами данных

- агрегация внутри ego графа количество ребер у вершин пользователей
- агрегация внутри ego графа  суммарное вермя пользователя
- фильтруем только нужные данные и удаляем дубликаты
- мерджим к основым датасетам историю по пользователям

#### Важность признаков

![image](https://github.com/blinov-89/VK_network/assets/61515881/3856106c-7c1c-491c-b05e-1f0b7aa4c446)


## метрика RMSE

#### RMSE Fold2: 0.7317339398587932
#### RMSE mean: 0.7315434900806901

#### [Ссылка на соревнование и лидерборд](https://cups.online/ru/workareas/digital_breakout_2023/793/1494)

# Наше решение помогает пользователям находить новых друзей

