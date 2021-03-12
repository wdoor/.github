
# WrongDoor

### Модули:
* [wrong-door-api] - Node.js GraphQL-API для хранения-обработки информации.
* [wrong-door-mobile] (refactoring) - Kotlin Android App, где и происходит взаимодействие с пользователем.
* [SmartCollegeConnecter] - Клиент GraphQL-API для C#(Оказывается, что клиенты для GraphQL не так популярны на c#!!!).
* [CommandExecutor] - Исполняющий команды сервер, подлючается к [SmartCollegeConnecter].
* [SmartCollegeRoom] (refactoring) - Исполняющий команды сервер, который запускается на отдельном компьютере, предоставляя дополнительный функционал относительно [CommandExecutor], подлючается к [SmartCollegeConnecter], ссылки нет т.к. мне стыдно.


#### Это программное решение для удаленного управления "локальной сетью" через мобильное приложение.

### Проблема: 
> Существует некий компьютер, доступ к которому ограничен тем, что он находится за роутером и никакие порты в его сторону не открыты, оный компьютер должен выполнять заданные пользователем команды, обрабатывая ошибки и оставаясь работоспособным максимальное количество времени.

### Решение 
> Мобильное приложение <---> API <--->  Исполняюший команды сервер

> Пользователь <---> Сервер <--->  "Зараженный" компьютер

[SmartCollegeConnecter]: <https://github.com/stercoris/SmartCollegeConnecter>
[CommandExecutor]: <https://github.com/stercoris/CommandExecutor>
[wrong-door-mobile]: <https://github.com/stercoris/wrong-door-mobile>
[wrong-door-api]: <https://github.com/stercoris/wrong-door-api>
[SmartCollegeRoom]: <>

