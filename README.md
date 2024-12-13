# Тесты для лабораторных работ курсов по сетевым технологиям ИРИТ-РтФ УрФУ
## Структура
- [labs](labs) - директория с тестами для лабораторных работ
- [labs/Autumn](labs/Autumn) - "Построение масштабируемых корпоративных сетей"
- [labs/Spring](labs/Spring) - "Компьютерные сети (Cisco/Juniper)"
- [libs](libs) - директория с общими функциями для тестирования

## Команда загрузки тестов на сервер PNET

```
# check
rsync -avun --chown www-data:www-data --exclude .git --exclude "__*" --exclude "trash" . root@<pnet-address>:/opt/unetlab

# upload
rsync -avu --chown www-data:www-data --exclude .git --exclude "__*" --exclude "trash" . root@<pnet-address>:/opt/unetlab
```

## Дополнительные настройки Lab

Во всех лабораторках, где используется прямой доступ в общую сеть с лабораторных стендов (например, [labs/Autumn/5/NAT.unl](labs/Autumn/5/NAT.unl)) необходимо в зависимости от стенда менять дефолтные MAC-адреса устройств, которые смотрят в сеть

```
mac-address aabb.cc00.<PNET-N>10
```