# VSTUInteractiveMap

## Проект, реализующий интерактивная карту на сайте вуза ВГТУ

Проект должен представлять собой веб-сайт с резиновой версткой, умеющий адаптироваться под мобильные устройства. На сайте должен иметься функционал для трех ролей:
- студент;
- преподаватель;
- диспетчер расписания.

Для каждой из ролей должен быть реализован соответствующий функционал:
- студент
  * построение маршрута об близлежащей аудитории до другой выбранной аудитории;
  * поиск аудитории на карте по запросу или интерактивно;
  * поиск деканата, туалета, буфета.
 
- преподаватель
  * просмотр занятых аудиторий;
  * отправка запроса на бронирование.
 
- диспетчер расписания
  * подтверждение запроса на бронь;
  * отклонение запроса на бронь.

## Техническая реализация

**Фронтовая часть** будет реализована с использованием фреймворка `Angular`. Вся основная логика будет производитсья на фронтовой части и написана на языке `TypeScript`. К этой логике относится:
- поиск аудитории и подсветка на карте результата;
- построение маршрута и его отображение;
- отправка запроса на бронирование и снятие брони.

**Бэковая часть** будет реализована на Java с использованием фреймворка `Spring Boot`. К серверной логике относится:
- аутентификация;
- вычисление расписания на определенный день;
- вычисление занятых и свободных аудиторий;
- бронирование и снятие брони аудиторий.

Для **аутентификации** будет использовано `Moodle API`.

В качестве **базы данных** будет использована `PostgreSQL`.
