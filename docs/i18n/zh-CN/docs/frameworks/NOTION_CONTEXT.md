# Notion Context Source (中文 (简体))

🌐 **Languages:** 🇺🇸 [English](../../../../frameworks/NOTION_CONTEXT.md) · 🇪🇹 [am](../../../am/docs/frameworks/NOTION_CONTEXT.md) · 🇸🇦 [ar](../../../ar/docs/frameworks/NOTION_CONTEXT.md) · 🇦🇿 [az](../../../az/docs/frameworks/NOTION_CONTEXT.md) · 🇧🇬 [bg](../../../bg/docs/frameworks/NOTION_CONTEXT.md) · 🇧🇩 [bn](../../../bn/docs/frameworks/NOTION_CONTEXT.md) · 🇧🇦 [bs](../../../bs/docs/frameworks/NOTION_CONTEXT.md) · 🇨🇿 [cs](../../../cs/docs/frameworks/NOTION_CONTEXT.md) · 🇩🇰 [da](../../../da/docs/frameworks/NOTION_CONTEXT.md) · 🇩🇪 [de](../../../de/docs/frameworks/NOTION_CONTEXT.md) · 🇬🇷 [el](../../../el/docs/frameworks/NOTION_CONTEXT.md) · 🇪🇸 [es](../../../es/docs/frameworks/NOTION_CONTEXT.md) · 🇪🇪 [et](../../../et/docs/frameworks/NOTION_CONTEXT.md) · 🇮🇷 [fa](../../../fa/docs/frameworks/NOTION_CONTEXT.md) · 🇫🇮 [fi](../../../fi/docs/frameworks/NOTION_CONTEXT.md) · 🇫🇷 [fr](../../../fr/docs/frameworks/NOTION_CONTEXT.md) · 🇮🇪 [ga](../../../ga/docs/frameworks/NOTION_CONTEXT.md) · 🇮🇳 [gu](../../../gu/docs/frameworks/NOTION_CONTEXT.md) · 🇳🇬 [ha](../../../ha/docs/frameworks/NOTION_CONTEXT.md) · 🇮🇱 [he](../../../he/docs/frameworks/NOTION_CONTEXT.md) · 🇮🇳 [hi](../../../hi/docs/frameworks/NOTION_CONTEXT.md) · 🇭🇷 [hr](../../../hr/docs/frameworks/NOTION_CONTEXT.md) · 🇭🇺 [hu](../../../hu/docs/frameworks/NOTION_CONTEXT.md) · 🇦🇲 [hy](../../../hy/docs/frameworks/NOTION_CONTEXT.md) · 🇮🇩 [id](../../../id/docs/frameworks/NOTION_CONTEXT.md) · 🇳🇬 [ig](../../../ig/docs/frameworks/NOTION_CONTEXT.md) · 🇮🇹 [it](../../../it/docs/frameworks/NOTION_CONTEXT.md) · 🇯🇵 [ja](../../../ja/docs/frameworks/NOTION_CONTEXT.md) · 🇬🇪 [ka](../../../ka/docs/frameworks/NOTION_CONTEXT.md) · 🇰🇭 [km](../../../km/docs/frameworks/NOTION_CONTEXT.md) · 🇮🇳 [kn](../../../kn/docs/frameworks/NOTION_CONTEXT.md) · 🇰🇷 [ko](../../../ko/docs/frameworks/NOTION_CONTEXT.md) · 🇱🇹 [lt](../../../lt/docs/frameworks/NOTION_CONTEXT.md) · 🇱🇻 [lv](../../../lv/docs/frameworks/NOTION_CONTEXT.md) · 🇮🇳 [ml](../../../ml/docs/frameworks/NOTION_CONTEXT.md) · 🇮🇳 [mr](../../../mr/docs/frameworks/NOTION_CONTEXT.md) · 🇲🇾 [ms](../../../ms/docs/frameworks/NOTION_CONTEXT.md) · 🇲🇹 [mt](../../../mt/docs/frameworks/NOTION_CONTEXT.md) · 🇲🇲 [my](../../../my/docs/frameworks/NOTION_CONTEXT.md) · 🇳🇵 [ne](../../../ne/docs/frameworks/NOTION_CONTEXT.md) · 🇳🇱 [nl](../../../nl/docs/frameworks/NOTION_CONTEXT.md) · 🇳🇴 [no](../../../no/docs/frameworks/NOTION_CONTEXT.md) · 🇮🇳 [or](../../../or/docs/frameworks/NOTION_CONTEXT.md) · 🇮🇳 [pa](../../../pa/docs/frameworks/NOTION_CONTEXT.md) · 🇵🇭 [phi](../../../phi/docs/frameworks/NOTION_CONTEXT.md) · 🇵🇱 [pl](../../../pl/docs/frameworks/NOTION_CONTEXT.md) · 🇵🇹 [pt](../../../pt/docs/frameworks/NOTION_CONTEXT.md) · 🇧🇷 [pt-BR](../../../pt-BR/docs/frameworks/NOTION_CONTEXT.md) · 🇷🇴 [ro](../../../ro/docs/frameworks/NOTION_CONTEXT.md) · 🇷🇺 [ru](../../../ru/docs/frameworks/NOTION_CONTEXT.md) · 🇱🇰 [si](../../../si/docs/frameworks/NOTION_CONTEXT.md) · 🇸🇰 [sk](../../../sk/docs/frameworks/NOTION_CONTEXT.md) · 🇸🇮 [sl](../../../sl/docs/frameworks/NOTION_CONTEXT.md) · 🇷🇸 [sr](../../../sr/docs/frameworks/NOTION_CONTEXT.md) · 🇸🇪 [sv](../../../sv/docs/frameworks/NOTION_CONTEXT.md) · 🇰🇪 [sw](../../../sw/docs/frameworks/NOTION_CONTEXT.md) · 🇮🇳 [ta](../../../ta/docs/frameworks/NOTION_CONTEXT.md) · 🇮🇳 [te](../../../te/docs/frameworks/NOTION_CONTEXT.md) · 🇹🇭 [th](../../../th/docs/frameworks/NOTION_CONTEXT.md) · 🇹🇷 [tr](../../../tr/docs/frameworks/NOTION_CONTEXT.md) · 🇺🇦 [uk-UA](../../../uk-UA/docs/frameworks/NOTION_CONTEXT.md) · 🇵🇰 [ur](../../../ur/docs/frameworks/NOTION_CONTEXT.md) · 🇺🇿 [uz](../../../uz/docs/frameworks/NOTION_CONTEXT.md) · 🇻🇳 [vi](../../../vi/docs/frameworks/NOTION_CONTEXT.md) · 🇳🇬 [yo](../../../yo/docs/frameworks/NOTION_CONTEXT.md) · 🇹🇼 [zh-TW](../../../zh-TW/docs/frameworks/NOTION_CONTEXT.md)

