# Устранение ошибки ERR.DS_API.REQUEST_TIMEOUT


## Описание проблемы {#issue-description}

* Построение чарта завершается с ошибкой `ERR.DS_API.REQUEST_TIMEOUT` после длительного ожидания.

## Решение {#issue-resolution}

DataLens не имеет настраиваемых параметров, так что повысить порог не получится. Попробуйте разбить наиболее затратные задачи на части либо используйте фильтрацию данных для уменьшения их количества.

## Если проблема осталась {#if-issue-still-persists}

Если вышеописанные действия не помогли решить проблему, [создайте запрос в техническую поддержку](https://console.cloud.yandex.ru/support?section=contact).
При создании запроса укажите:

1. Ссылку на проблемный объект в DataLens (чарт или дашборд);
2. Request ID проблемного запроса (отображается на странице с ошибкой).