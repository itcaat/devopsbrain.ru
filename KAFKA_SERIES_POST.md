# Kafka: от первого сообщения до production

Наконец-то закончил писать серию статей про Kafka. В ней мне хотелось не просто объяснить термины, но и связать их в понятную картину.

Вместе мы пройдем путь на примере классического интернет-магазина. Сначала отправим событие о заказе, потом разберём порядок сообщений, репликацию и производительность. А дальше посмотрим, что будет происходить в случае отказа тех или иных частей нашей архитектуры.

В серии есть все необходимые основы основы — Topic, Partition, Offset, Consumer Group, - и практические решения: выбор ключей, контракты событий, Outbox, идемпотентность, retry и DLQ.

Если вы только знакомитесь с Kafka или уже используете её, но отдельные механизмы пока не складываются в общую картину, приглашаю почитать. И не стесняйтесь оставлять свой фидбек, если где-то остались вопросы после прочтения. 

1. [Kafka: архитектура и базовые принципы — Часть 1](https://devopsbrain.ru/posts/2026-08-06-kafka-from-zero-to-hero-part-1/)
2. [Kafka: как масштабируются Partitions, Consumer Groups и порядок сообщений — Часть 2](https://devopsbrain.ru/posts/2026-08-06-kafka-from-zero-to-hero-part-2/)
3. [Kafka: Record, Offset и Append-Only Log — Часть 3](https://devopsbrain.ru/posts/2026-08-06-kafka-from-zero-to-hero-part-3/)
4. [Kafka: репликация, Leader, Follower и ISR — Часть 4](https://devopsbrain.ru/posts/2026-08-06-kafka-from-zero-to-hero-part-4/)
5. [Kafka: что делает её производительной — Часть 5](https://devopsbrain.ru/posts/2026-08-06-kafka-from-zero-to-hero-part-5/)
6. [Kafka: события, команды, Topics и Keys — Часть 6](https://devopsbrain.ru/posts/2026-08-06-kafka-from-zero-to-hero-part-6/)
7. [Kafka: Retention, Compaction и контракты событий — Часть 7](https://devopsbrain.ru/posts/2026-08-06-kafka-from-zero-to-hero-part-7/)
8. [Kafka: гарантии доставки, Outbox и идемпотентность — Часть 8](https://devopsbrain.ru/posts/2026-08-06-kafka-from-zero-to-hero-part-8/)
9. [Kafka: Retry, DLQ и эксплуатация Consumer — Часть 9](https://devopsbrain.ru/posts/2026-08-06-kafka-from-zero-to-hero-part-9/)
