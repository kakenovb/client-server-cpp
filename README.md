# client-server-cpp

Проект содержит реализацию сервера который работает с несколькими клиентами. Сервер работает в бесконечном цикле обрабатывая каждого нового клиента в новом потоке (завершение через прерывание ctrl+c). Клиенту можно передать имя переменной окружения в которой будет храниться порт сервера (который нужно прежде  установить для сервера). Логгирование происходит при помощи boost.log. 

Для сборки CMake в директории проекта:

cmake -S ./src -B ./build

cmake --build ./build

Запуск:

./build/server

./build/client
