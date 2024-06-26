# Интеграция в интерфейсе {{ forms-name }}

Чтобы создать форму в сервисе {{ forms-full-name }} и подключить ее к очереди, выполните шаги:

## Шаг 1. Создайте и настройте форму {#create-form}

1. Перейдите в сервис [{{ forms-full-name }}]({{ link-forms }}). Если сервис не подключен, обратитесь к администратору вашей организации.

1. [Создайте](../../forms/new-form) новую форму.

1. Настройте форму так, чтобы собрать данные, которые необходимы для создания задачи.

1. Настройте [интеграцию с {{ tracker-name }}](../../forms/create-task):

    1. Укажите очередь и другие параметры задачи.

    1. В поле **Описание задачи** добавьте ответы на вопросы формы.

    1. Чтобы сохранить в параметрах задачи ответ на определенный вопрос формы, в настройках интеграции добавьте поле задачи, нажмите **Переменные** → **Ответ на вопрос** и выберите вопрос. 
    
      Если в параметрах задачи нет нужного вам поля, вы можете его [создать](../user/create-param.md).

    1. Сохраните параметры интеграции.
    Форма будет отправлять в {{ tracker-name }} ответы пользователя, а {{ tracker-name }} создаст на их основе задачу.



1. Настройте [доступ к заполнению формы](../../forms/restrictions.md#restrictions__sec_access).
    По умолчанию форму могут заполнять все пользователи. Вы можете разрешить заполнение формы только сотрудникам вашей организации.


1. [Опубликуйте](../../forms/publish.md) форму. Форма будет доступна по ссылке, указанной в поле **Ссылка**.

## Шаг 2. Подключите форму к очереди {#link-form}

1. Перейдите в [{{ tracker-name }}]({{ link-tracker }}).

1. {% include [go to settings](../../_includes/tracker/transition-page.md) %} 

1. В правом верхнем углу нажмите ![](../../_assets/tracker/svg/settings.svg) **Настройки очереди**.

1. Перейдите на вкладку **Интеграции**.

1. В блоке **Формы** нажмите **Добавить форму** → ![](../../_assets/tracker/svg/link.svg) **Подключить существующую**.

   {% note tip %}
   
   Вы также можете [создать форму](../user/forms-template.md) во встроенном конструкторе {{ tracker-name }}.
   
   {% endnote %}

1. Вставьте ссылку на форму.

1. Добавьте название и описание формы. Они будут видны в окне выбора формы при создании задачи, а также в списке форм, подключенных к очереди.

1. Нажмите кнопку **Добавить форму**.

#### См. также: {#see-also}

* [Документация {{ forms-full-name }}](../../forms).
* [{#T}](attach-form.md).
* [{#T}](../user/forms-template.md).

