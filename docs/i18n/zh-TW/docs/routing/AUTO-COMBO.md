# OmniRoute Auto-Combo Engine (中文 (繁體))

🌐 **Languages:** 🇺🇸 [English](../../../../routing/AUTO-COMBO.md) · 🇪🇹 [am](../../../am/docs/routing/AUTO-COMBO.md) · 🇸🇦 [ar](../../../ar/docs/routing/AUTO-COMBO.md) · 🇦🇿 [az](../../../az/docs/routing/AUTO-COMBO.md) · 🇧🇬 [bg](../../../bg/docs/routing/AUTO-COMBO.md) · 🇧🇩 [bn](../../../bn/docs/routing/AUTO-COMBO.md) · 🇧🇦 [bs](../../../bs/docs/routing/AUTO-COMBO.md) · 🇨🇿 [cs](../../../cs/docs/routing/AUTO-COMBO.md) · 🇩🇰 [da](../../../da/docs/routing/AUTO-COMBO.md) · 🇩🇪 [de](../../../de/docs/routing/AUTO-COMBO.md) · 🇬🇷 [el](../../../el/docs/routing/AUTO-COMBO.md) · 🇪🇸 [es](../../../es/docs/routing/AUTO-COMBO.md) · 🇪🇪 [et](../../../et/docs/routing/AUTO-COMBO.md) · 🇮🇷 [fa](../../../fa/docs/routing/AUTO-COMBO.md) · 🇫🇮 [fi](../../../fi/docs/routing/AUTO-COMBO.md) · 🇫🇷 [fr](../../../fr/docs/routing/AUTO-COMBO.md) · 🇮🇪 [ga](../../../ga/docs/routing/AUTO-COMBO.md) · 🇮🇳 [gu](../../../gu/docs/routing/AUTO-COMBO.md) · 🇳🇬 [ha](../../../ha/docs/routing/AUTO-COMBO.md) · 🇮🇱 [he](../../../he/docs/routing/AUTO-COMBO.md) · 🇮🇳 [hi](../../../hi/docs/routing/AUTO-COMBO.md) · 🇭🇷 [hr](../../../hr/docs/routing/AUTO-COMBO.md) · 🇭🇺 [hu](../../../hu/docs/routing/AUTO-COMBO.md) · 🇦🇲 [hy](../../../hy/docs/routing/AUTO-COMBO.md) · 🇮🇩 [id](../../../id/docs/routing/AUTO-COMBO.md) · 🇳🇬 [ig](../../../ig/docs/routing/AUTO-COMBO.md) · 🇮🇹 [it](../../../it/docs/routing/AUTO-COMBO.md) · 🇯🇵 [ja](../../../ja/docs/routing/AUTO-COMBO.md) · 🇬🇪 [ka](../../../ka/docs/routing/AUTO-COMBO.md) · 🇰🇭 [km](../../../km/docs/routing/AUTO-COMBO.md) · 🇮🇳 [kn](../../../kn/docs/routing/AUTO-COMBO.md) · 🇰🇷 [ko](../../../ko/docs/routing/AUTO-COMBO.md) · 🇱🇹 [lt](../../../lt/docs/routing/AUTO-COMBO.md) · 🇱🇻 [lv](../../../lv/docs/routing/AUTO-COMBO.md) · 🇮🇳 [ml](../../../ml/docs/routing/AUTO-COMBO.md) · 🇮🇳 [mr](../../../mr/docs/routing/AUTO-COMBO.md) · 🇲🇾 [ms](../../../ms/docs/routing/AUTO-COMBO.md) · 🇲🇹 [mt](../../../mt/docs/routing/AUTO-COMBO.md) · 🇲🇲 [my](../../../my/docs/routing/AUTO-COMBO.md) · 🇳🇵 [ne](../../../ne/docs/routing/AUTO-COMBO.md) · 🇳🇱 [nl](../../../nl/docs/routing/AUTO-COMBO.md) · 🇳🇴 [no](../../../no/docs/routing/AUTO-COMBO.md) · 🇮🇳 [or](../../../or/docs/routing/AUTO-COMBO.md) · 🇮🇳 [pa](../../../pa/docs/routing/AUTO-COMBO.md) · 🇵🇭 [phi](../../../phi/docs/routing/AUTO-COMBO.md) · 🇵🇱 [pl](../../../pl/docs/routing/AUTO-COMBO.md) · 🇵🇹 [pt](../../../pt/docs/routing/AUTO-COMBO.md) · 🇧🇷 [pt-BR](../../../pt-BR/docs/routing/AUTO-COMBO.md) · 🇷🇴 [ro](../../../ro/docs/routing/AUTO-COMBO.md) · 🇷🇺 [ru](../../../ru/docs/routing/AUTO-COMBO.md) · 🇱🇰 [si](../../../si/docs/routing/AUTO-COMBO.md) · 🇸🇰 [sk](../../../sk/docs/routing/AUTO-COMBO.md) · 🇸🇮 [sl](../../../sl/docs/routing/AUTO-COMBO.md) · 🇷🇸 [sr](../../../sr/docs/routing/AUTO-COMBO.md) · 🇸🇪 [sv](../../../sv/docs/routing/AUTO-COMBO.md) · 🇰🇪 [sw](../../../sw/docs/routing/AUTO-COMBO.md) · 🇮🇳 [ta](../../../ta/docs/routing/AUTO-COMBO.md) · 🇮🇳 [te](../../../te/docs/routing/AUTO-COMBO.md) · 🇹🇭 [th](../../../th/docs/routing/AUTO-COMBO.md) · 🇹🇷 [tr](../../../tr/docs/routing/AUTO-COMBO.md) · 🇺🇦 [uk-UA](../../../uk-UA/docs/routing/AUTO-COMBO.md) · 🇵🇰 [ur](../../../ur/docs/routing/AUTO-COMBO.md) · 🇺🇿 [uz](../../../uz/docs/routing/AUTO-COMBO.md) · 🇻🇳 [vi](../../../vi/docs/routing/AUTO-COMBO.md) · 🇳🇬 [yo](../../../yo/docs/routing/AUTO-COMBO.md) · 🇨🇳 [zh-CN](../../../zh-CN/docs/routing/AUTO-COMBO.md)

---

> **使用者注意**：想要快速開始嗎？請參閱 [Auto-Combo 使用者指南](../getting-started/AUTO-COMBO-GUIDE.md)，其中提供簡明的說明與範例。

> 具備自適應評分與零設定自動路由的自我管理模型鏈

## 零配置自動路由（`auto/`前綴）

不需要創建組合。直接在客戶端使用`auto`或`auto/`變體。

### 快速範例

| 型號ID              | 行為                                                                                           |
| ------------------- | ---------------------------------------------------------------------------------------------- |
| `auto`              | 合格的提供者模型、 LKGP策略和平衡權重                                                          |
| `auto/coding`       | 編碼任務的品質優先權重                                                                         |
| `auto/fast`         | 有利於較低延遲和健康的提供者                                                                   |
| `auto/cheap`        | 節省成本的權重：有利於較低的目錄價格；保持LKGP黏性，而不是嚴格的最便宜優先排序                 |
| `auto/subscription` | 僅計劃包含的配額，即時驗證；空池返回HTTP 503，絕不是計費後備                                   |
| `auto/thrifty`      | 訂閱→無鑰匙→免費→便宜→高級版，一次一檔；可以計費                                               |
| `auto/offline`      | 有利於配額可用性和提供者健康狀況（`offline-friendly` pack）；非離線推理—請求仍發送至遠端提供者 |
| `auto/smart`        | 品質第一的權重，探索率 10%                                                                     |
| `auto/lkgp`         | 顯式LKGP，與預設`auto`具有相同的權重                                                           |
| `auto/chaos`        | 每個提供者一個模型的並行面板，預設最多五個，回傳一個答案                                       |

權重變體保留了LKGP黏性，因此`fast`和`cheap`表達偏好，而不是保證每個請求的最低延遲或價格。 `auto/chaos`進行多個上游呼叫。 `auto/thrifty`可以使用付費容量；恢復計畫配額取決於更新資格和連接冷卻時間，而不僅僅是重置時間。請參閱[訂閱優先路由](./SUBSCRIPTION_LADDER.md)。

### 類別×層級構成 (`auto/<category>:<tier>`)

OpenRouter 風格的後綴分隔**什麼樣的路線**（類別）來自**如何優化它**（層），因此您可以自由組合它們（#4235 B 階段， `open-sse/services/autoCombo/suffixComposition.ts`）：

- **類別**： `coding` · `reasoning` · `vision` · `chat` · `multimodal`。 `vision`/`multimodal`保留具有視覺能力的模型； `reasoning`保留reasoning/thinking模型。 `coding`和`chat`不加入能力過濾器。非聊天類別在任何層覆蓋之前選擇品質優先的權重。
- **等級**（選擇評分權重/池過濾器）： `fast` （快速發貨）· `cheap` （別名`floor`，成本節約器）· `reliable` （斷路器運行狀況+延遲穩定性）· `free` / `pro` （透過`classifyTier` —免費層與高級層按模型層過濾池）。 `subscription`和`thrifty`採用基於連線的[訂閱階梯](./SUBSCRIPTION_LADDER.md)。

