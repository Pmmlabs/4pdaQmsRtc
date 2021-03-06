4pdaQmsRtc
==========

Юзерскрипт для добавления функции передачи файлов в личке 4pda

Требования к ПО
--
   - Firefox 19 или выше
   - дополнение [Scriptish](http://scriptish.org/) (или [GreaseMonkey](http://www.greasespot.net/))
  
или

   - Chrome 25 или выше
   - дополнение [TamperMonkey](https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo?hl=ru)

Описание
--
После установки скрипта в окошке набора сообщения появляются элементы управления для отправки файлов.

Файлы передаются напрямую, без всяких облачных сервисов, с использованием технологии WebRTC.

Работает на библиотеке RTCMultiConnection и для использует для сигналинга публичный аккаунт Firebase.

Файлы библиотек RTCMultiConnection и Firebase лежат рядом, потому что стабильность серверов гитхаба лучше, чем сайта, откуда я их взял.

[![YouTube](http://img.youtube.com/vi/GoITwdFTjBY/1.jpg)](http://www.youtube.com/watch?v=GoITwdFTjBY) - смотреть краткий обзор на Youtube
Установка
--
   - Установите дополнение соответственно вашему браузеру (см. Требования к ПО)
   - Установите скрипт https://greasyfork.org/scripts/238/code.user.js

Домашняя страница на Greasyfork: https://greasyfork.org/scripts/238

Известная проблема
--
В Firefox иногда не передаются файлы, тогда нужно обновить страницу. Ошибка связана с неприспособленностью клиентской библиотеки Firebase к использованию в юзерскриптах. Следует найти способ определить, установилось ли соединение с сервером Firebase или нет. Пока что это не удаётся сделать.