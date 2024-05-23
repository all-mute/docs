# Секрет

{% include notitle [preview](../../_includes/note-preview.md) %}

Секрет состоит из набора версий, в которых хранятся защищенные данные подключения. Версия содержит наборы _ключей_ и _значений_. Ключ — это несекретное название для значения, по которому его можно идентифицировать. Значение — это секретные данные о подключении.

К секретам можно настраивать доступ, используя сервис [{{ iam-full-name }}](../../iam/index.yaml). Доступные роли для разных сценариев использования описаны в разделе [{#T}](../security/index.md).

Секреты хранятся в сервисе [{{ lockbox-full-name }}](../../lockbox/index.yaml). Чтобы посмотреть, какие секреты хранят информацию о подключениях, выберите в вашем каталоге в списке сервисов **{{ ui-key.yacloud.iam.folder.dashboard.label_lockbox }}**. На странице **{{ ui-key.yacloud.lockbox.label_section-secrets }}** будут перечислены секреты, имена которых совпадают с [идентификаторами подключений](../operations/update-connection.md#list-connections).  

К версиям секрета можно настроить доступ дополнительно к доступу к самому секрету. Для этого нужно назначить роль `{{ roles-lockbox-admin }}` или `{{ roles-lockbox-payloadviewer }}`. Подробнее об управлении доступом читайте в разделе [Управление доступом {{ lockbox-full-name }} - Какие роли мне необходимы](../security/index.md#choosing-roles).