Для создания ревизии необходимо сделать [реестр](../../container-registry/concepts/registry.md) или [репозиторий](../../container-registry/concepts/repository.md), в которых находится Docker-образ, [публичными](../../container-registry/qa/index.md#public-registry) или указать в настройках ревизии [сервисный аккаунт](../../iam/concepts/users/service-accounts.md), у которого [есть права](../../iam/operations/sa/assign-role-for-sa.md) на скачивание Docker-образа. Например, роль `container-registry.images.puller` на каталог или реестр, в которых находится Docker-образ.