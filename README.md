# Gmaps testing project

* to install run command grunt-build
* to run project run command grunt

#Description

Single-page по управлению локациями.

Для работы с локациямии исполозовался Google Maps Javascript API, https://developers.google.com/maps/documentation/javascript/.

Приложение представляет собой простой список локаций.
Данные для списка хранятся в и берутся из localStorage.

Возможные действия с локациями:
 - добавление
 - удаление
 - редактирование

Свойства локации:
 - имя
 - координаты (lat, lng)
 - адрес

Локация в списке представлена google map плагином, на котором локация отмечена маркером.

В обычном режиме (по умолчанию):
 - показывается информация о локации (имя, адрес, координаты) в виде статического текста;
 - карта центрируется в точке локации при переходе в обычный режим, т.е. при:
   - загрузке страницы,
   - добавлении новой локации,
   - выходе из режима редактирования;
 - две кнопки - для удаления локации и перехода в режим редактирования

В режиме редактирования:
 - показываются поля для редактирования имени, адреса, координат;
 - при изменении поля адреса изменяються значения координат и положение маркера;
 - при изменении полей координат изменяються адрес и положение маркера;
 - две кнопки - для сохранения и отмены изменений (обе переводят в обычный режим)