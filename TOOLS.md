# Инструменты

Всего 106: 102 в таблицах ниже и 4 составных.
Заголовки двуязычные, как в самом сервере.

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
| `members_find` | Найти подписчика во всех базах | Find a subscriber across all lists |
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

## Сегменты

| Инструмент | Что делает | Tool |
|---|---|---|
| `segments_list` | Сохранённые сегменты | Saved segments |
| `segments_get` | Один сегмент с условиями | A single segment with its conditions |
| `segments_create` | Сохранить сегмент | Save a segment |
| `segments_update` | Изменить сегмент | Change a segment |
| `segments_delete` ⚠️ | Удалить сегмент | Delete a segment |
| `segments_count` | Размер сегмента | Size of a segment |
| `segments_fields` | Из чего собирать условия отбора | What segment conditions are made of |

## Рассылки и шаблоны

| Инструмент | Что делает | Tool |
|---|---|---|
| `campaigns_list` | Рассылки | Campaigns |
| `campaigns_get` | Одна рассылка | A single campaign |
| `campaigns_create` | Создать черновик рассылки | Create a campaign draft |
| `campaigns_update` | Изменить черновик рассылки | Update a campaign draft |
| `campaigns_copy` | Скопировать рассылку | Copy a campaign |
| `campaigns_test` | Отправить тестовое письмо | Send a test email |
| `campaigns_preview` | Ссылка на просмотр письма | Preview link for the email |
| `campaigns_estimate` | Сколько писем уйдёт | How many emails will go out |
| `campaigns_schedule` ⚠️ | Запланировать отправку рассылки | Schedule a campaign |
| `campaigns_send_now` ⚠️ | Отправить рассылку сейчас | Send a campaign now |
| `campaigns_unschedule` | Снять с расписания | Remove from schedule |
| `campaigns_pause` | Приостановить отправку | Pause sending |
| `campaigns_resume` | Возобновить отправку | Resume sending |
| `campaigns_resend_unopened` ⚠️ | Переотправить неоткрывшим | Resend to non-openers |
| `campaigns_ab_create` | Сделать из черновика A/B-тест | Turn a draft into an A/B test |
| `campaigns_ab_get` | Настройки A/B-теста | A/B test settings |
| `campaigns_ab_update` | Изменить A/B-тест | Change an A/B test |
| `campaigns_ab_delete` | Разобрать A/B-тест | Take an A/B test apart |
| `campaigns_ab_winner` ⚠️ | Выбрать победителя A/B-теста | Pick the winner of an A/B test |
| `campaigns_ab_winner_cancel` | Отменить выбор победителя | Undo the winner choice |
| `folders_list` | Папки рассылок | Campaign folders |
| `campaigns_move_to_folder` | Переместить рассылку в папку | Move a campaign to a folder |
| `templates_saved` | Шаблоны аккаунта | Templates of the account |
| `templates_html` | HTML-шаблоны аккаунта | HTML templates of the account |
| `templates_get` | Один HTML-шаблон | A single HTML template |
| `templates_create` | Сохранить HTML-шаблон | Save an HTML template |
| `templates_update` | Изменить HTML-шаблон | Update an HTML template |

## Автоматизации

| Инструмент | Что делает | Tool |
|---|---|---|
| `automations_list` | Автоматизации | Automations |
| `automations_events` | События запуска автоматизаций | Automation trigger events |
| `automations_create` | Создать автоматизацию | Create an automation |
| `automations_update` | Изменить автоматизацию | Update an automation |
| `automations_delete` ⚠️ | Удалить автоматизацию | Delete an automation |
| `automations_trigger` ⚠️ | Запустить автоматизацию для адреса | Trigger an automation for an address |
| `workflows_list` | Сценарии конструктора | Builder scenarios |

## Отчёты

| Инструмент | Что делает | Tool |
|---|---|---|
| `reports_summary` | Сводка по рассылке или по аккаунту | Summary for a campaign or the account |
| `reports_recipients` | Получатели по событию | Recipients by event |
| `reports_links` | Клики по ссылкам | Link clicks |
| `reports_link_clickers` | Кто кликнул по ссылке | Who clicked a link |
| `reports_bounces` | Возвраты по SMTP-кодам | Bounces by SMTP code |
| `reports_domains` | Статистика по почтовым доменам получателей | Statistics by recipient email domain |
| `reports_geo` | География открытий | Geography of opens |
| `reports_clients` | Устройства, браузеры и почтовые клиенты | Devices, browsers and email clients |
| `reports_events` | Лента событий рассылки | Campaign event feed |
| `reports_timeline` | Динамика рассылки по времени | Campaign timeline |
| `reports_ab` | Результаты A/B-теста | A/B test results |
| `analytics_report` | Отчёт по периодам | Report by periods |

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

## Диалоги: ответы на рассылки

| Инструмент | Что делает | Tool |
|---|---|---|
| `dialogs_list` | Ответы подписчиков на рассылки | Subscriber replies to campaigns |
| `dialogs_get` | Один диалог с контекстом | A single dialog with its context |
| `dialogs_messages` | Переписка диалога | Conversation of a dialog |
| `dialogs_reply` ⚠️ | Ответить подписчику | Reply to the subscriber |
| `dialogs_close` | Закрыть диалог | Close a dialog |
| `dialogs_unread_count` | Сколько непрочитанных ответов | How many unread replies |

## Роутер входящей почты

| Инструмент | Что делает | Tool |
|---|---|---|
| `router_routes_list` | Маршруты входящей почты | Inbound mail routes |
| `router_messages_list` | Входящие письма Роутера | Inbound Router messages |
| `router_messages_get` | Одно входящее письмо Роутера | A single inbound Router message |
| `router_deliveries_list` | Доставки Роутера | Router deliveries |

⚠️ — необратимо: уходят письма либо удаляются данные. Клиенты по этой
пометке сами спрашивают подтверждение.

Составные инструменты собирают сводки из нескольких вызовов и в таблицы
выше не входят: `whoami`, `get_dashboard_link`, `campaigns_delete`, `lists_stats`.