---

> **权威来源：** `src/lib/notion/api.ts`（REST 客户端）、`src/lib/db/notion.ts`
> （令牌持久化）、`open-sse/mcp-server/tools/notionTools.ts`（6 个 MCP 工具）、
> `src/app/api/settings/notion/route.ts`（设置 API）。工具注册和作用域
> 绑定位于 `open-sse/mcp-server/server.ts` 中。

## 功能简介

OmniRoute 可以连接到 **Notion** 工作区，将其用作**上下文源**——一个可由智能体通过内置 MCP 服务器访问的读写知识库。配置 Notion 集成令牌后，MCP 工具可让 LLM 搜索页面和数据库、读取页面内容和区块树、使用筛选条件/排序查询数据库，以及追加新区块——所有操作都通过 OmniRoute 代理（支持重试、超时和错误分类），
因此模型绝不会直接访问 Notion API。

该集成是官方 Notion REST API
（`https://api.notion.com/v1`、`Notion-Version: 2026-03-11`）的轻量级强化封装。客户端
（`src/lib/notion/api.ts`）增加了：

- 针对 `429` 和 `5xx` 的**指数退避重试**（最多尝试 3 次）。
- 通过 `AbortController` 实现的 **55 秒请求超时**。
- **类型化错误分类**——`NotionAuthError`（401/403）、
  `NotionNotFoundError`（404）、`NotionRateLimitError`（429，遵循 `retry after`
  提示）、`NotionValidationError`（400/409）、`NotionServerError`（5xx）、
  `NotionTimeoutError`。
- **消息清理**，在向外返回消息前移除类似堆栈跟踪的片段。

## 设置

Notion 令牌**没有对应的环境变量**——它通过
`src/lib/db/notion.ts` 存储在 SQLite 的 `key_value` 表中（命名空间为 `notion`，键为 `integration_token`）。可在端点控制面板的 **Context Sources** 选项卡中进行配置
（`ObsidianSourceCard` 的同级组件 `NotionSourceCard`），也可以通过设置 REST API 进行配置。

> [!NOTE]
> 此令牌是 **Notion 内部集成令牌**。请在
> <https://www.notion.com/my-integrations> 创建集成，然后将希望
> OmniRoute 访问的页面/数据库共享给该集成（Notion 的权限模型基于共享，
> 而非整个工作区）。

### 通过 REST 配置

