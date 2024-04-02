# Тесты для лабораторных работ курсов по сетевым технологиям ИРИТ-РтФ УрФУ
## Структура
- [labs](labs) - директория с тестами для лабораторных работ
- [labs/Autumn](labs/Autumn) - "Построение масштабируемых корпоративных сетей"
- [labs/Spring](labs/Spring) - "Компьютерные сети (Cisco/Juniper)"
- [libs](libs) - директория с общими функциями для тестирования

## Команда загрузки тестов на сервер PNET

```
rsync -avu --chown www-data:www-data --exclude .git . root@<pnet-address>:/opt/unetlab
```