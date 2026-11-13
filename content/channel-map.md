---
title: "Карта канала DevOps Brain"
description: "Навигация по авторским статьям, практическим разборам и обзорам инструментов из Telegram-канала DevOps Brain."
layout: "channel-map"
lastmod: 2026-11-13T12:00:00+03:00
toc: true
---

В Telegram-ленте уже больше двух лет копятся длинные разборы, серии статей и обзоры инструментов. Искать нужный материал по истории сообщений неудобно, поэтому я собрал здесь карту публикаций канала за период с апреля 2024 года по ноябрь 2026 года.

Это не полный архив: короткие новости, анонсы, мемы и быстро устаревающие заметки сюда не вошли. Если материал вырос в полноценную статью, ссылка ведёт на сайт. Для самостоятельных заметок и небольших циклов сохранена ссылка на исходный пост в Telegram.

## Kafka: от первого сообщения до production

Серия идёт от базовой архитектуры к эксплуатации Consumer. Лучше читать по порядку: каждая следующая часть использует механизмы и пример интернет-магазина из предыдущих.

1. [Архитектура и базовые принципы](/posts/2026-08-06-kafka-from-zero-to-hero-part-1/)
2. [Как масштабируются Partitions, Consumer Groups и порядок сообщений](/posts/2026-08-06-kafka-from-zero-to-hero-part-2/)
3. [Record, Offset и Append-Only Log](/posts/2026-08-06-kafka-from-zero-to-hero-part-3/)
4. [Репликация, Leader, Follower и ISR](/posts/2026-08-06-kafka-from-zero-to-hero-part-4/)
5. [Что делает Kafka производительной](/posts/2026-08-06-kafka-from-zero-to-hero-part-5/)
6. [События, команды, Topics и Keys](/posts/2026-08-06-kafka-from-zero-to-hero-part-6/)
7. [Retention, Compaction и контракты событий](/posts/2026-08-06-kafka-from-zero-to-hero-part-7/)
8. [Гарантии доставки, Outbox и идемпотентность](/posts/2026-08-06-kafka-from-zero-to-hero-part-8/)
9. [Retry, DLQ и эксплуатация Consumer](/posts/2026-08-06-kafka-from-zero-to-hero-part-9/)

## Kubernetes и Infrastructure as Code

