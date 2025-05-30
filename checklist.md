# Тестирование интерфейса

---

## Страница: Главная / Типы счетов

### Чек-лист

| Проверка                                                                                     | Статус     |
|----------------------------------------------------------------------------------------------|------------|
| Таблица загружается без ошибок.                                                              | Пройден    |
| Отображаются колонки: ID, Название, Описание, Статус.                                        | Пройден    |
| Для каждого созданного элемента автоматически генерируется уникальный ID                      | Пройден    |
| Поле Название и Описание принимает буквы (англ., каз.) и цифры                               | Пройден    |
| Есть placeholder «Имя и фамилия»                                                             | Пройден    |
| Поле не принимает запрещённые символы (например, спецсимволы: !@#$%^&* и т.п.)              | Не пройден |
| При вводе название слишком длинного текста запрещено                                         | Не пройден |
| При вводе пустого значения в любом из обязательных полей сохранение запрещено                | Пройден    |
| Проверить, что поле «Название» требует ввода как минимум двух слов (имя и фамилия), разделённых пробелом; значения без пробела не принимаются. | Не пройден |
| Колонки сортируются по убыванию и возрастанию при нажатии на заголовку/иконку сортировки     | Пройден    |
| Статусы отображаются корректно: "Активный", "Неактивный"                                    | Пройден    |
| Отображаются чекбоксы рядом с элементами                                                    | Пройден    |
| При выборе и снятии чекбоксов отображается актуальное количество выбранных элементов.        | Не пройден |
| Кнопка «Удалить» отображается на странице                                                    | Пройден    |
| При отсутствии выбранных элементов кнопка «Удалить» недоступна                              | Пройден    |
| При выборе одного или нескольких элемента кнопка «Удалить» становится доступной             | Пройден    |
| После нажатия на кнопку происходит удаление выбранных элементов, элементы исчезают из списка | Пройден    |
| Есть пагинация: на каждой странице отображается не более 10 элементов                        | Пройден    |
| Поиск работает по всем колонкам таблицы: при вводе запроса результаты показываются, если совпадение есть в любой из колонок | Пройден    |
| Кнопка «Добавить тип счета» доступна и видна                                                | Пройден    |
| При нажатии открывается форма с полями: название, описание, статус и с кнопками отмена, создать | Пройден    |
| Поле статус по умолчанию выключено (OFF)                                                   | Пройден    |


## Страница: Главная / Счета

### Чек-лист

| Проверка                                                                                     | Статус     |
|----------------------------------------------------------------------------------------------|------------|
| Таблица загружается корректно и в форме есть поля:  ID, Название, Баланс, Валюта, Тип, Отрицательный баланс, Описание, Статус |            |
| Для каждого созданного элемента автоматически генерируется уникальный ID                      | Пройден    |
| Поле Название и Описание принимает буквы (англ., каз.) и цифры                               | Пройден    |
| Есть placeholder «Имя и фамилия»                                                             | Пройден    |
| Поле не принимает запрещённые символы (например, спецсимволы: !@#$%^&* и т.п.)              | Не пройден |
| При вводе название слишком длинного текста запрещено                                         | Не пройден |
| При вводе пустого значения в любом из обязательных полей сохранение запрещено                | Пройден    |
| Проверить, что поле «Название» требует ввода как минимум двух слов (имя и фамилия), разделённых пробелом; значения без пробела не принимаются. | Не пройден |
| Колонки сортируются по убыванию и возрастанию при нажатии на заголовку/иконку сортировки     | Пройден    |
| Статусы отображаются корректно: "Активный" - зеленым цветом, "Неактивный" - красным цветом  |            |
| Отображаются чекбоксы рядом с элементами                                                    | Пройден    |
| При выборе и снятии чекбоксов отображается актуальное количество выбранных элементов.        | Не пройден |
| Кнопка «Удалить» отображается на странице                                                    | Пройден    |
| При отсутствии выбранных элементов кнопка «Удалить» недоступна                              | Пройден    |
| При выборе одного или нескольких элемента кнопка «Удалить» становится доступной             | Пройден    |
| После нажатия на кнопку происходит удаление выбранных элементов, элементы исчезают из списка | Пройден    |
| Есть пагинация: на каждой странице отображается не более 10 элементов                        | Пройден    |
| Поиск работает по всем колонкам таблицы: при вводе запроса результаты показываются, если совпадение есть в любой из колонок | Пройден    |
| Кнопка «Добавить тип счета» доступна и видна                                                | Пройден    |
| При нажатии открывается форма с полями: название, описание, статус и с кнопками отмена, создать | Пройден    |
| Поле статус по умолчанию выключено (OFF)                                                   | Пройден    |
| При нажатии Отменить форма закрывается без сохранения                                      | Пройден    |
| При вводе данных и нажатии Сохранить форма закрывается и тип счета добавляется в список    | Пройден    |
| Если не заполнено название, сохранение невозможно (валидация)                              | Не пройден |
| При нажатии Отмена форма закрывается без сохранения                                        | Пройден    |
| При нажатии Создать с заполненными данными — счёт добавляется в таблицу                     | Пройден    |
| Если поле Название не заполнено — форма не сохраняется                                     | Пройден    |
| Поле Баланс принимает дробные числа с точкой (например: 100.50)                            | Пройден    |
| Поле Баланс не принимает отрицательные значения, даже если включён чекбокс «Отрицательный баланс» | Не пройден |
| Поле Баланс не принимает любые символы, кроме цифр и одной точки                          | Пройден    |
| Поле «Баланс» принимает только числовое значение с одной точкой, если она находится между цифрами | Пройден    |
| Доступны следующие значения: KZT, USD, RUB, EUR                                           | Пройден    |
| Валюта выбирается при добавлении счёта                                                    | Пройден    |
| В таблице реализована сортировка по колонке «Валюта»                                      | Пройден    |