| 例子                   | 決心                                              |
| ---------------------- | ------------------------------------------------- |
| `auto/coding:fast`     | 合格池，低延遲權重                                |
| `auto/coding:cheap`    | 合格池，節省成本的權重（別名`auto/coding:floor`） |
| `auto/reasoning:pro`   | 僅限reasoning/thinking型號，高級                  |
| `auto/vision`          | 具有品質第一權重的視覺模型                        |
| `auto/multimodal:free` | 支援多式聯運的型號，僅限免費套餐                  |

任何有效的`auto/<category>[:<tier>]`都會按需解析；精選子集在`/v1/models`和儀表板（ `open-sse/services/autoCombo/builtinCatalog.ts`中的`AUTO_SUFFIX_VARIANTS` ）中進行廣告。 Category/tier過濾是**預設失敗關閉**：如果沒有符合條件的模型匹配，則虛擬組合有一個空池，並且聊天解析器返回HTTP 503 (`src/sse/handlers/chatHelpers.ts`)。過濾器是`narrowPoolByCategoryTier` in `open-sse/services/autoCombo/virtualFactory.ts`。

當過濾器不符合任何內容時，`OMNIROUTE_AUTO_FREE_FALLBACK_TO_FULL_POOL=true`將舊版category/tier恢復到完整池；這可以丟棄所要求的層或能力約束。模型系列過濾器從不使用該後備，並且僅限訂閱的路由仍然需要經過驗證的計劃包含的容量。

> **即時模型智能：**自動路由健康度由即時通知**競技場ELO**排名+**模型開發**當`ARENA_ELO_SYNC_ENABLED`標誌開啟時分層資料（否則回落到靜態適應度圖）。

**使用方法：**

```bash
# Any IDE or CLI tool that supports OpenAI format
Base URL: http://localhost:20128/v1
API Key:  <your-endpoint-key>

# In your code/config, set model to:
model: "auto"                 # balanced default
model: "auto/coding"          # favor coding task fit
model: "auto/fast"            # favor lower latency
model: "auto/cheap"           # favor lower catalog cost
```

**會發生什麼事：**

1. OmniRoute偵測`src/sse/handlers/chat.ts`中的`auto/`前綴
2. 查詢全部**活躍的提供者連接**從資料庫中
3. 應用憑證、模型可見性和資格過濾器
4. 從可用模型建立邏輯provider/model候選者，保留符合條件的帳戶白名單以供調度
5. 建立一個**虛擬組合**記憶體中（不儲存在DB中）
6. 使用所選變體的權重配置檔+ LKGP策略的路線

**主要特性：**

- ✅**始終開啟：**無需切換，無需建立組合，無需配置
- ✅**動態的：**自動反映目前連線的提供者
- ✅**會話黏性：** LKGP確保優先考慮最後一個成功的提供者
- ✅**多帳戶感知：**邏輯provider/model候選者保留符合條件的帳戶白名單
- ✅**無需儲存組合：**虛擬配置保留在記憶體中；正常的路由指標和運行時狀態仍然可以保留

### 每鍵候選控制（#7819，等級 1 + 2）

`GET /v1/auto-combo/{channel}/candidates` （`{channel}` = `auto/`之後的後綴，或基本通道的文字`auto` ）是**只讀**列出`auto/*`通道的目前候選池的端點，用即時可達性裝飾，重用現有的彈性讀取（絕不是原始斷路器`state`）：

- 提供者斷路器— `getCircuitBreaker(provider).getStatus()` / `.canExecute()`
- 已解析`provider_connections`行上的連接冷卻— `rateLimitedUntil` / `testStatus`
- 型號鎖定— `isModelLocked(provider, connectionId, model)`

每個候選人還攜帶該API密鑰的`excluded`標誌。排除項按 API 金鑰儲存（`auto_candidate_overrides`表、遷移`128`） — OmniRoute是單一租戶，沒有`users`表，因此`apiKeyId`是最接近的真實每個呼叫者身分— ，並透過純粹的、經過單元測試的`filterExcludedCandidates()` (`open-sse/services/autoCombo/candidateOverrides.ts`) 在`open-sse/services/autoCombo/virtualFactory.ts`中的候選池阻塞點強制執行。過濾器是**故障開放**：未設定的apiKeyId/channel或DB查找失敗都會使池不被過濾，因此未配置覆蓋的操作員會看到與此功能之前相同的路由位元組。

**延後到後續問題：**每個候選權重+明確排序（第 3 級—饋入現有weighted/priority策略路徑）並為每個`auto/*`通道固定特定的`combo.ts`策略（第 4 級）。請參閱#7819計劃，以了解有關在單一租用戶模型下覆蓋是否應保留每個 API 金鑰或成為全域的懸而未決的問題。

**幕後花絮：**

```txt
Request: { model: "auto/coding" }
   ↓
src/sse/handlers/chat.ts detects prefix
   ↓
createVirtualAutoCombo('coding') → candidatePool from active connections
   ↓
handleComboChat (same engine as persisted combos)
   ↓
Auto-scoring selects best provider/model per request
```

**實施文件：**

| 文件                                                      | 目的                            |
| --------------------------------------------------------- | ------------------------------- |
| `open-sse/services/autoCombo/autoPrefix.ts`               | 前綴解析器 (`parseAutoPrefix`)  |
| `open-sse/services/autoCombo/virtualFactory.ts`           | 建立虛擬`AutoComboConfig`對象   |
| `open-sse/services/autoCombo/providerRegistryAccessor.ts` | 用於模擬提供者註冊表的測試鉤子  |
| `src/sse/handlers/chat.ts`                                | 整合：自動前綴短路              |
| `src/shared/constants/providers.ts`                       | `SYSTEM_PROVIDERS.auto`系統入口 |

## 儲存的自動組合的帳戶首選項

智慧型自動編輯器提供了一個可選的**帳戶偏好**部分。每個連線都可以是首選、正常（預設）、保留或排除。多個連接可以共享一個層。自動在第一個符合條件的層中選擇，保留其scoring/router行為；失敗的嘗試會落入剩餘的具體帳戶，優先於正常帳戶，然後再保留。此組合從不使用排除的連線。

此設定儲存為`config.accountPreferences`，由連接ID鍵入：

```json
{
  "accountPreferences": {
    "connection-a": "preferred",
    "connection-b": "preferred",
    "connection-c": "reserve",
    "connection-d": "excluded"
  }
}
```

省略或空的地圖會保留現有的路線。首選項不會啟用已停用的連線、授予 API 金鑰存取權限、復原配額阻止的候選者或繞過預算檢查。每次嘗試都僅限於其特定連接，因此帳戶後備無法跳轉組合路由器後面的層。現有的會話關聯性可能會保留符合條件的帳戶；排除綁定到本機回合的帳戶會停止該回合，而不是默默地更改帳戶。

配置的首選項使用帳戶感知自動路徑：未調度未綁定的上下文快取、智慧管道、混亂和影子快捷方式。這些請求的投機對沖被停用，因此儲備帳戶無法與首選帳戶競爭。其他組合策略不解釋此設定。將組合從「自動」變更為保留已儲存的首選項以供以後切換回來。

## 與真實型號 ID 相符的組合名稱