- **Лучшие практики конфигурирования Kubernetes:** [часть 1 — база](/posts/2025-12-10-kubernetes-best-practices-2025-chast-1/), [часть 2 — сервисы, метки, конфиги и лимиты](/posts/2025-12-10-kubernetes-best-practices-2025-chast-2/) и [часть 3 — безопасность, логи и graceful shutdown](/posts/2025-12-10-kubernetes-best-practices-2025-chast-3/).
- [Настройка валидных самоподписных SSL-сертификатов в локальном Kubernetes](/posts/2025-02-14-valid-ssl-certs-in-local-k8s/)
- [Ищем эксплойты с помощью Kubescape и Metasploit](/posts/2025-02-16-metasploit-kubescape/)
- [Локальная песочница Kubernetes и Terraform](/posts/2025-02-23-terraform-kubernetes-desktop-startkit/)
- [Контейнер не равен Docker: где проходит граница понятия](https://t.me/devopsbrain/237)
- [Kubernetes Resource Recommendations: знакомство с Robusta KRR](https://t.me/devopsbrain/8)

## Linux, диагностика и производительность

- [CPU Usage и Load Average: что на самом деле показывает система](/posts/2025-08-10-about-load-avarage-and-cpu-usage/)
- [Bash-скрипт для быстрой диагностики Linux](/posts/2025-12-26-bash-script-dlya-diagnostiki-linux-sistemy/)
- [Как работает OOM Killer и почему он выбирает конкретный процесс](https://t.me/devopsbrain/202)
- **Dive in performance tools:** [Sysdig](https://t.me/devopsbrain/95), [память в `top`](https://t.me/devopsbrain/104), [CPU](https://t.me/devopsbrain/105), [таблица процессов](https://t.me/devopsbrain/106), [практические выводы](https://t.me/devopsbrain/107), [bmon](https://t.me/devopsbrain/123) и [bandwhich](https://t.me/devopsbrain/129).
- [Утилиты для параллельной работы с множеством серверов](https://t.me/devopsbrain/181)
- [Как настроить `htop` под себя](https://t.me/devopsbrain/165)

## Сети

- **Практика в GNS3:** [установка и настройка под macOS](/posts/2026-01-07-modelirovanie-seti-na-macos-ustanovka-i-nastroyka/), [первая сеть](/posts/2026-01-20-simuliruem-seti-v-gns3-delaem-pervuyu-set/) и [Cisco с VLAN](/posts/2026-02-04-simuliruem-seti-v-gns-cisco-vlan/).
- [Reverse Proxy, Load Balancer и API Gateway: в чём разница](/posts/2026-02-25-reverse-proxy-vs-load-balancer-vs-api-gateway/)
- [Как объединить устройства в приватную сеть через ZeroTier](/posts/2026-03-05-sozdanie-privatnoy-seti-zerotier/)
- [Как прокачать сеть между разными ЦОД](/posts/2025-09-21-bottleneck-bandwidth-and-round-trip-time/)
- [Эмуляция задержек, потерь и других сетевых проблем через `tc netem`](https://t.me/devopsbrain/163)
- [Consistent Hashing: теория и интерактивный симулятор](/posts/2025-04-29-ring-hashing/)

## Мониторинг, SRE и эксплуатация

- [Как `evaluation_interval` и `for` влияют на алерты Prometheus](/posts/2025-02-26-evaluation_interval-and-for-in-prometheus/)
- **SLA, SLO и SLI простыми словами:** [часть 1](https://t.me/devopsbrain/177) и [часть 2](https://t.me/devopsbrain/178).
- [Почему графики в Grafana меняются на разных интервалах](https://t.me/devopsbrain/238)
- [Знакомство с нагрузочным тестированием в Grafana k6](/posts/2024-11-18-nagruzochnoe-testirovanie-s-pomoshyu-grafana-k6/)
- [Keep: единая точка для алертов из разных систем](/posts/2025-01-10-mini-obzor-keep/)
- [Чеклист по инфраструктуре перед длинными праздниками](/posts/2025-12-25-checklist-dlya-admina-devops-sre-pered-prazdnikami/)

## Git, CI/CD и безопасность разработки

- [Как исправлять ошибки в Git с помощью `fixup` и `autosquash`](/posts/2025-02-10-kak-ispravit-oshibki-v-git/)
- [Как обнаруживать утечки секретов в Git](/posts/2025-01-28-boremsya-s-utechkoy-sekretov-v-git/)
- **Динамические матрицы в GitHub Actions:** [часть 1](https://t.me/devopsbrain/169) и [часть 2](https://t.me/devopsbrain/170).
- [Как бесплатно разместить сайт, блог, CV или Wiki](/posts/2025-05-01-besplatny-site/)
- [Как запустить публичный сайт на телефоне](/posts/2025-02-05-kak-zapustit-site-na-telefone/)
- [Как удалить уже смерженные локальные ветки в Git](https://t.me/devopsbrain/250)
- [Как я научил TeamCity говорить с ИИ через MCP](/posts/2025-06-26-teamcity-mcp-server/)

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
- [Excalidraw: как рисовать технические схемы без боли](/posts/2024-10-17-kak-risovat-schemi-bez-boli/)
- [Oh My Zsh: настраиваем удобную командную строку](/posts/2025-01-10-kak-nastroit-oh-my-zsh/)
- [SiYuan: система для управления личными знаниями](/posts/2025-01-23-obzor-siyuan/)
- [ntfy: отправляем уведомления на телефон через HTTP API](/posts/2025-01-25-obzor-ntfy/)
- [Macpine: запускаем лёгкие Linux VM на macOS](/posts/2024-08-02-obzor-macpine/)
- [Docmost: open source альтернатива Notion](https://t.me/devopsbrain/58)
- [Kubetools: каталог инструментов для Kubernetes](https://t.me/devopsbrain/51)
- [NeoHtop: современная альтернатива `htop`](https://t.me/devopsbrain/80)
- [Tabby: кроссплатформенный терминал](https://t.me/devopsbrain/94)

## Go и разработка инфраструктурных инструментов

- [Expr для Go: динамические правила вместо цепочек `if`](/posts/2026-11-03-expr-lang-in-go/)
- [Zerolog: организуем структурированные логи в Go](https://t.me/devopsbrain/57)
- [Net-peek: кто потребляет трафик на сервере](https://t.me/devopsbrain/248)
- [Another Redis Benchmark](/posts/2024-11-21-another-redis-benchmark/)
- [iops-perf: тестируем дисковую подсистему](/posts/2025-01-08-iops-perf/)

## Карьера, процессы и инженерная культура

- [Реальные вопросы для DevOps/SRE-интервью](/posts/2026-03-11-interview-devops-questions-2026/)
- [Вредные советы начинающим специалистам в IT](/posts/2025-01-20-vrednie-soveti-nachinayushim-it-specialistam/)
- [Зачем команде писать постмортемы](/posts/2024-10-18-davayte-vse-pisat-postmortemi/)
- [Как вернуться в рабочий ритм после длинных праздников](https://t.me/devopsbrain/189)
- [Почему фундаментальные знания всё ещё важны в эпоху ИИ](https://t.me/devopsbrain/218)

## ИИ и размышления об индустрии

- [Кладбище AI-экспериментов: что остаётся, когда гаснет хайп](/posts/2026-06-16-kladbishe-ai-experimentov/)
- [Иллюзия приватности: как мы доверились ИИ без оглядки](/posts/2025-05-20-ai-illusion-of-privacity/)
- [Open source свернул не туда?](/posts/2024-11-08-opensource-svernul-ne-tuda/)
- **Как OS/2 проиграла Windows:** [часть 1](https://t.me/devopsbrain/149) и [часть 2](https://t.me/devopsbrain/155).
- [AI больше не стыдно?](https://t.me/devopsbrain/247)
- [Как собрать личного AI-ассистента на базе Telegram и n8n](https://t.me/devopsbrain/213)

## Проекты и эксперименты

- [Все открытые проекты автора](/projects/)
- [Proxmox Service Discovery](/posts/2024-10-22-proxmox-service-disovery/)
- [GitHub Unhappy Approve: расширение для Chrome](/posts/2024-10-11-github-unhappy-approve/)
- [Suggest News Telegram Bot](/posts/2024-07-31-telegram-bot-suggest-news/)
- [Pulkovo Flightboard: табло аэропорта в Minecraft](/posts/2025-03-27-pulkovo-flightboard/)
- [iKanban: симулятор закрытых задач](https://t.me/devopsbrain/207)

Карта будет пополняться вместе с каналом. Новые заметки, короткие находки и обсуждения появляются в [Telegram-канале DevOps Brain](https://t.me/devopsbrain).
