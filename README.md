# DashaMail MCP Server

MCP-сервер сервиса email-маркетинга [DashaMail](https://dashamail.ru): даёт
ИИ-агенту доступ к аккаунту — адресные базы, рассылки, отчёты, шаблоны,
автоматизации, транзакционные письма, вебхуки и входящая почта.

Сервер удалённый, разворачивать ничего не нужно.

| | |
|---|---|
| Адрес | `https://mcp.dashamail.ru/` |
| Транспорт | Streamable HTTP, протокол MCP 2025-06-18 |
| Авторизация | OAuth 2.1 + PKCE + динамическая регистрация клиента, либо API-ключ |
| Инструментов | 75 ([список](TOOLS.md)) |
| В реестре | `ru.dashamail/mcp` |
| Документация | https://dashamail.ru/api/mcp/ |

Исходный код сервера закрыт — репозиторий нужен для описания и обратной
связи. Ошибки и пожелания: issues или `support@dashamail.ru`.

## Подключение

Нужен аккаунт DashaMail — [зарегистрироваться](https://dashamail.ru).
Бесплатного тарифа достаточно, чтобы подключиться и посмотреть.

### Claude

Settings → Connectors → Add custom connector, адрес
`https://mcp.dashamail.ru/`. Откроется экран согласия DashaMail, где вы
выбираете, какие разделы аккаунта доступны агенту.

### Cursor, VS Code и другие клиенты

```json
{
  "mcpServers": {
    "dashamail": {
      "url": "https://mcp.dashamail.ru/"
    }
  }
}
```

Клиент сам зарегистрируется по OAuth. Если клиент OAuth не умеет, передайте
[API-ключ](https://dashamail.ru/api/) заголовком:

```json
{
  "mcpServers": {
    "dashamail": {
      "url": "https://mcp.dashamail.ru/",
      "headers": { "Authorization": "Bearer ВАШ_КЛЮЧ" }
    }
  }
}
```

## Что важно знать

**Сначала черновик.** Создание рассылки никогда не запускает отправку — для
этого есть отдельные инструменты `campaigns_schedule` и
`campaigns_send_now`. Так агент не разошлёт письма, «помогая» с черновиком.

**Подтверждение перед отправкой.** У восьми инструментов, которые отправляют
письма или удаляют данные, проставлен `destructiveHint` — клиент спрашивает
подтверждение перед каждым вызовом. Чтение идёт без вопросов.

**Права выбираете вы.** На экране согласия видно, какие разделы аккаунта
запрашивает клиент; выбор меняется потом в кабинете. Токен ограничен
выбранным.

**Два параметра для сужения:**

| Параметр | Что делает |
|---|---|
| `?readonly=1` | убирает все изменяющие инструменты, остаётся только чтение |
| `?toolset=core` | короткий набор (~35) для клиентов с малым контекстом |

Например: `https://mcp.dashamail.ru/?readonly=1&toolset=core`

## Что можно делать

- собрать и почистить адресную базу, проверить её здоровье перед отправкой;
- сделать черновик рассылки по брифу, запланировать, потом разобрать отчёт —
  открытия, клики, возвраты, отписки по доменам, ссылкам, географии и
  устройствам;
- разобраться, почему клиент не получил транзакционное письмо;
- сравнить периоды и каналы, не открывая кабинет.

## Ссылки

- [Документация MCP-сервера](https://dashamail.ru/api/mcp/)
- [Страница возможностей](https://dashamail.ru/features/mcp/)
- [REST API v2](https://dashamail.ru/api/)
- [Политика обработки персональных данных](https://dashamail.ru/privacy/)
  ([English](https://dashamail.ru/privacy_en/))

---

## English

MCP server for [DashaMail](https://dashamail.ru), an email marketing service
used by Russian businesses. It gives an AI agent access to the account:
subscriber lists and members, campaigns, reports, templates, automations,
transactional email, webhooks and inbound routing — 75 tools in total.

The server is remote, at `https://mcp.dashamail.ru/`, over Streamable HTTP.
Authentication is OAuth 2.1 with PKCE and dynamic client registration; an API
key in the `Authorization` header works too. A DashaMail account is required.

Draft-first by design: creating a campaign never sends it. Sending, scheduling
and deletion carry `destructiveHint`, so clients ask for confirmation before
each call; read-only tools run without prompts. Users pick scopes on the
consent screen and can change them later. `?readonly=1` drops every write
tool, `?toolset=core` exposes a compact set for small context windows.

The server source is closed; this repository holds the description and is the
place for issues. Tool list: [TOOLS.md](TOOLS.md). Support:
`support@dashamail.ru`.
