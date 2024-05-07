# Список недоработок

Разработан в качестве практичеcкого задания на курсе PHPDEV-1004. Является результатом выполнения **Модуль 20. Стандарты написания кода и общие подходы**

---

## Цель проекта

Освоить основные принципы написания "Чистого кода"

## Используемые принципы

* YAGNI

* KISS

* DRY

* SOLID


**YAGNI**

Удаление участков кода в частности 
@media(max-width:1140px), что исключает излишнюю детализацию не требуемую в техзадании.

Удалены некоторые "margin" и "padding"   с учетом допустимой погрешности  при верстке 3-6 px у элементов DOM.


**KISS**

Элементам списка  и ссылкам, а также элементам div section class="repair" применены  общие классы, что исключает необходимость описания стилей каждого элемента.

Медиа-запрос @media(max-width:1256px) расширен и доработан, что привело к оптимизации других медиа-запросов.

Уменьшено колличество вынесенных общих стилей, созданы общие стили которые унифицируют предыдущие.

Названия блоков и элементов упрощено с учетом отражения поведения сущности и требований БЭМ, выстроена логическая связь между элементами.

Использованы свойства наследования классов.


**DRY**
Удалены стили у кнопок (модификаторов), которые применялись в стилях блоков и элементов;

Удалены стили у заголовков (модификаторов ), которые применялись в стилях блоков и элементов;

Удалены перекрещивающиеся "margine" и "padding" у родительских классов и "наследников" ;

Удалены перекрещивающиеся стили "font-size", "line-height ", "font-family" у родительских классов и "наследников" ;

**SOLID**

***Single responsibility principle:***

Внешняя геометрия и позиционирование элементов осуществляется с помощью блока или элемента, в то время как у модификаторов для отражения функционального поведения, оставлены стили связанные с изменением цвета,размера шрифта. 

***Open-Closed Principle:***

Реализован с помощью применения миксов для стилизации элементов.
А также в некоторых случаях используется модификация контекстом(ст.1277,1290,1303,1364).


**Доработака верстки по БЭМ**
 
Изменены названия блоков, элементов, добавлены модификаторы.

Перераспределены стили между блоками , элементами и модификаторами.

Всем элементам Dom прописаны классы.

В описаниях стилей  исключены селекторы тэгов и селекторы идентификаторов.

Исключено повышение специфичности селекторов связанное с их совместным использованием.

Названия элементов изменены с учетом осмысления сущности и отражения логики построения зависимостей элементов.

**Семантика и валидность верстки проверена W3C**

**Линтеры которые использовались для проверки кода на наличие ошибок и приведения его в порядок:**
 
 * Code Spell Checker 
 * Beautify

## Как открыть/запустить

В представленной папке содержаться две подпапки.

1-Первоначальная версия сайта

2-С исправленным html и scc кодом, а также со списком недоработок.


Зайти в папку сайта в файловом менеджере, кликнуть 2 раза по файлу index.html. 