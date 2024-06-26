# Создание интернет-магазина на «1С-Битрикс: Управление сайтом»


[«1С-Битрикс: Управление сайтом»](https://ru.wikipedia.org/wiki/1С-Битрикс:_Управление_сайтом) — это система управления контентом (CMS), с помощью которой вы можете создать интернет-магазин, корпоративный сайт или новостной портал и управлять его структурой и содержимым.

Из этого руководства вы узнаете, как развернуть и настроить интернет-магазин на платформе «1С-Битрикс». В процессе настройки вы создадите [виртуальную машину](../../compute/concepts/vm.md) в {{ yandex-cloud }}, развернете на ней «1С-Битрикс» и запустите необходимые сервисы. В качестве базы данных вы будете использовать отказоустойчивый [кластер {{ mmy-full-name }}](../../managed-mysql/concepts/index.md).

Вы можете создать инфраструктуру для интернет-магазина на «1С-Битрикс: Управление сайтом» с помощью одного из инструментов:
* [Консоль управления](../../tutorials/internet-store/bitrix-shop/console.md) — используйте этот способ, чтобы пошагово создать инфраструктуру в консоли управления {{ yandex-cloud }}.
* [{{ TF }}](../../tutorials/internet-store/bitrix-shop/terraform.md) — используйте этот способ, чтобы упростить создание ресурсов и управление ими, используя подход «инфраструктура как код» (IaC). Скачайте пример конфигурации {{ TF }} с репозитория GitHub, а затем разверните инфраструктуру с помощью [{{ TF }}-провайдера {{ yandex-cloud }}]({{ tf-docs-link }}).