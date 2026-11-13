---
title: "Карта канала DevOps Brain"
description: "Навигация по авторским статьям, практическим разборам и обзорам инструментов из Telegram-канала DevOps Brain."
layout: "channel-map"
lastmod: 2026-11-13T12:00:00+03:00
toc: true
---

В Telegram-ленте уже больше двух лет копятся длинные разборы, серии статей и обзоры инструментов. Искать нужный материал по истории сообщений неудобно, поэтому я собрал здесь карту публикаций канала за период с апреля 2024 года по ноябрь 2026 года.

Это не полный архив: короткие новости, анонсы, мемы и быстро устаревающие заметки сюда не вошли. Все ссылки на этой странице ведут непосредственно на публикации в Telegram-канале.

## Kafka: от первого сообщения до production

Серия идёт от базовой архитектуры к эксплуатации Consumer. Лучше читать по порядку: каждая следующая часть использует механизмы и пример интернет-магазина из предыдущих.

- [Архитектура и базовые принципы — часть 1](https://t.me/devopsbrain/243)
- [Partitions, Consumer Groups и порядок сообщений — часть 2](https://t.me/devopsbrain/244)
- [Обзор полной серии из девяти частей](https://t.me/devopsbrain/251)

## Kubernetes и Infrastructure as Code

- **Лучшие практики конфигурирования Kubernetes:** [часть 1 — база](https://t.me/devopsbrain/182), [часть 2 — сервисы, метки, конфиги и лимиты](https://t.me/devopsbrain/183) и [часть 3 — безопасность, логи и graceful shutdown](https://t.me/devopsbrain/184).
- **Самоподписные SSL-сертификаты в локальном Kubernetes:** [часть 1](https://t.me/devopsbrain/134) и [часть 2](https://t.me/devopsbrain/135).
- [Ищем эксплойты с помощью Kubescape и Metasploit](https://t.me/devopsbrain/136)
- [Локальная песочница Kubernetes и Terraform](https://t.me/devopsbrain/204)
- [Контейнер не равен Docker: где проходит граница понятия](https://t.me/devopsbrain/237)
- [Kubernetes Resource Recommendations: знакомство с Robusta KRR](https://t.me/devopsbrain/8)

## Linux, диагностика и производительность

- [Скрипт для быстрой диагностики Linux](https://t.me/devopsbrain/187)
- [Как работает OOM Killer и почему он выбирает конкретный процесс](https://t.me/devopsbrain/202)
- **Dive in performance tools:** [Sysdig](https://t.me/devopsbrain/95), [память в `top`](https://t.me/devopsbrain/104), [CPU](https://t.me/devopsbrain/105), [таблица процессов](https://t.me/devopsbrain/106), [практические выводы](https://t.me/devopsbrain/107), [bmon](https://t.me/devopsbrain/123) и [bandwhich](https://t.me/devopsbrain/129).
- [Утилиты для параллельной работы с множеством серверов](https://t.me/devopsbrain/181)
- [Как настроить `htop` под себя](https://t.me/devopsbrain/165)

## Сети

- **Практика в GNS3:** [установка и настройка под macOS](https://t.me/devopsbrain/193), [первая сеть](https://t.me/devopsbrain/194) и [Cisco с VLAN](https://t.me/devopsbrain/201).
- [Как объединить устройства в приватную сеть через ZeroTier](https://t.me/devopsbrain/216)
- [Как прокачать сеть между разными ЦОД](https://t.me/devopsbrain/162)
- [Эмуляция задержек, потерь и других сетевых проблем через `tc netem`](https://t.me/devopsbrain/163)
- [Consistent Hashing: теория и интерактивный симулятор](https://t.me/devopsbrain/140)

## Мониторинг, SRE и эксплуатация

- [Как `evaluation_interval` и `for` влияют на алерты Prometheus](https://t.me/devopsbrain/138)
- **SLA, SLO и SLI простыми словами:** [часть 1](https://t.me/devopsbrain/177) и [часть 2](https://t.me/devopsbrain/178).
- [Почему графики в Grafana меняются на разных интервалах](https://t.me/devopsbrain/238)
- [Знакомство с нагрузочным тестированием в Grafana k6](https://t.me/devopsbrain/84)
- [Keep: единая точка для алертов из разных систем](https://t.me/devopsbrain/86)
- [Чеклист по инфраструктуре перед длинными праздниками](https://t.me/devopsbrain/185)

## Git, CI/CD и безопасность разработки

- [Как исправлять ошибки в Git с помощью `fixup` и `autosquash`](https://t.me/devopsbrain/133)
- [Как обнаруживать утечки секретов в Git](https://t.me/devopsbrain/122)
- **Динамические матрицы в GitHub Actions:** [часть 1](https://t.me/devopsbrain/169) и [часть 2](https://t.me/devopsbrain/170).
- **Как бесплатно разместить сайт, блог, CV или Wiki:** [часть 1](https://t.me/devopsbrain/141) и [часть 2](https://t.me/devopsbrain/143).
- [Как запустить публичный сайт на телефоне](https://t.me/devopsbrain/124)
- [Как удалить уже смерженные локальные ветки в Git](https://t.me/devopsbrain/250)
- [Как я научил TeamCity говорить с ИИ через MCP](https://t.me/devopsbrain/167)

## Полезные CLI- и TUI-инструменты

- [`git-igitt`: история Git с читаемым графом веток](https://t.me/devopsbrain/190)
- [`dive`: разбираем Docker-образ по слоям](https://t.me/devopsbrain/191)
- [`ncdu`: ищем, куда исчезло место на диске](https://t.me/devopsbrain/192)
- [`posting`: HTTP-клиент в терминале](https://t.me/devopsbrain/195)
- [`witr`: выясняем, почему процесс запущен и кто им управляет](https://t.me/devopsbrain/196)
- [`cli-stash`: сохраняем сложные команды и быстро вставляем их в терминал](https://t.me/devopsbrain/198)
- [`snitch`: смотрим сетевые соединения и связанные процессы](https://t.me/devopsbrain/209)
- [`termshark`: анализируем трафик и PCAP-файлы в терминале](https://t.me/devopsbrain/217)
- [`syswatch`: наблюдаем за CPU, памятью, диском и сетью в одной сессии](https://t.me/devopsbrain/239)
- [Excalidraw: как рисовать технические схемы без боли](https://t.me/devopsbrain/73)
- [Oh My Zsh: настраиваем удобную командную строку](https://t.me/devopsbrain/92)
- [SiYuan: система для управления личными знаниями](https://t.me/devopsbrain/109)
- [ntfy: отправляем уведомления на телефон через HTTP API](https://t.me/devopsbrain/118)
- [Macpine: запускаем лёгкие Linux VM на macOS](https://t.me/devopsbrain/66)
- [Docmost: open source альтернатива Notion](https://t.me/devopsbrain/58)
- [Kubetools: каталог инструментов для Kubernetes](https://t.me/devopsbrain/51)
- [NeoHtop: современная альтернатива `htop`](https://t.me/devopsbrain/80)
- [Tabby: кроссплатформенный терминал](https://t.me/devopsbrain/94)

## Go и разработка инфраструктурных инструментов

- [Expr для Go: динамические правила вместо цепочек `if`](https://t.me/devopsbrain/253)
- [Zerolog: организуем структурированные логи в Go](https://t.me/devopsbrain/57)
- [Net-peek: кто потребляет трафик на сервере](https://t.me/devopsbrain/248)

## Карьера, процессы и инженерная культура

- [Вредные советы начинающим специалистам в IT](https://t.me/devopsbrain/108)
- [Зачем команде писать постмортемы](https://t.me/devopsbrain/74)
- [Как вернуться в рабочий ритм после длинных праздников](https://t.me/devopsbrain/189)
- [Почему фундаментальные знания всё ещё важны в эпоху ИИ](https://t.me/devopsbrain/218)

## ИИ и размышления об индустрии

- [Кладбище AI-экспериментов: что остаётся, когда гаснет хайп](https://t.me/devopsbrain/240)
- [Иллюзия приватности: как мы доверились ИИ без оглядки](https://t.me/devopsbrain/147)
- [Open source свернул не туда?](https://t.me/devopsbrain/81)
- **Как OS/2 проиграла Windows:** [часть 1](https://t.me/devopsbrain/149) и [часть 2](https://t.me/devopsbrain/155).
- [AI больше не стыдно?](https://t.me/devopsbrain/247)
- [Как собрать личного AI-ассистента на базе Telegram и n8n](https://t.me/devopsbrain/213)

## Проекты и эксперименты

- [GitHub Unhappy Approve: расширение для Chrome](https://t.me/devopsbrain/68)
- [Бот для предложенных новостей в Telegram](https://t.me/devopsbrain/63)
- [iKanban: симулятор закрытых задач](https://t.me/devopsbrain/207)

Карта будет пополняться вместе с каналом. Новые заметки, короткие находки и обсуждения появляются в [Telegram-канале DevOps Brain](https://t.me/devopsbrain).
