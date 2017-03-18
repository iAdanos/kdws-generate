# kdws-generate
Script generates a part of winroute.cfg for Kerio Control to block Microsoft Telemetry hosts and domains.  
You need manualy insert script's result in your winroute.cfg and restart Kerio Control.


Usage:
> ./kdws-deterate 999  

Where: 999 - ID of your last entry in IP groups config part.

-----

Скрипт генерирует часть конфигурационного файла winroute.cfg для Kerio Control, добавляя в секцию "Группы IP" список доменов и IP-адресов, на которые отправляются данные телеметрии от Майкрософт.  
Результат работы скрипта необходимо собственноручно добавить в winroute.cfg и перезапустить Kerio Control.

Пример использования:
> ./kdws-deterate 999  

Где: 999 - ID последней записи в секции "Группы IP" внутри winroute.cfg.

-----

Списки IP и доменов взяты из [DWS Lite](https://github.com/Nummer/Destroy-Windows-10-Spying), за что огромное спасибо создателям.

Скорее всего, репозиторий не будет поддерживаться, но его можно форкать и отправлять пулл-реквесты.