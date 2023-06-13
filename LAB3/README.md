# Развертывание системы мониторинга ELK Stack

## Цель работы

1.  Освоить базовые подходы централизованного сбора и накопления информации
2.  Освоить современные инструменты развертывания контейнирозованных приложений
3.  Закрепить знания о современных сетевых протоколах прикладного уровня

## Ход выполнения практической работы

### Задание 1. Развернуть систему мониторинга на базе ElasticSearch

1.  Настройка

Для работы ElasticSearch требуется увеличить размер виртуальной памяти системы:

``` ()
sudo sysctl -w vm.max_map_count=262144
```

Далее следуем инструкции по ссылке:

https://www.elastic.co/guide/en/elasticsearch/reference/current/docker.html

2.  Запуск образов командой

``` ()
docker-compose up -d
```

3.  Переходим на `localhost:5061` и авторизируемся

![All text](https://github.com/anyam/saznd/blob/main/LAB3/авторизация.png)

4.  Проверка установленных средств для сбора информации

![All text](https://github.com/MoonFlower18/threat_hunting/blob/main/Prak_3/%D0%A1%D0%BA%D1%80%D0%B8%D0%BD%D1%88%D0%BE%D1%82%D1%8B/3.png)

5.  Новый DataView для filebeat

![Att text](https://github.com/anyam/saznd/blob/main/LAB3/file%20beat.png)

6.  Новый DataView для packetbeat

![All text](https://github.com/anyam/saznd/blob/main/LAB3/packetbeat.png)

## Оценка результата

Была развёрнута система ElasticSearch и настроена система сбора трафика и лог-файлов.

## Вывод

В результате работы была освоена система контейнеризации приложений Docker, работа с Docker-compose и освоена система централизованного сбора и накопления информации ElasticSearch.
