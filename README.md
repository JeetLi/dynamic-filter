<h1>Тестовое задание "Dynamic-Filter"</h1>

<h3>Задачи:</h3>

1) Сверстать по макету фильтр и список квартир.
    - Цвета и шрифты использовать те, что прописаны в файле ***tailwind.config.ts*** и ***globals.scss***
    - Для кастомных стилей(если понадобится) создать и использовать ***custom.scss***
    - Необходимо, чтобы верстка была адаптивной
    - При необходимости создавать отдельные компоненты только для мобильной версии
2) Написать логику работы фильтра, а так же получения и отрисовки квартир.
   - При переключении фильтра, остальные фильтра должны подстраиваться под заданное значение. Например выбирается проект "Тестовый", у этого проекта доступны только квартиры с комнатностью 2, соотвественно для дальнейшеного выбора доступно только выбор комнатностьи со значением "2".
   - Вся фильтрация для фильтра и квартир происходит на беке.
   - Фильтр не должен "схлапываться", то есть не должно быть такого, что в выдаче нет квартир и фильтр показывает не корректные значения. Например стоимость от 0 до 0.
   - Все выбранные значения фильтра должны записываться в query параметры. И при копировании url с query параметрами и вставки в новом окне браузера значения фильтров должны поставляться и должна просходить фильтрация квартир

<h4>Можно использовать любые инструменты<h4>

***
<h3>Технические требования:</h3>

1) Docker и docker-compose
2) Node.js >19.7.0 
***
<h3>Необходимые материалы</h3>

1) [Макет в фигме](https://www.figma.com/file/KS3E1LkarFwFQD90K1BUGN/%D0%A2%D0%B5%D1%81%D1%82%D0%BE%D0%B2%D0%BE%D0%B5-%D0%B7%D0%B0%D0%B4%D0%B0%D0%BD%D0%B8%D0%B5-(Frontend)?type=design&node-id=4-229&mode=design&t=30jNLqdVcubjNOxp-0)
2) [Документация по api](http://localhost:8083/)
**Будет доступна после установки проекта**
***
<h3>Инструкция по установке проекта:</h3>

Из корня проекта вызываем команду:

```php
make init
```

***
<h3>Инструкция по запуску проекта</h3>

1) Из корня проекта вызываем команду:

```php
make up
```

Адрес бекенда
[http://localhost:8083/](http://localhost:8083/)

Документация апи
[http://localhost:8083/api/documentation](http://localhost:8083/api/documentation)

2) Из папки ***frontend*** вызываем команды:
```php
npm i && npm run dev
```
Проект откроется по адресу
[http://localhost:3000/](http://localhost:3000/)

3) Для того чтобы остановить контейнеры Docker из папки проекта вызываем команду:
```php
make stop
```
***
<h3>Ожидаемый результат:</h3>

1) из папки ***frontend*** выполняется команда:
```php
npm run lint
```
**Все проверки линтера проходят успешно**

2) из папки ***frontend*** выполняются команды:
```php
npm run build && npm run start
```
**Билд успешно собирается и проект открывается по адресу**
[http://localhost:3000/](http://localhost:3000/)

3) Верстка сделана согласно макету, так же сделан адаптив этой страницы
4) При переключении фильтра квартиры фильтруются и фильтр подстраивается под уже отмеченные значения
5) При переключении фильтр в адресной строке добавляются query парметры
6) При копировании ссылки с  query параметрами и вставки их в новом окне браузера происходит постановка значений в фильтр и фильтрация квартир
***
<h4>Готовый результат выложить в гитхаб и отправить ссылку на репозиторий</h4>