`name`與裸模型 id 相同的組合（例如名為`gpt-5.5`組合）是一個**有意的、支持的模式**，不是一個錯誤：它是[#6940](https://github.com/cheaper-inference/OmniRoute/issues/6940)中記錄的每個模型 ID 提供者回退的機制。由於組合解析在裸模型 ID 解析（ `src/sse/services/model.ts`中的`getComboForModel()` ）之前進行檢查，因此對裸 ID `gpt-5.5`的請求將通過組合的目標（例如`acme-responses/gpt-5.5`、 `backup-responses/gpt-5.5`）進行路由，而不是直接發送到單個提供者—這會重用為[#3227/#3233](https://github.com/cheaper-inference/OmniRoute/issues/3227)構建的組合會重寫前優先級，並由`tests/unit/responses-combo-resolution-3227.test.ts`測試前`tests/unit/combo-name-codex-responses-rewrite.test.ts`進行測試的組合。

建立組合或將組合重新命名為隱藏真實模型 ID 的名稱是**從未拒絕過**—這樣做會破壞這個記錄的工作流程。相反（#8530），當（新）名稱與真實模型 ID 衝突時， `POST /api/combos`和`PUT /api/combos/[id]`將非阻塞`warning`欄位附加到回應：

```json
{ "warning": { "code": "COMBO_NAME_SHADOWS_MODEL", "modelId": "gpt-5.5", "providerId": "openai" } }
```

啟動時， `scanComboModelNameCollisionsAtBoot()` (`src/instrumentation-node.ts`) 也會記錄一條單行`[STARTUP]`警告，枚舉隱藏模型 id 的每個現有組合，因此意外命中此警告的操作員（而不是按照#6940故意命中）會收到信號。檢測助手位於`src/lib/combos/modelNameCollision.ts`中。

## 從客戶端呼叫自訂組合

持久組合（設定→組合）僅在客戶端發送組合的**確切的名字**在`model`欄位—中，組合名稱沒有模糊或部分匹配，且不涉及`auto/`前綴。解析順序（`getComboForModel()` in `src/sse/services/model.ts`）：

1. 精確的組合名稱匹配（`model: "my-combo"`），
2. `combo/<name>`字首 (`model: "combo/my-combo"`),
3. 模型→組合 glob 映射 (`/api/model-combo-mappings`)。

```bash
curl -X POST http://localhost:20128/v1/chat/completions \
  -H "Authorization: Bearer <key>" \
  -H "Content-Type: application/json" \
  -d '{"model":"my-combo","messages":[{"role":"user","content":"Hello"}]}'
```

兩個常見的陷阱：

- **`auto`不使用你的連擊。** `auto`/`auto/*`建立自己的零配置候選池，並且僅在組合字面名稱為`auto`時才參考持久組合（不建議）。若要透過組合進行路由，請傳送其確切名稱—而不是`auto`。
- **`openrouter/auto`是真正的付費OpenRouter產品**（“自動最佳可用”），而不是OmniRoute別名。它是OpenRouter註冊表 (`open-sse/config/providers/registry/openrouter/index.ts`) 的單一靜態模型條目，並且單獨計費。使用設定→路由→隱藏付費模型將其從`auto`池中排除。

請參閱[#7992](https://github.com/cheaper-inference/OmniRoute/issues/7992)和[#7111](https://github.com/cheaper-inference/OmniRoute/issues/7111)以了解此文件的原始混淆。

## 它是如何工作的（持久自動組合）

自動組合引擎使用以下方式動態對provider/model候選者進行評分**16 個聲明因素**（在`open-sse/services/autoCombo/scoring.ts` → `DEFAULT_WEIGHTS`中定義）。預設權重總和為`1.0`；自訂權重由`normalizeScoringWeights()`重新規範化。預設情況下，三個因素的權重為零： `cacheAffinity`、 `resetWindowAffinity`和`reliability`。模式包為`reliability`賦予`0.03`權重，或`reliability-first`中的`0.04` ； `quality`預設在`quality-first`中攜帶`0.03` ，在其他包中則攜帶`0.02` 。 `cacheAffinity`還在加權分數之外控制提示快取重複資料刪除。

![Auto-Combo 16-factor scoring](../diagrams/exported/auto-combo-scoring.svg)

> 來源： [diagrams/auto-combo-scoring.mmd](../diagrams/auto-combo-scoring.mmd) （透過`npm run docs:render-diagrams`重新生成）。檔案名稱是歷史的；來源圖和渲染圖顯示了`DEFAULT_WEIGHTS`中聲明的所有 16 個因素。

| 因素                  | 預設重量 | 描述                                                                                                                                         |
| :-------------------- | :------- | :------------------------------------------------------------------------------------------------------------------------------------------- |
| `quota`               | 0.1429   | 剩餘配額/速率限制空間 [0..1]                                                                                                                 |
| `health`              | 0.1605   | 斷路器的健康分數（CLOSED= 1.0、 HALF_OPEN= 0.5、 OPEN= 0.0）                                                                                 |
| `costInv`             | 0.1429   | 逆**混合**成本（60% 輸入+ 40% 輸出代幣價格，標準化） —更便宜=得分較高                                                                        |
| `latencyInv`          | 0.1143   | 反向 p95 延遲歸一化為池—更快=得分更高                                                                                                        |
| `taskFit`             | 0.0762   | 任務類型適應性（編碼、審查、規劃、分析、調試、文件）                                                                                         |
| `stability`           | 0.0476   | 基於延遲標準差的基於變異數的穩定性—反應時間波動得分較低的候選者                                                                              |
| `tierPriority`        | 0.0476   | 帳戶等級優先級— Ultra = 1.0、Pro = 0.67、Standard = 0.33、Free = 0.0                                                                         |
| `tierAffinity`        | 0.0476   | 候選人層級與清單推薦層級之間的親和度                                                                                                         |
| `specificityMatch`    | 0.0476   | 請求特異性（清單提示）和模型層之間的匹配                                                                                                     |
| `contextAffinity`     | 0.0476   | 請求的上下文視窗需求與模型的上下文視窗之間的關聯性                                                                                           |
| `sessionAvailability` | 0.0476   | 此會話的候選連線的OAuth會話可用性（`getOAuthSessionAvailability()`；非 OAuth 連線得分 1.0）                                                  |
| `connectionDensity`   | 0.0476   | 在同一提供者的連線之間分散負載（反集中）                                                                                                     |
| `cacheAffinity`       | 0.00     | 與最有可能已持有此請求的提示快取前綴 (`open-sse/services/combo/promptCacheAffinity.ts`) 的連接的 Rendezvous-hash 親和力；預設為停用（#8008） |
| `resetWindowAffinity` | 0.00     | 偏向配額重置視窗有利的連線（預設為停用）                                                                                                     |
| `quality`             | 0.03     | 來自路由事件品質追蹤器的回饋驅動的輸出品質訊號；沒有觀察結果的候選人得到中性 0.5                                                             |
| `reliability`         | 0.00     | 從 10 個樣本樓層後面 24 小時的使用歷史記錄中觀察到的成功份額`1 - failureRate`（否則為實時指標）；沒有觀察結果的候選讀作 1.0。預設禁用        |

冷啟動後，記憶體中的`quality`追蹤器 (`open-sse/services/routing/quality.ts`) 為空，因此每個候選者都會獲得中立的`0.5`分數，直到第一個觀察結果落地。

> **無法讀取的配額 (#15347)。**當提供者有配額獲取器但它傳回任何可讀內容（獲取失敗、缺少憑證、僅使用訊息或沒有可解析`windows`且沒有有限`percentUsed`格式錯誤快照，包括`percentUsed: null`）時，候選者在`quota`軸上對`0`進行評分，其最終得分乘以`UNREADABLE_QUOTA_SOFT_DEPRIORITIZE_FACTOR` (0.5, `autoStrategy.ts`)，與懲罰連接狀態。失敗的使用讀取是有關遙測的證據，而不是提供者的證據，因此它的排名嚴格低於任何實際讀取，包括已確認的 100%-used讀取，但絕不會被硬阻止或驅逐。沒有上限的提供者將`unlimited: true`和分數報告為完整配額；沒有註冊配額獲取器的提供者根本沒有遙測來源，並保留預設值`100`。

**和：** `0.1429 + 0.1605 + 0.1429 + 0.1143 + 0.0762 + (7 × 0.0476) + 0.00 + 0.00 + 0.03 + 0.00 = 1.0`如`DEFAULT_WEIGHTS`中所聲明的；使用者配置的權重在評分之前由`normalizeScoringWeights()`重新歸一化為分佈。

## 模式套件

`open-sse/services/autoCombo/modePacks.ts` 中有 6 個預先定義的權重設定檔。每個套件都會完全取代預設權重，讓選擇偏向某個目標。每個套件的權重總和都已是 `1.0`（以四位小數顯示時為 `0.9999`），因此套件啟用時，`normalizeScoringWeights()` 沒有任何實質需要修正的內容——以下數值在考量四捨五入後，就是評分器實際套用的值。

| 因素                  | ship-fast  | cost-saver | quality-first | offline-friendly | reliability-first | chaos-mode |
| :-------------------- | :--------- | :--------- | :------------ | :--------------- | :---------------- | :--------- |
| `quota`               | 0.1133     | 0.1133     | 0.0752        | **0.3324**       | 0.1133            | 0.0376     |
| `health`              | 0.2667     | 0.1810     | 0.1714        | 0.2667           | **0.3524**        | **0.4000** |
| `costInv`             | 0.0276     | **0.3324** | 0.0276        | 0.0752           | 0.0181            | 0.0140     |
| `latencyInv`          | **0.3048** | 0.0476     | 0.0476        | 0.0476           | 0.0476            | 0.0186     |
| `taskFit`             | 0.0952     | 0.0952     | **0.3524**    | 0.0000           | 0.0952            | 0.1905     |
| `stability`           | 0.0000     | 0.0476     | 0.1429        | 0.0952           | 0.1905            | 0.1714     |
| `tierPriority`        | 0.0376     | 0.0376     | 0.0276        | 0.0376           | 0.0276            | 0.0040     |
| `tierAffinity`        | 0.0000     | 0.0000     | 0.0000        | 0.0000           | 0.0000            | 0.0000     |
| `specificityMatch`    | 0.0000     | 0.0000     | 0.0000        | 0.0000           | 0.0000            | 0.0000     |
| `contextAffinity`     | 0.0095     | 0.0000     | 0.0000        | 0.0000           | 0.0000            | 0.0186     |
| `sessionAvailability` | 0.0476     | 0.0476     | 0.0476        | 0.0476           | 0.0476            | 0.0476     |
| `resetWindowAffinity` | 0.0000     | 0.0000     | 0.0000        | 0.0000           | 0.0000            | 0.0000     |
| `connectionDensity`   | 0.0476     | 0.0476     | 0.0476        | 0.0476           | 0.0476            | 0.0476     |
| `quality`             | 0.02       | 0.02       | **0.03**      | 0.02             | 0.02              | 0.02       |
| `reliability`         | 0.03       | 0.03       | 0.03          | 0.03             | **0.04**          | 0.03       |

注意事項：

- **套件包含 `quality` 和 `reliability`**（`quality 0.02`，`quality-first 0.03`；`reliability 0.03`，`reliability-first 0.04`），並且會完整取代權重映射（`weights = pack`，而非合併）。`DEFAULT_WEIGHTS` 包含 `quality 0.03 / reliability 0`；選擇 `balanced`/`default` 會保留這些預設值，選擇套件則會使用上方列出的套件值。在冷啟動資源池中（尚無觀測資料，因此 `quality 0.5` 且 `reliability 1`），這兩個因素在一般套件下會增加 `+0.04`（`0.03 + 0.01`），在 `quality-first` 下增加 `+0.045`，在 `reliability-first` 下增加 `+0.05`。
- 每個套件中的 `tierAffinity`、`specificityMatch` 和 `resetWindowAffinity` 都明確設為 `0`。
- 各套件的重點一覽：
  - **ship-fast** → latencyInv 0.3048 + health 0.2667（低延遲、健康的連線）
  - **cost-saver** → costInv 0.3324（最便宜的 token 勝出）
  - **quality-first** → taskFit 0.3524 + stability 0.1429 + quality 0.03，為所有套件中最高（最適合任務且表現一致的模型）
  - **offline-friendly** → quota 0.3324 + health 0.2667（不論速度／成本，最大化可用餘裕）
  - **reliability-first** → health 0.3524 + stability 0.1905 + reliability 0.04，為所有套件中最高（最少意外）
  - **chaos-mode** → health 0.4000 + taskFit 0.1905（權重套件 `auto/chaos` 指派給其面板成員的權重；平行扇出不會讀取這些權重，而且這不是故障注入設定檔，請參閱 [CHAOS-MODE.md](../guides/CHAOS-MODE.md#autochaos-parallel-fan-out)）

### 每個請求的控制項（標頭）— #6023 / #6024 / #6025 / #3470

`auto` 組合可透過三個標頭**針對每個請求**進行引導，而不會變更該組合已儲存的設定。這些標頭僅適用於 `auto` 策略，且只影響攜帶這些標頭的請求；未提供標頭時，會使用該組合已儲存的 `modePack`/`budgetCap`/`budgetFallback`。

| 標頭                          | 接受值                                                                                                                                                                         | 效果                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| :---------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `X-OmniRoute-Mode`            | 預設別名（`fast`、`balanced`、`quality`、`cheap`、`reliable`、`offline`）或原始套件名稱（`ship-fast`、`cost-saver`、`quality-first`、`offline-friendly`、`reliability-first`） | 覆寫此請求的評分權重。`balanced`/`default` 會強制使用預設權重（不使用套件）。未知值會被忽略（保留設定）。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| `X-OmniRoute-Budget`          | 正數（每個請求的最高 USD 金額）                                                                                                                                                | 硬性成本上限：預估成本超過此上限的候選項目會在選擇前被篩除。當**所有**候選項目都超出上限時的處理方式，由下方的 `X-OmniRoute-Budget-Fallback` 控制。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| `X-OmniRoute-Budget-Fallback` | `cheapest`（預設，別名：`cheapest-viable`、`soft`）或 `strict`（別名：`block`、`hard`）                                                                                        | `cheapest`：即使全域最便宜的候選項目仍超出上限，也會退回選擇該候選項目（舊版行為）。`strict`：拒絕進行選擇——請求會立即失敗並回傳 `HTTP 402`，而非在未提示的情況下超支。未知值會被忽略。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| `X-OmniRoute-Effort`          | `auto`（其他值保留）                                                                                                                                                           | 自適應思考預算：當請求**不含**任何形式的推理欄位（`reasoning_effort`、`reasoning`、`thinking`）時，閘道會根據確定性的請求結構訊號（最後一則使用者訊息的長度、截至最後一則使用者訊息的上下文大小、先前的工具結果、工具迴圈深度），將 `auto` 解析為 `low`/`medium`/`high`。訊號範圍僅限於目前回合——最後一則使用者訊息之後的所有內容都會被忽略——因此，工具迴圈中的每個請求都會解析為相同層級（每回合無狀態固定、不保留工作階段狀態，也不會在迴圈中途升級，以免破壞上游提示快取前綴）。用戶端明確指定的推理欄位一律優先。僅適用於上游分派解析為 OpenAI Chat Completions 格式的請求（`targetFormat === FORMATS.OPENAI`）——`reasoning_effort` 是 OpenAI 格式的欄位，因此此標頭對以 Claude 或 Gemini 為目標的請求不會產生作用（請參閱 `open-sse/handlers/chatCore/adaptiveEffortWiring.ts`）。 |

```bash
# 強制使用最快的設定檔、將此請求的費用上限設為 $0.05，並在可能超支時直接封鎖
curl -sS http://localhost:20128/v1/chat/completions \
  -H "Content-Type: application/json" \
  -H "X-OmniRoute-Mode: fast" \
  -H "X-OmniRoute-Budget: 0.05" \
  -H "X-OmniRoute-Budget-Fallback: strict" \
  -d '{"model":"auto","messages":[{"role":"user","content":"hi"}]}'
```

解析是一個純函式（`open-sse/services/autoCombo/requestControls.ts`）；解析後的值會傳入引擎現有的 `config.modePack` / `config.budgetCap` /
`config.budgetFallback` 輸入。組合中儲存的 `config.budgetFallback`（"strict" |
"cheapest"）會設定持續性原則；此標頭則會針對單一請求覆寫該原則。

## 所有路由策略

OmniRoute的組合引擎支持**22種路由策略**（在`src/shared/constants/routingStrategies.ts` → `ROUTING_STRATEGY_VALUES`中聲明）。 Auto Combo引擎本身是在`auto`策略下暴露的；其他可用於持久組合。

| 策略                | 描述                                                                                                                                                                                                                                                       |
| :------------------ | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `priority`          | 具有明確優先順序的第一目標有序列表                                                                                                                                                                                                                         |
| `weighted`          | 根據目標重量按比例隨機抽取；其他目標成為後備目標（見下文）                                                                                                                                                                                                 |
| `round-robin`       | 按黏性批次依序循環遍歷目標（預設情況下每個目標 3 次成功；見下文）                                                                                                                                                                                          |
| `context-relay`     | 當對話轉移到另一個帳戶時，優先順序加上移交摘要                                                                                                                                                                                                             |
| `fill-first`        | 完成每個目標的配額，然後再轉到下一個目標                                                                                                                                                                                                                   |
| `p2c`               | 對兩個目標進行採樣，並選擇更健康、更快的一個                                                                                                                                                                                                               |
| `random`            | 根據要求提供新鮮的 Fisher-Yates 洗牌；連續請求可以從同一目標開始                                                                                                                                                                                           |
| `least-used`        | 選擇此組合中記錄請求最少的目標（每個模型+帳戶）                                                                                                                                                                                                            |
| `cost-optimized`    | 首先嘗試最低的目錄輸入代幣價格；未知價格排在最後（不是最終請求成本）                                                                                                                                                                                       |
| `reset-aware` ⭐    | 對剩餘會話和每週配額以及重置緊急程度進行評分；近鄰輪換                                                                                                                                                                                                     |
| `reset-window`      | 優先選擇配額視窗重置最快的目標                                                                                                                                                                                                                             |
| `expiry-first`      | 首先使用其配額將過期的帳戶，未使用的—最接近重置截止日期的最高剩餘金額先行                                                                                                                                                                                  |
| `headroom`          | 選擇剩餘配額空間最多的目標                                                                                                                                                                                                                                 |
| `quota-weighted`    | 按配額可用性和飛行負載分配請求；保留會話關聯性                                                                                                                                                                                                             |
| `strict-random`     | 每個組合洗牌：每個目標在洗牌前使用一次；一個週期的最後一個永遠不會開始下一個週期                                                                                                                                                                           |
| `auto`              | 使用自動組合評分（16 因素） —**受到推崇的**                                                                                                                                                                                                                |
| `lkgp`              | 最後已知的良好路徑（固定到最後一個成功的提供者，然後退回到規則）                                                                                                                                                                                           |
| `context-optimized` | 首先嘗試最大的已知上下文視窗（已解決模型能力限制）                                                                                                                                                                                                         |
| `cache-optimized`   | 優先選擇可能在快取中保存提示前綴的合格連線（`open-sse/services/combo/promptCacheAffinity.ts`、 #8008）                                                                                                                                                     |
| `fusion` 🧬         | 並行地扇出一組模型，然後透過法官綜合一個答案（見下文）                                                                                                                                                                                                     |
| `pipeline`          | 依序運行目標，將每個步驟的輸出執行緒化到下一步的輸入；只傳回最終答案（#6396）                                                                                                                                                                              |
| `jev`               | 使用者偏好清單； TypeSafe Jev 承認哪些條目針對此請求執行。獲勝者優先，其他承認的目標保留您的順序。選擇加入並付費：僅在`COMBO_JEV_STRATEGY_ENABLED`開啟時呼叫（預設為關閉）；每個呼叫都會向 api.typesafe.ai 發送有界摘錄。當不可用時返回到您的訂單 (#15276) |

⭐ = v3.8.0 新增功能 · 🧬 = v3.8.36 新增功能

`jev`策略僅在啟用`COMBO_JEV_STRATEGY_ENABLED`時才會進行付費TypeSafe呼叫。單獨儲存的TypeSafe密鑰並不能啟用它。當標誌關閉時，組合保持操作員的命令，而不進行該呼叫（`open-sse/services/combo/jevAsk.ts`）。

### `weighted`語意

`weighted`是一個**根據請求按比例隨機抽取**(`open-sse/services/combo/targetSorters.ts` → `selectWeightedTarget`)，不是均衡器：

- 每個請求都會吸引**一**以機率`weight / totalWeight`步進；其餘步驟依權重降序排列，作為該請求的後備鏈。
- 權重為`0` （或缺失）的步驟是**從未畫過**雖然任何其他步驟的權重為> 0 —但它只能在繪製的步驟失敗後作為後備。僅當**全部**權重為 0 時選擇變得均勻。
- 目標全部不可用的—提供者斷路器`OPEN`、連接冷卻、模型鎖定—的步驟都會在發生之前從抽籤中刪除（`open-sse/services/combo/targetResolution.ts`），因此單一健康的步驟可以暫時贏得每個請求。
- `stickyWeightedLimit` （組合配置，預設`1` =關閉）在重新繪製之前固定多次連續成功的繪製步驟。

對於嚴格輪換，請使用`round-robin`； `weighted`上的相同權重給出了統計—而不是嚴格的—平衡。

### 代理管道模式

具有至少兩個模型的`pipeline`組合可以選擇使用`config.agenticOrchestration.enabled`進行planner/executor路由。第一個目標有規劃和最終答案；第二個目標發出客戶端本機工具呼叫。 OmniRoute從請求協定中偵測工具結果延續，詢問規劃器是否需要另一輪工具，並動態地使執行器或規劃器成為面向客戶端的最後一步。

可選的`config.agenticOrchestration.contextCompaction`在每個計劃者或執行者調度之前應用單獨的有效負載預算。明確啟用它：

```json
{
  "enabled": true,
  "defaultMaxChars": 400000,
  "targetRatio": 0.72,
  "toolResultMaxChars": 24000,
  "modelMaxChars": { "provider/planner": 175000, "provider/executor": 300000 }
}
```

這些是操作員選擇的序列化JSON字元預算，而不是令牌上下文視窗或保證的上游限制。精確模型IDs覆蓋預設值。高於閾值時，壓縮會刪除相同的工具定義，透過摘要修剪過大的工具證據，並根據目標比率刪除舊的完整歷史記錄組。它保留了system/developer指令、最新的使用者請求、最後一輪工具（包括並行calls/results）和Gemini的領先路由指令。保留頂級指令和工具設定。遺漏標記記錄刪除的歷史記錄；這是確定性的修剪，而不是語義總結。如果固定上下文仍然超出預算，則請求在聯絡模型之前返回 413。當禁用壓縮或壓縮低於閾值時，請求將保持不變地通過。

在工具結果延續上，當兩個連續完成的輪次重複相同的工具呼叫但結果不變時，或當兩個連續輪次中每個明確標記的結果失敗時， OmniRoute也會停止執行。更改的結果允許重複呼叫（例如輪詢）。此防護根據新的使用者請求進行重置，將並行呼叫分組為一輪，並支援Anthropic、聊天完成、回應和Gemini歷史記錄。規劃者收到原因並擁有最終答案，即使它要求另一輪工具也是如此。

第二個目標之後的其他模型是有序執行程式備份。失敗的HTTP回應或傳輸異常將前進到下一個執行器，攜帶相同的規劃器決策和本機工具，但該執行器自己的步驟提示和已解決的連接。第一個成功的回應原樣返回，包括SSE流；成功的流啟動後的失敗無法在此處重試。如果所有執行器都失敗，則傳回最後一個失敗的執行器。客戶端中止停止調度。

```json
{
  "strategy": "pipeline",
  "models": [{ "model": "provider/planner" }, { "model": "provider/executor" }],
  "config": {
    "agenticOrchestration": { "enabled": true, "maxToolRounds": 8 }
  }
}
```

執行器可以在一個回應中發出多個獨立的呼叫。相關呼叫在稍後的客戶端工具結果輪流中進行處理，規劃人員會審查每個結果。 `maxToolRounds`預設為`8`並接受`1`–`32`；一旦達成，規劃者必須給出最佳的最終答案。內部規劃器決策被緩衝，而選定的面向客戶的回應保留原始的流首選項。

### `round-robin`黏性批次和帳戶擴展

循環是批量的，而不是每一步一個請求：

- `stickyRoundRobinLimit` （組合配置，然後`comboStickyRoundRobinLimit`，然後`settings.stickyRoundRobinLimit`，預設**3** ）在輪換之前連續多次成功保持相同的目標。將組合覆蓋設定為`1`以進行單一請求輪換。組合編輯器顯示有效值及其來自哪一層。
- `connectionAwareExpansion` （組合配置，然後設置，預設**錯誤的**）在輪換之前將每個提供者層級的步驟擴展為每個帳戶的目標。 B 組策略（優先順序、加權、循環、隨機、p2c、最少使用、成本優化、lkgp、填充優先順序、嚴格隨機、上下文優化、快取優化、上下文中繼、融合、管道、jev）保持提供者層級的視圖，直到開啟。組合編輯器公開了繼承/開/關；繼承使用全域預設值（關閉）。
- 提示快取局部路由（`promptCacheAffinityEnabled`，預設**真的**) 對固定連線重新排序，以便符合的快取金鑰保留在一個帳戶上。它優先於固定的每個帳戶步驟的循環法和加權輪替。如果您需要嚴格旋轉，請在「設定→組合預設值」下將其關閉。沒有每個組合的覆蓋。

對於一種模型上的多帳戶輪換，首選**一個動態帳戶步驟**（空`connectionId`，整個池）具有黏性限制`1`，而不是三個固定的`connectionId`。即使RR計數器前進，固定步驟加上親和力也會折疊到同一帳戶上。

## 融合策略

`fusion`是一種能夠做到這一點的策略**不是**選擇一個目標。它將提示扇出**每個面板模型並行**，然後是一個可設定的**法官模型**從所有小組答覆中綜合出一個最終答案。從上游`decolua/9router`移植（OpenRouter的 Fusion 設計）；在`open-sse/services/fusion.ts`中實現。

工作原理：

0. **工具軸承旁路**—攜帶非空`tools`數組的請求，其中`tool_choice`未明確`"none"`完全跳過面板：它直接路由到單一模型（配置的判斷，或`panel[0]`），其中`tools`/`tool_choice`未經修改地傳遞。小組成員沒有工具存取權限，法官的綜合指令不鼓勵工具呼叫發射，因此agentic/tool-calling客戶端獲得真正的工具呼叫決策，而不是合成的散文（#6771）。
1. **扇出**（僅限非工具承載請求） —提示會立即發送到每個面板模型，強制非流式傳輸並剝離工具（法官需要完整的散文來合成）。
2. **法定人數恩典集合**一旦`minPanel`答覆到達， —就會為落後者啟動一個短暫的寬限計時器，然後繼續與收集到的任何內容進行融合。這限制了最慢模型對掛起時間的懲罰，並受到硬超時的限制。
3. **判斷綜合**—小組的答案是匿名的（`Source 1`， `Source 2`，... —因此法官權衡實質內容，而不是模型品牌）並交給法官，法官分析共識/矛盾/部分覆蓋/獨特見解/盲點，然後寫入**一**權威答案。判斷呼叫保留客戶端原始的`stream`標誌+工具，因此串流和下游工具使用仍然有效。
4. **優雅降級**— 0 小組回答→ `503`；恰好 1 個倖存者→直接返回答案（無需融合）；單型號面板直接回答。

小組成員也可能是引用另一個組合— `combo-ref`步驟 (`{kind: "combo-ref", comboName: "..."}`)，它解析為**一個黑盒子麵板聲音**（完全遞歸調度到引用的組合中，而不是該組合自己的目標的扇出），具有與每個其他組合引用消耗策略已經使用的相同的depth/cycle保護（#6764）。

### 配置

在組合的`config` blob 上設定（沒有架構遷移—它重複使用現有的`combos`表）：

| 場地                                     | 類型     | 預設           | 目的                                                   |
| :--------------------------------------- | :------- | :------------- | :----------------------------------------------------- |
| `config.judgeModel`                      | `string` | 第一個面板模型 | 綜合最終答案的模型                                     |
| `config.fusionTuning.minPanel`           | `number` | `2`            | 寬限計時器啟動前需要成功回答（限制為`[2, panelSize]`） |
| `config.fusionTuning.stragglerGraceMs`   | `number` | `8000`         | 一旦達到法定人數，落後者需要等待多長時間               |
| `config.fusionTuning.panelHardTimeoutMs` | `number` | `90000`        | 絕對上限，因此一個掛起的模型無法阻止請求               |

預設值位於`FUSION_DEFAULTS` (`open-sse/services/fusion.ts`) 中。

### 例子

```bash
curl -X POST http://localhost:20128/api/combos \
  -H "Authorization: Bearer <key>" \
  -H "Content-Type: application/json" \
  -d '{
    "name": "fusion-panel",
    "strategy": "fusion",
    "targets": [
      { "model": "cc/claude-opus-4-7" },
      { "model": "cx/gpt-5.5" },
      { "model": "glm/glm-5.1" }
    ],
    "config": {
      "judgeModel": "cc/claude-opus-4-7",
      "fusionTuning": { "minPanel": 2, "stragglerGraceMs": 8000, "panelHardTimeoutMs": 90000 }
    }
  }'
```

然後像任何組合一樣呼叫它： `{"model":"fusion-panel","messages":[...]}`。

## 虛擬 Auto-Combo 工廠

Auto Combo 引擎不需要預先定義的組合。相反地，`open-sse/services/autoCombo/virtualFactory.ts` 會即時建立候選項目：

1. 取得 `getProviderConnections({ isActive: true })`（所有已啟用的連線）
2. 篩選出具有有效憑證的連線（API 金鑰或透過 `hasUsableOAuthToken()` 判定為未過期的 OAuth 權杖）
3. 與 `getProviderRegistry()` 交叉比對模型可用性與定價
4. 針對每個 `(provider, model, connection)` 元組建立一個 `VirtualAutoComboCandidate`
5. 選擇 `connection.defaultModel`（或登錄檔中的第一個模型）作為分派目標
6. 使用 16 因子的 `scorePool()` 與變體的權重套件，為每個候選項目評分
7. 傳回產生於記憶體中的 `AutoComboConfig` 給 `handleComboChat()` — 絕不持久化至資料庫

這表示**新增一個已啟用 `auto/*` 的提供者，會自動擴充候選集區** — 不需要手動編輯組合。虛擬組合會針對每個請求重新建立，因此新加入或恢復健康狀態的連線都能立即被採用。

## 自我修復

- **暫時排除**：分數 < 0.2 → 排除 5 分鐘（漸進式退避，最長 30 分鐘）
- **斷路器感知**：OPEN → 自動排除；HALF_OPEN → 探測請求
- **事故模式**：>50% 為 OPEN → 停用探索，最大化穩定性
- **冷卻恢復**：排除期結束後，第一個請求會是縮短逾時時間的「探測」請求

## Bandit 探索

5% 的請求（可設定）會隨機路由至提供者進行探索。在事故模式下停用。

## API

有**沒有專用的`POST /api/combos/auto`端點**— Auto-Combo 有兩種消耗方式：

1. **零配置（建議）：**使用`model: "auto"`或`model: "auto/<variant>"`發送任何聊天完成請求。虛擬工廠根據—請求建立組合，無需持久性，無需API呼叫。

2. **與`strategy: "auto"`持久組合：**透過`POST /api/combos`建立常規組合併設定`strategy: "auto"`加`config.auto.weights` / `config.auto.candidatePool`。使用相同的評分引擎；此組合儲存在`combos`中並可由ID重複使用。

為了發現， `GET /api/combos/auto`列出了每個變體及其解析的候選池以及候選池視窗中的`context_length` / `max_output_tokens` — MAX 。客戶端（例如 opencode 外掛程式）必須通告這些值而不是`0`：零上下文完全停用 opencode 的自動壓縮，讓會話成長，直到網關的歷史清除破壞上下文。 MAX可以安全地進行廣告，因為自動組合上下文預過濾器會將超大請求路由到大視窗候選者。

```bash
# Zero-config usage (no combo creation)
curl -X POST http://localhost:20128/v1/chat/completions \
  -H "Authorization: Bearer <key>" \
  -H "Content-Type: application/json" \
  -d '{"model":"auto/coding","messages":[{"role":"user","content":"Hello"}]}'

# Persisted auto combo via the regular combos endpoint
curl -X POST http://localhost:20128/api/combos \
  -H "Content-Type: application/json" \
  -d '{"id":"my-auto","name":"Auto Coder","strategy":"auto","config":{"auto":{"candidatePool":["anthropic","google","openai"],"weights":{"quota":0.15,"health":0.3,"costInv":0.05,"latencyInv":0.35,"taskFit":0.1,"stability":0,"tierPriority":0.05}}}}'
```

### 自動佈線策略

持久的`strategy: "auto"`組合可以將`config.routerStrategy` （或舊版`config.auto.routerStrategy`）設定為以下之一：

- `rules` —預設加權評分
- `score` —選擇最高配置的加權分數。精確的關係保留配置的候選順序；來自完整排名池的現有`explorationRate`樣本。
- `cost` / `eco` —最便宜的健康提供者
- `latency` / `fast` —最低的 p95 延遲，但具有可靠性損失
- `sla-aware` / `sla` —喜歡滿足 p95 延遲、錯誤率和可選成本的候選人SLOs
- `lkgp` —最後已知的良好提供者優先
- `nadir` —詢問[Nadir](https://getnadir.com)的決定API提示需要池中的哪個模型；選擇加入，失敗時向`rules`開放
- `decision` —詢問配置的決策者（TypeSafe System One、您自己的決策URL或組合自己的模型之一）池中的哪個模型適合請求；在預設關閉`COMBO_DECISION_ROUTER_ENABLED`標誌後面，失敗打開到`rules`

### 路由器策略詳細信息

自動組合引擎公開了 7 個可插拔**RouterStrategy**您可以透過`config.routerStrategy` （或舊版`config.auto.routerStrategy`）交換的實現。每個策略都會從候選池中選擇一個提供者，並給出`RoutingContext` （任務類型、 tool/vision提示、令牌估計、可選的SLA策略、可選的最後已知的良好提供者）。

#### 1. `rules` （預設） — 16因素加權評分

包裝現有的評分引擎。過濾掉`OPEN`斷路器候選者，然後使用目前任務類型和`getTaskFitness()`運行`scorePool()` ，選擇得分最高的提供者。

```ts
class RulesStrategyImpl implements RouterStrategy {
  readonly name = "rules";
  readonly description = "16-factor weighted scoring (see DEFAULT_WEIGHTS)";

  select(pool, context) {
    const eligible = pool.filter((c) => c.circuitBreakerState !== "OPEN");
    const ranked = scorePool(
      eligible.length > 0 ? eligible : pool,
      context.taskType,
      undefined,
      getTaskFitness
    );
    return { provider: ranked[0].provider /* ... */ };
  }
}
```

**何時使用**: 預設.當您想要在所有訊號之間進行平衡權衡時使用。

**別名**： `rules` （無別名）

---

#### 2. `cost` / `eco` —最便宜的健康提供者

按`costPer1MTokens` （升序）對候選池進行排序，並選擇最便宜的。首先過濾掉`OPEN`候選者。

```ts
class CostStrategyImpl implements RouterStrategy {
  readonly name = "cost";
  readonly description = "Always selects cheapest available provider";

  select(pool, context) {
    const healthy = pool.filter((c) => c.circuitBreakerState !== "OPEN");
    const sorted = [...healthy].sort((a, b) => a.costPer1MTokens - b.costPer1MTokens);
    return { provider: sorted[0].provider /* ... */ };
  }
}
```

**何時使用**：成本敏感的工作負載、批次或後台作業。

**別名**: `cost`, `eco`

---

#### 3. `latency` / `fast` —最低的 p95 延遲，但具有可靠性損失

按`p95LatencyMs + (errorRate * 1000)`排序。錯誤率懲罰可確保不可靠的提供者排名較低，即使其標稱延遲較低。

```ts
class LatencyStrategyImpl implements RouterStrategy {
  readonly name = "latency";
  readonly description = "Prioritizes lowest p95 latency with reliability weighting";

  select(pool, context) {
    const healthy = pool.filter((c) => c.circuitBreakerState !== "OPEN");
    const sorted = [...healthy].sort(
      (a, b) => a.p95LatencyMs + a.errorRate * 1000 - (b.p95LatencyMs + b.errorRate * 1000)
    );
    return { provider: sorted[0].provider /* ... */ };
  }
}
```

**何時使用**：對延遲敏感的工作負載，例如即時聊天、自動完成或互動式編碼助理。

**別名**: `latency`, `fast`

---

#### 4. `sla-aware` / `sla` — latency/error/cost SLO合規性

根據每個候選者滿足配置的SLO策略的程度對其進行評分：

| 因素       | 重量 | 公式                                              |
| ---------- | ---- | ------------------------------------------------- |
| 延遲分數   | 35%  | `threshold / max(value, ε)`                       |
| 錯誤分數   | 35%  | `threshold / max(value, ε)`                       |
| 健康評分   | 15%  | `1.0` (CLOSED) / `0.5` (HALF_OPEN) / `0.0` (OPEN) |
| 成本分數   | 10%  | `threshold / max(value, ε)`或逆歸一化             |
| 穩定性得分 | 5%   | 逆歸一化延遲 stddev                               |

When `hardConstraints: true`, candidates are sorted primarily by**違規分數**（他們超過任何SLO程度），然後按綜合分數。 Otherwise it's just the composite score.

```ts
class SLAStrategyImpl implements RouterStrategy {
  readonly name = "sla-aware";
  readonly description =
    "Selects the provider most likely to satisfy latency, error-rate, and cost SLOs";

  select(pool, context) {
    // ... scores each candidate against policy: { targetP95Ms, maxErrorRate, maxCostPer1MTokens, hardConstraints }
  }
}
```

**SLA字段**（在組合配置上設定）：

```json
{
  "strategy": "auto",
  "config": {
    "routerStrategy": "sla-aware",
    "slaTargetP95Ms": 1500,
    "slaMaxErrorRate": 0.05,
    "slaMaxCostPer1MTokens": 5,
    "slaHardConstraints": true
  }
}
```

**何時使用**：具有嚴格延遲、錯誤率或成本預算的生產工作負載。

**別名**: `sla-aware`, `sla`

---

#### 5. `lkgp` —最後已知的良好提供者優先

嘗試**最後已知的良好提供者**（如果設定）首先，然後退回到`rules`策略。對於會話黏性很有用—同一提供者處理對話中的後續請求。

```ts
class LKGPStrategyImpl implements RouterStrategy {
  readonly name = "lkgp";
  readonly description = "Tries last known good provider first, then falls back to rules";

  select(pool, context) {
    if (context.lkgpEnabled === false) {
      return getStrategy("rules").select(pool, context);
    }

    if (context.lastKnownGoodProvider) {
      const candidates = pool.filter(
        (c) => c.provider === context.lastKnownGoodProvider && c.circuitBreakerState !== "OPEN"
      );
      if (candidates.length > 0) {
        return { provider: candidates[0].provider /* ... */ };
      }
    }

    // Fallback to rules strategy
    return getStrategy("rules").select(pool, context);
  }
}
```

**何時使用**：多輪對話，您希望同一提供者處理後續請求（例如，為了快取、上下文連續性或定價一致性）。

**別名**： `lkgp` （無別名）

---

#### 6. `nadir` —透過 Nadir 提示感知模型選擇

上述每個策略都根據候選人自己的遙測資料對候選人進行排名； none of them reads the request. `nadir`將最後一個用戶回合加上池的模型 ID 發送給[Nadir](https://getnadir.com)的決策API (`POST /v1/bucket`)，並路由到 Nadir 從該選單中選擇的模型（`simple` →最便宜的模型， `complex` → 。為該模型提供服務的連接仍然由`rules`選擇，因此配額、運行狀況和成本不斷決定哪個帳戶。

```json
{
  "strategy": "auto",
  "config": {
    "routerStrategy": "nadir",
    "nadir": {
      "apiKey": "ndr_...",
      "baseUrl": "https://api.getnadir.com",
      "timeoutMs": 2000
    }
  }
}
```

`OMNIROUTE_NADIR_API_KEY`和`OMNIROUTE_NADIR_BASE_URL`是兩個字串的 env 後備。僅自架最低點需要`baseUrl` （允許尾隨`/v1` ）。無密鑰呼叫位於 Nadir 的匿名層，該層按IP進行速率限制。透過一把鑰匙（[建立一個](https://app.getnadir.com/dashboard/api-keys)），每個決定都會記錄到您的最低點儀表板。 Full setup and verification: [getnadir.com/docs/gateway-omniroute](https://getnadir.com/docs/gateway-omniroute/).

剩下的內容是：最後一條用戶訊息的文字（前 16k 個字元）、候選模型 ID 和`source: "omniroute"`通道標籤。 No system prompt, history, tools or headers.

故障行為是故障開放：逾時（預設 2000 毫秒）、 non-2xx、無法存取的主機、格式錯誤的回應或池外的選擇解析為`rules`決策，原因以`NadirStrategy: fallback (…)`為前綴。呼叫失敗後，該策略會跳過網路 30 秒，因此中斷會導致每 30 秒一次逾時，而不是每個請求一次。只有當 Nadir 實際做出選擇時，路由事件才會報告`strategy: "nadir"` 。

**何時使用**：跨模型層（小型、中型和前沿模型）的池上的混合難度流量，其中始終前沿是您想要削減的成本。

**別名**： `nadir` （無別名）

---

#### 7. `decision` —可插入決策器選擇模型

`decision`問一個**決定者**池中的哪個模型適合請求，然後將池縮小到該模型，並讓`rules`選擇連接（配額、運行狀況和成本仍然選擇帳戶）。當路由器旋鈕位於`config` （儀表板所寫的內容）頂部或`config.auto.routerStrategy`旁邊的`config.auto.decision`時，決策器會在組合的決策區塊— `config.decision`中設定：

| `decider`     | 誰回答                                                                                                  | 需求                                 |
| ------------- | ------------------------------------------------------------------------------------------------------- | ------------------------------------ |
| `systemone`   | TypeSafe系統一（`POST https://api.typesafe.ai/v1/systemone`），預設型號`jev-latest`                     | `typesafe`連接或 env key             |
| `http`        | 您自己的`baseUrl`決策者： `wire: "systemone"` (`{baseUrl}/v1/systemone`) 或`"openai-chat"` （聊天完成） | `baseUrl` + `model`;關鍵可選         |
| `combo-model` | 您的提供者模型之一，像融合法官一樣在過程中呼叫                                                          | `model`為`provider/model` （無組合） |

```json
{
  "strategy": "auto",
  "config": {
    "routerStrategy": "decision",
    "decision": {
      "decider": "http",
      "baseUrl": "https://decider.example.com",
      "wire": "openai-chat",
      "model": "qwen-small",
      "connectionId": "<stored connection id>",
      "timeoutMs": 2000,
      "minConfidence": 0.6,
      "descriptions": { "gpt-4o-mini": "Quick drafts and short answers" }
    }
  }
}
```

欄位（在儲存時透過嚴格模式驗證，並在請求時再次驗證）：

- `decider` — `systemone`、 `http`或`combo-model`。
- `model` — TypeSafe模型、 URL處的決策模型或組合模型所呼叫的`provider/model` （最多 200 個字元）。
- 僅限`baseUrl` — `http` ： `http(s)` URL最多 500 個字符，沒有憑證、查詢或片段。指向此OmniRoute （環回+ `PORT`）的URL被拒絕。
- 僅`wire` — `http` ： `systemone` （預設）或`openai-chat`。
- `connectionId` —使用其金鑰的儲存連線（僅在呼叫API金鑰的允許連線內）。如果沒有它， `systemone`會讀取`typesafe`連接，每個網路決策者都會回退到`OMNIROUTE_DECISION_API_KEY`。沒有`apiKey`欄位：密鑰永遠不會儲存在組合中。
- `timeoutMs` —整數，100–5000，預設 2000。
- `minConfidence` — 0–1；置信度較低的答案會回退到`rules` （報告沒有置信度的決策者計為 0）。
- `descriptions` —最多 50 個條目（密鑰最多 300 個，文字最多 1000 個字元），由型號 id 或`provider/model`鍵入；未設定的條目會獲得產生的成本排名描述。

**旗幟。** `COMBO_DECISION_ROUTER_ENABLED` （預設`false`）控制每個決策者。當它關閉時， `decision`組合不會讀取憑證，不會進行呼叫並使用`rules`進行路由；日誌顯示`fallback (disabled)`。單獨儲存的鑰匙永遠不會打開它。沒有決策塊的組合根本不受影響。

**盒子裡還剩下什麼。**僅最後一則使用者訊息的文字（最多 8000 個字元； chat/Claude `messages`或 Responses `input`）以及模型 ID 選單及其描述。絕不是系統提示、回應`instructions`、工具、歷史記錄、標題或帳戶資料。網路呼叫透過提供者出站防護，無需重試，無需重定向，並且有 64 個KB回應上限。 `combo-model`呼叫是非流式、免工具的`temperature: 0`，預算為 256 個代幣；在決策呼叫中開始的決策被拒絕。

**Failure behavior** is fail-open: any failure resolves to the `rules` decision, and the reason reads `decision(<decider>): fallback (<reason>)`, with `<reason>` one of `disabled`, `not_configured`, `missing_credential`, `timeout`, `http_error`, `invalid_response`, `out_of_menu`, `refused`, `cooldown`, `network_error`, `recursion`, `low_confidence`, `single_option` or `no_user_text`. After a timeout, HTTP error or network error the endpoint is skipped for 30 s. A successful pick reads `decision(<decider>): selected <model> from <n>; confidence <c> (<rules reason>)`. No URL, key, prompt or upstream body reaches the log.

當路由器策略為`decision`時，組合建構器顯示這些字段，並使用產生的描述作為佔位符和**測試決策**使用未儲存的設定呼叫`POST /api/combos/decision-preview`一次的按鈕（相同標誌）。

**何時使用**：混合難度流量，您希望由您選擇的分類器（而不是專門由 Nadir）根據請求選擇層。

**別名**： `decision` （無別名）

---

### 自訂路由器策略

您可以透過公共API註冊您自己的`RouterStrategy`實現：

```ts
import {
  registerStrategy,
  type RouterStrategy,
} from "@omniroute/open-sse/services/autoCombo/routerStrategy";

class MyCustomStrategy implements RouterStrategy {
  readonly name = "my-custom";
  readonly description = "My custom routing strategy";

  select(pool, context) {
    // Your routing logic here
    return {
      provider: pool[0].provider,
      model: pool[0].model,
      strategy: this.name,
      reason: "MyCustomStrategy: ...",
      candidatesConsidered: pool.length,
      finalScore: 1.0,
    };
  }
}

registerStrategy("my-custom", new MyCustomStrategy());
```

然後使用它：

```json
{
  "strategy": "auto",
  "config": {
    "routerStrategy": "my-custom"
  }
}
```

---

### 路由器策略選擇指南

| 使用案例           | 策略        | 原因                     |
| ------------------ | ----------- | ------------------------ |
| 平衡工作量         | `rules`     | 預設—考慮所有因素        |
| 成本最小化         | `cost`      | 總是選最便宜的           |
| 最大限度地減少延遲 | `latency`   | 選擇最快可靠的提供者     |
| 嚴格SLOs           | `sla-aware` | 按p95/error/cost閾值過濾 |
| 多輪聊天           | `lkgp`      | 會話黏性                 |
| 混合難度           | `nadir`     | 根據提示選擇模型層       |
| 自己的分類器       | `decision`  | 您的決策者選擇模型       |

SLA 感知領域：

```json
{
  "strategy": "auto",
  "config": {
    "routerStrategy": "sla-aware",
    "slaTargetP95Ms": 1500,
    "slaMaxErrorRate": 0.05,
    "slaMaxCostPer1MTokens": 5,
    "slaHardConstraints": true
  }
}
```

## 任務適用性

針對 6 種任務類型（`coding`、`review`、`planning`、`analysis`、`debugging`、`documentation`）為 30 多個模型評分。支援萬用字元模式（例如，`*-coder` → 高程式設計分數）。

## 汽車變體回顧

`AutoVariant`在`autoPrefix.ts`聲明**7 個值**（`coding`、 `fast`、 `cheap`、 `offline`、 `smart`、 `lkgp`、 `chaos`）。 Together與裸`auto` （由`parseAutoPrefix()`處理為`variant: undefined`）和兩個平面層覆蓋`auto/subscription`和`auto/thrifty` （ `builtinCatalog.ts`中的`FLAT_TIER_OVERLAY_IDS` ），有**10平款IDs** :

`auto`, `auto/coding`, `auto/fast`, `auto/cheap`, `auto/offline`, `auto/smart`, `auto/lkgp`, `auto/chaos`, `auto/subscription`, `auto/thrifty`

除此之外， `auto/<category>[:<tier>]`組合、模型系列IDs （例如`auto/claude-opus`）和`builtinCatalog.ts`中的`auto/best-*` / `auto/pro-*`別名也可以解析。

## 層級如何融入 Auto-Combo

這個 16 因子評分函式（`open-sse/services/autoCombo/scoring.ts`）將層級歸屬視為兩個訊號：`tierPriority`（0.0476）與 `tierAffinity`（0.0476）。如需完整的 `DEFAULT_WEIGHTS` 設定，請參閱上方的標準[評分因子表](#how-it-works-persisted-auto-combos)；各套件的覆寫設定（ship-fast/cost-saver/quality-first/offline-friendly）則列於「各套件的權重設定檔」表格中。

僅憑層級**不會**強制優先選擇第 1 層級——如果第 1 層級的延遲表現不佳，或成本與品質的取捨並非最佳，第 2 層級就會勝出。若要強制遵循層級順序，請使用組合策略 `priority`，並依層級排列提供者。

若要大幅偏好第 1 層級（訂閱制），請提高 `tierPriority` 的權重：

```json
{
  "strategy": "auto",
  "config": { "auto": { "weights": { "tierPriority": 0.3, "costInv": 0.05 } } }
}
```

如需層級定義與提供者分類，請參閱 [`docs/guides/TIERS.md`](../guides/TIERS.md)。

## 測試和覆蓋範圍

### 確定性路由決策矩陣 (`npm run test:combo:matrix`)

`tests/integration/combo-matrix/*.test.ts`證明路由**決定**它透過真實的組合管道與模擬的上游覆蓋端到端的公共策略。承保範圍包括：

- 22 種公共`ROUTING_STRATEGY_VALUES`策略中的 18 種（有序、加權、成本、上下文、融合…）； `quota-weighted`、 `cache-optimized`、 `pipeline`和`jev`不由矩陣執行，而是依賴它們自己的單元測試。
- `quota-share` （內部）端對端：透過真正的`selectQuotaShareTarget`接縫（`registerQuotaFetcher` / `setLKGP` / `__setHeadroomSaturationFetcherForTests`）進行DRR公平性+飽和度去優先權化。
- `context-relay`通用切換覆蓋每個目標計數。

該套件在CI （`test:integration`作業）中與`--test-concurrency=1`和`--test-force-exit`一起運行，因此它是確定性的，不需要實時憑證。

### 門控現場煙霧（NOT中的CI —真實提供者）

| 命令                                   | 它的作用                                                       |
| :------------------------------------- | :------------------------------------------------------------- |
| `npm run test:combo:live`              | 使用`RUN_COMBO_LIVE=1`進行進程內真實路由；快照即時OmniRoute DB |
| `npm run test:combo:live:vps`          | HTTP呼叫實時OmniRoute伺服器（設定`COMBO_LIVE_BASE_URL`）       |
| `npm run test:combo:live:vps:failover` | 同樣，有故意的故障轉移場景                                     |

這些冒煙測試練習真實的線路路徑（組合→提供者→完成）。他們被有意排除在CI之外，因為他們需要即時憑證和VPS存取權限。

---

## 文件

| 文件                                                      | 目的                                                                         |
| :-------------------------------------------------------- | :--------------------------------------------------------------------------- |
| `open-sse/services/autoCombo/scoring.ts`                  | 16 因素評分函數、 `DEFAULT_WEIGHTS`、池範數                                  |
| `open-sse/services/autoCombo/taskFitness.ts`              | 模型×任務適應度查找                                                          |
| `open-sse/services/autoCombo/engine.ts`                   | 選擇邏輯、強盜、預算上限                                                     |
| `open-sse/services/autoCombo/selfHealing.ts`              | 排除、探測、事件模式                                                         |
| `open-sse/services/autoCombo/modePacks.ts`                | 6 種重量配置（快速運輸、節省成本、品質第一、離線友好、可靠性第一、混沌模式） |
| `open-sse/services/autoCombo/autoPrefix.ts`               | `auto/`前綴解析器+ 6 個變體                                                  |
| `open-sse/services/autoCombo/virtualFactory.ts`           | 從即時連接建立記憶體中的`AutoComboConfig`                                    |
| `open-sse/services/autoCombo/providerRegistryAccessor.ts` | 用於模擬提供者註冊表的測試鉤子                                               |
| `src/shared/constants/routingStrategies.ts`               | `ROUTING_STRATEGY_VALUES` （22個策略）                                       |
| `src/sse/handlers/chat.ts`                                | 整合：自動前綴短路                                                           |