```bash
# 保存并验证集成令牌（POST 会通过发起一次测试搜索进行验证）
curl -X POST http://localhost:20128/api/settings/notion \
  -H "Content-Type: application/json" \
  -d '{"token":"ntn_xxx"}'

# 检查连接状态
curl http://localhost:20128/api/settings/notion

# 断开连接（清除已存储的令牌）
curl -X DELETE http://localhost:20128/api/settings/notion
```

这三种方法均需要通过控制面板身份验证（`isAuthenticated`）。执行 `POST` 时，
OmniRoute 会保存令牌并立即运行一次仅返回 1 条结果的测试搜索；如果 Notion
返回错误对象，则会清除令牌，并使该调用以 `400` 失败。

## MCP工具 (6)

在`open-sse/mcp-server/tools/notionTools.ts`中定义。令牌在调用时通过`getNotionToken()`解析；如果没有配置，该工具会抛出`"Notion integration token not configured. Set it in Settings > Context Sources."`

| 工具                         | 范围           | 描述                                                                |
| ---------------------------- | -------------- | ------------------------------------------------------------------- |
| `notion_search`              | `read:notion`  | 通过文本查询搜索页面和数据库（返回标题、 IDs、 URLs）。已分页。     |
| `notion_get_page`            | `read:notion`  | 通过ID获取页面的内容和元数据。                                      |
| `notion_list_block_children` | `read:notion`  | 列出块或页面（块树）的所有块子级。已分页。                          |
| `notion_query_database`      | `read:notion`  | 使用可选的`filter` + `sorts` （Notion API格式）查询数据库。已分页。 |
| `notion_get_database`        | `read:notion`  | 通过ID获取数据库的schema/metadata 。                                |
| `notion_append_blocks`       | `write:notion` | 将块子级附加到现有块或页面（每个请求最多 100 个块）。               |

### 输入参数

- `notion_search` — `query` （1–500 个字符）、 `pageSize` （1–100，默认 20）、 `startCursor` （可选）。
- `notion_get_page` — `pageId` （32 个字符的十六进制或UUID）。
- `notion_list_block_children` — `blockId`、 `pageSize` （1–100，默认 50）、 `startCursor` （可选）。
- `notion_query_database` — `databaseId`、 `filter` （可选， Notion过滤器格式）、 `sorts` （可选数组）、 `pageSize` （1–100，默认 50）、 `startCursor` （可选）。
- `notion_get_database` — `databaseId`.
- `notion_append_blocks` — `blockId`、 `children` （块对象数组）、 `after` （可选位置）。

### 范围

读取工具需要`read:notion` ，写入工具需要`write:notion`。当`OMNIROUTE_MCP_ENFORCE_SCOPES=true`时，范围由`withScopeEnforcement()`在`open-sse/mcp-server/server.ts`中强制执行，并且始终适用于API密钥缺少`manage`/`admin`的HTTP/SSE调用者；调用者允许的范围来自`OMNIROUTE_MCP_SCOPES` （逗号分隔）或经过身份验证的API密钥的范围上下文。有关完整范围模型，请参阅[MCP-SERVER.md](./MCP-SERVER.md) 。

## 端点

| 方法     | 路径                   | 用途                             |
| -------- | ---------------------- | -------------------------------- |
| `GET`    | `/api/settings/notion` | 返回 `{ connected, hasToken }`。 |
| `POST`   | `/api/settings/notion` | 保存并验证集成令牌。             |
| `DELETE` | `/api/settings/notion` | 断开连接（清除已存储的令牌）。   |

> 这些是仪表板设置路由。**不存在公开的 `/v1` Notion 代理
> 端点** — 只能通过上述 MCP 工具访问 Notion。

## 使用场景

- **基于知识的回答** — 让代理使用 `notion_search` 搜索工作区，并在回答前通过
  `notion_get_page` 获取最相关的结果，以便回复能够引用真实的内部文档。
- **数据库支持的工作流** — 使用过滤器和排序条件，通过 `notion_query_database`
  查询任务/CRM 数据库，然后汇总行数据或对其进行分类处理。
- **回写/日志记录** — 使用 `notion_append_blocks` 将会议记录、运行摘要或代理输出
  追加到现有页面中（仅追加；不进行破坏性编辑）。
- **结构探索** — 使用 `notion_list_block_children` 遍历页面的块树，或在查询数据库前
  使用 `notion_get_database` 了解数据库的属性架构。

## 相关文档

- [MCP 服务器](./MCP-SERVER.md) — 传输方式、作用域强制执行及完整的工具清单。
- [Obsidian 上下文源](./OBSIDIAN_CONTEXT.md) — 另一个内置上下文源。
- [记忆系统](./MEMORY.md) — 持久化会话记忆（作为补充上下文层自动注入，而非通过工具获取）。
