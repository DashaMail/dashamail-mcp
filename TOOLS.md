# Инструменты

Всего 75. Заголовки двуязычные, как в самом сервере.

## Аккаунт, отправители, домены

| Инструмент | Что делает | Tool |
|---|---|---|
| `account_get` | Баланс и лимиты аккаунта | Account balance and limits |
| `senders_list` | Подтверждённые адреса отправителей | Verified sender addresses |
| `senders_add` ⚠️ | Добавить адрес отправителя | Add a sender address |
| `domains_list` | Домены отправки и их DNS-статус | Sending domains and their DNS status |
| `domains_add` | Добавить домен отправки | Add a sending domain |
| `domains_check` | Перепроверить DNS доменов | Re-check domain DNS |

## Адресные базы и подписчики

| Инструмент | Что делает | Tool |
|---|---|---|
| `lists_list` | Адресные базы | Subscriber lists |
| `lists_get` | Одна адресная база | A single subscriber list |
| `lists_create` | Создать адресную базу | Create a subscriber list |
| `lists_update` | Изменить адресную базу | Update a subscriber list |
| `fields_add` | Добавить дополнительное поле базы | Add an additional list field |
| `fields_update` | Изменить дополнительное поле базы | Update an additional list field |
| `lists_unsubscribed` | Отписавшиеся подписчики | Unsubscribed subscribers |
| `lists_complaints` | Пожаловавшиеся на спам | Spam complainers |
| `members_search` | Подписчики базы | Subscribers of a list |
| `members_get` | Один подписчик | A single subscriber |
| `members_add` | Добавить подписчика | Add a subscriber |
| `members_add_batch` | Добавить подписчиков пачкой | Add subscribers in a batch |
| `members_update` | Изменить подписчика | Update a subscriber |
| `members_unsubscribe` | Отписать подписчика | Unsubscribe a subscriber |
| `members_move` | Перенести подписчика в другую базу | Move a subscriber to another list |
| `members_copy` | Скопировать подписчика в другую базу | Copy a subscriber to another list |
| `members_activity` | История событий подписчика | Subscriber event history |
| `members_status` | Текущий статус адреса | Current status of an address |
| `members_check_email` | Проверить адрес перед подпиской | Check an address before subscribing |
| `imports_start` | Запустить импорт подписчиков из файла по URL | Start a subscriber import from a file URL |
| `imports_status` | Результат последнего импорта | Result of the last import |
| `imports_history` | История импортов | Import history |

## Рассылки и шаблоны

| Инструмент | Что делает | Tool |
|---|---|---|
| `campaigns_list` | Рассылки | Campaigns |
| `campaigns_get` | Одна рассылка | A single campaign |
| `campaigns_create` | Создать черновик рассылки | Create a campaign draft |
| `campaigns_update` | Изменить черновик рассылки | Update a campaign draft |
| `campaigns_schedule` ⚠️ | Запланировать отправку рассылки | Schedule a campaign |
| `campaigns_send_now` ⚠️ | Отправить рассылку сейчас | Send a campaign now |
| `campaigns_pause` | Приостановить отправку | Pause sending |
| `campaigns_resume` | Возобновить отправку | Resume sending |
| `campaigns_unschedule` | Снять с расписания | Remove from schedule |
| `campaigns_resend_unopened` ⚠️ | Переотправить неоткрывшим | Resend to non-openers |
| `campaigns_copy` | Скопировать рассылку | Copy a campaign |
| `folders_list` | Папки рассылок | Campaign folders |
| `campaigns_move_to_folder` | Переместить рассылку в папку | Move a campaign to a folder |
| `templates_list` | Сохранённые шаблоны аккаунта | Saved account templates |
| `templates_gallery` | Готовые шаблоны из галереи | Ready-made templates from the gallery |
| `templates_create` | Сохранить HTML-шаблон | Save an HTML template |

## Автоматизации

| Инструмент | Что делает | Tool |
|---|---|---|
| `automations_list` | Автоматизации | Automations |
| `automations_trigger` ⚠️ | Запустить автоматизацию для адреса | Trigger an automation for an address |

## Отчёты

| Инструмент | Что делает | Tool |
|---|---|---|
| `reports_summary` | Сводка по рассылке или по аккаунту | Summary for a campaign or the account |
| `reports_recipients` | Получатели по событию | Recipients by event |
| `reports_events` | Лента событий рассылки | Campaign event feed |
| `reports_links` | Клики по ссылкам | Link clicks |
| `reports_link_clickers` | Кто кликнул по ссылке | Who clicked a link |
| `reports_bounces` | Возвраты по SMTP-кодам | Bounces by SMTP code |
| `reports_domains` | Статистика по почтовым доменам получателей | Statistics by recipient email domain |
| `reports_geo` | География открытий | Geography of opens |
| `reports_clients` | Устройства, браузеры и почтовые клиенты | Devices, browsers and email clients |

## Транзакционные письма

| Инструмент | Что делает | Tool |
|---|---|---|
| `transactional_send` ⚠️ | Отправить транзакционное письмо | Send a transactional email |
| `transactional_get` | Статус транзакционного письма | Status of a transactional email |
| `transactional_log` | Журнал транзакционных писем | Transactional email log |
| `transactional_stats` | Статистика транзакционных писем по периодам | Transactional email statistics by period |

## Вебхуки

| Инструмент | Что делает | Tool |
|---|---|---|
| `webhooks_list` | Вебхуки массовых рассылок | Campaign webhooks |
| `webhooks_set` | Задать URL вебхука массовых рассылок | Set a campaign webhook URL |
| `webhooks_delete` ⚠️ | Удалить вебхук массовых рассылок | Delete a campaign webhook |
| `webhooks_list_transactional` | Вебхуки транзакционных писем | Transactional email webhooks |
| `webhooks_set_transactional` | Задать URL вебхука транзакционных писем | Set a transactional email webhook URL |
| `webhooks_delete_transactional` ⚠️ | Удалить вебхук транзакционных писем | Delete a transactional email webhook |

## Роутер входящей почты

| Инструмент | Что делает | Tool |
|---|---|---|
| `router_routes_list` | Маршруты входящей почты | Inbound mail routes |
| `router_messages_list` | Входящие письма Роутера | Inbound Router messages |
| `router_messages_get` | Одно входящее письмо Роутера | A single inbound Router message |
| `router_deliveries_list` | Доставки Роутера | Router deliveries |

⚠️ — инструмент помечен `destructiveHint`: клиент спрашивает подтверждение.

Шесть составных инструментов (`whoami`, `get_dashboard_link`, `campaigns_delete`, `members_find`, `lists_stats`, `reports_compare`) считают сводки на сервере и в этот список не входят.
