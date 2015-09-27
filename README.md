**Задача: механизм авторизации пользователя (для мессенджера).**

Пользователь должен быть описан классом. Система авторизации должна быть в отдельном модуле. Интерфейс консольный.

1. В консоли при запуске приложение предлагает авторизоваться. Если пользователь с таким именем существует, то проверяется пароль. 
Если не существует, то предлагается создать аккаунт пользователя. Пароль проверяется внутри приложения (можно хардкодить)

2. То же самое, но юзеры и пароли читаются/сохраняются в файл на диске

3. Пароль при вводе с консоли не показывается (смотрите java.io.Console)

4. Пароль хранится не в открытом виде, а хэшируется и в файл пишется только хэш

**Запуск:**
> $ javac -d ./classes src/com/acbelter/auth/AuthSystem.java -classpath src

> $ java -cp ./classes com.acbelter.auth.AuthSystem