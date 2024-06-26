# Работа с сохраненными SQL-запросами

{% include notitle [preview](../../_includes/note-preview.md) %}

Любой SQL-запрос может быть сохранен для дальнейшего использования и создания шаблона.

## Сохранить запрос {#custom-templates}

Чтобы сохранить запрос:

1. На панели данных, для любого запроса нажмите ![image](../../_assets/console-icons/floppy-disk.svg) рядом с кнопкой **Выполнить**.
1. В окне **Сохранение запроса**:
   1. Выберите соединение с базой данной, к которой осуществляется запрос.
   1. Укажите **Название** — произвольное имя запроса, под которым он будет отображаться в списке сохраненных запросов.
   1. Для того чтобы сохраненный запрос мог использоваться в качестве шаблона в списке-подсказке, выберите опцию **Добавить подсказку** и укажите **Текст подсказки**, содержащий `userTemplate_`.
   1. Проверьте или отредактируйте SQL-запрос.

      {% note tip %}

      Если добавляете подсказку и указываете имя шаблона, то в запросе можно указать аргументы, которые будут подсвечиваться при выборе этого шаблона, например: `SELECT $1 FROM employees LIMIT $2`.

      {% endnote %}

   1. Нажмите **Сохранить**.

После сохранения запроса он отобразится в окне **Сохранённые запросы** (![image](../../_assets/console-icons/floppy-disk.svg)), а если вы добавили подсказку, то он будет показываться как шаблон вместе с [готовыми шаблонами](#use-templates) {{ websql-full-name }}.

Запросы сохраняются для выбранной [организации](../../organization/concepts/manage-services.md) {{ yandex-cloud }} и текущей сессии браузера.

## Использовать шаблоны {#use-templates}

Для применения шаблонов:

1. Начните печатать `template` в поле запроса.
   В списке-подсказке вы увидите сохраненные шаблоны `userTemplate_*` и заготовленные шаблоны:

    * `template_CREATE`
    * `template_DELETE`
    * `template_DROP_TABLE`
    * `template_INSERT`
    * `template_SELECT`
    * `template_UPDATE`

1. Выберите шаблон из списка-подсказки.
1. Дополните шаблон релевантными параметрами. Используйте клавишу `TAB`, чтобы переключаться между дополняемыми частями шаблона.
1. Нажмите кнопку **Выполнить**.
