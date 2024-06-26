[![Build status](https://ci.appveyor.com/api/projects/status/djpacjee3rpgy85o/branch/master?svg=true)](https://ci.appveyor.com/project/Tryd0g0lik/test-table/branch/master)


# The task description
**Формулировка**: \
Необходимо реализовать модель таблицы, в которую можно вносить данные. \
**Требования**: 
- Таблица должна являться javascript. 
- Добавление/ Удаление строк.
- Необходимо реализовать функцию для загрузки данных в таблицу из json файла.
- Возможны следующие типы для колонок: number, string, boolean.

Данный функционал необходимо реализовать на javascript или ReactJS без использования дополнительных библиотек. \
Визуальную часть реализовать по своему усмотрению, спорные моменты по дизайну также по своему усмотрению.

## О работе
- [Front развернут](https://tryd0g0lik.github.io/test-table/) на `github-pages`
- Backend на внешнем сервере.
Открывая фронт подождите 50 секундю Время для запуска сервера.


Вся логика писалась с целью создать код как можно больше динамичным и как можно меньше статичных данных \ 
Например для реаллизации той же технологии dnd в дальнейшем.


### Казус
Первая загрузка данных на страницу реализована [через Redux](https://github.com/Tryd0g0lik/test-table/tree/master/src/frontend/src/reduxs). \
Казус в том, что при первичной загрузки страницы логика срабатывает быстрее, запускается внешний сервер. Поэтому страница кажется пустой.
Спустя 50 секунд работают [добавление](https://github.com/Tryd0g0lik/test-table/blob/8b46e01fbd47e616cd9f5de6f49a45685358c86c/src/backend/src/server.js#L21-L40)/[удаление](https://github.com/Tryd0g0lik/test-table/blob/8b46e01fbd47e616cd9f5de6f49a45685358c86c/src/backend/src/server.js#L86-L101) данных на сервер. \
В локальном режиме работает все сразу.


## Stack 
- NodeJS
- TS
- React
- Redux
- webpack
- daisyui
- tailwindcss

- [Backend](https://github.com/Tryd0g0lik/test-table/tree/master/src/backend)
- [Frontend](https://github.com/Tryd0g0lik/test-table/tree/master/src/frontend)

## Command 

 - `server:front` this's  start wark for a local [server of front](https://github.com/Tryd0g0lik/test-table/blob/8b46e01fbd47e616cd9f5de6f49a45685358c86c/package.json#L14);
 - `cssstyle` here styles of out framework. This [command is a runs styles](https://github.com/Tryd0g0lik/test-table/blob/8b46e01fbd47e616cd9f5de6f49a45685358c86c/package.json#L17) for local developmentж
 - `watchs` [run the `server.js'](https://github.com/Tryd0g0lik/test-table/blob/8b46e01fbd47e616cd9f5de6f49a45685358c86c/package.json#L19) of backend
 
## History
- [master]: github's root;
- [1]: Beginning works. Here a htaml table and datas backend was added ;
- [2.1]: redux was added and fixed function ADD and REMOVE was; 

## View
![pic](./Screenshot_22.png)
