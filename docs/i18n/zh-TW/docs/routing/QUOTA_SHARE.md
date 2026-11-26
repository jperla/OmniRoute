# Quota Sharing Engine (中文 (繁體))

🌐 **Languages:** 🇺🇸 [English](../../../../routing/QUOTA_SHARE.md) · 🇪🇹 [am](../../../am/docs/routing/QUOTA_SHARE.md) · 🇸🇦 [ar](../../../ar/docs/routing/QUOTA_SHARE.md) · 🇦🇿 [az](../../../az/docs/routing/QUOTA_SHARE.md) · 🇧🇬 [bg](../../../bg/docs/routing/QUOTA_SHARE.md) · 🇧🇩 [bn](../../../bn/docs/routing/QUOTA_SHARE.md) · 🇧🇦 [bs](../../../bs/docs/routing/QUOTA_SHARE.md) · 🇨🇿 [cs](../../../cs/docs/routing/QUOTA_SHARE.md) · 🇩🇰 [da](../../../da/docs/routing/QUOTA_SHARE.md) · 🇩🇪 [de](../../../de/docs/routing/QUOTA_SHARE.md) · 🇬🇷 [el](../../../el/docs/routing/QUOTA_SHARE.md) · 🇪🇸 [es](../../../es/docs/routing/QUOTA_SHARE.md) · 🇪🇪 [et](../../../et/docs/routing/QUOTA_SHARE.md) · 🇮🇷 [fa](../../../fa/docs/routing/QUOTA_SHARE.md) · 🇫🇮 [fi](../../../fi/docs/routing/QUOTA_SHARE.md) · 🇫🇷 [fr](../../../fr/docs/routing/QUOTA_SHARE.md) · 🇮🇪 [ga](../../../ga/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [gu](../../../gu/docs/routing/QUOTA_SHARE.md) · 🇳🇬 [ha](../../../ha/docs/routing/QUOTA_SHARE.md) · 🇮🇱 [he](../../../he/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [hi](../../../hi/docs/routing/QUOTA_SHARE.md) · 🇭🇷 [hr](../../../hr/docs/routing/QUOTA_SHARE.md) · 🇭🇺 [hu](../../../hu/docs/routing/QUOTA_SHARE.md) · 🇦🇲 [hy](../../../hy/docs/routing/QUOTA_SHARE.md) · 🇮🇩 [id](../../../id/docs/routing/QUOTA_SHARE.md) · 🇳🇬 [ig](../../../ig/docs/routing/QUOTA_SHARE.md) · 🇮🇹 [it](../../../it/docs/routing/QUOTA_SHARE.md) · 🇯🇵 [ja](../../../ja/docs/routing/QUOTA_SHARE.md) · 🇬🇪 [ka](../../../ka/docs/routing/QUOTA_SHARE.md) · 🇰🇭 [km](../../../km/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [kn](../../../kn/docs/routing/QUOTA_SHARE.md) · 🇰🇷 [ko](../../../ko/docs/routing/QUOTA_SHARE.md) · 🇱🇹 [lt](../../../lt/docs/routing/QUOTA_SHARE.md) · 🇱🇻 [lv](../../../lv/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [ml](../../../ml/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [mr](../../../mr/docs/routing/QUOTA_SHARE.md) · 🇲🇾 [ms](../../../ms/docs/routing/QUOTA_SHARE.md) · 🇲🇹 [mt](../../../mt/docs/routing/QUOTA_SHARE.md) · 🇲🇲 [my](../../../my/docs/routing/QUOTA_SHARE.md) · 🇳🇵 [ne](../../../ne/docs/routing/QUOTA_SHARE.md) · 🇳🇱 [nl](../../../nl/docs/routing/QUOTA_SHARE.md) · 🇳🇴 [no](../../../no/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [or](../../../or/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [pa](../../../pa/docs/routing/QUOTA_SHARE.md) · 🇵🇭 [phi](../../../phi/docs/routing/QUOTA_SHARE.md) · 🇵🇱 [pl](../../../pl/docs/routing/QUOTA_SHARE.md) · 🇵🇹 [pt](../../../pt/docs/routing/QUOTA_SHARE.md) · 🇧🇷 [pt-BR](../../../pt-BR/docs/routing/QUOTA_SHARE.md) · 🇷🇴 [ro](../../../ro/docs/routing/QUOTA_SHARE.md) · 🇷🇺 [ru](../../../ru/docs/routing/QUOTA_SHARE.md) · 🇱🇰 [si](../../../si/docs/routing/QUOTA_SHARE.md) · 🇸🇰 [sk](../../../sk/docs/routing/QUOTA_SHARE.md) · 🇸🇮 [sl](../../../sl/docs/routing/QUOTA_SHARE.md) · 🇷🇸 [sr](../../../sr/docs/routing/QUOTA_SHARE.md) · 🇸🇪 [sv](../../../sv/docs/routing/QUOTA_SHARE.md) · 🇰🇪 [sw](../../../sw/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [ta](../../../ta/docs/routing/QUOTA_SHARE.md) · 🇮🇳 [te](../../../te/docs/routing/QUOTA_SHARE.md) · 🇹🇭 [th](../../../th/docs/routing/QUOTA_SHARE.md) · 🇹🇷 [tr](../../../tr/docs/routing/QUOTA_SHARE.md) · 🇺🇦 [uk-UA](../../../uk-UA/docs/routing/QUOTA_SHARE.md) · 🇵🇰 [ur](../../../ur/docs/routing/QUOTA_SHARE.md) · 🇺🇿 [uz](../../../uz/docs/routing/QUOTA_SHARE.md) · 🇻🇳 [vi](../../../vi/docs/routing/QUOTA_SHARE.md) · 🇳🇬 [yo](../../../yo/docs/routing/QUOTA_SHARE.md) · 🇨🇳 [zh-CN](../../../zh-CN/docs/routing/QUOTA_SHARE.md)

---

> **文件參考**：`docs/routing/QUOTA_SHARE.md`
> 屬於 B 組（計畫 16 + 22）。

---

## 概述

配額共享引擎會將提供者以時間為基礎的配額（例如 Codex 的
5 小時視窗、Kimi 的 1500 req/h）公平分配給共用相同連線的多個 API 金鑰。

**其解決的問題：** OmniRoute 會透過同一個上游提供者帳戶代理許多 API 金鑰。
若沒有共享邏輯，金鑰 A 突然產生的大量請求可能會耗盡該小時的提供者配額，
導致金鑰 B 和 C 在視窗重設之前都遭到封鎖。引擎透過以下方式避免此問題：

1. 追蹤每個金鑰在各維度（%、請求、權杖、$）的滾動用量。
2. 套用工作守恆的公平份額演算法：只要全域集區尚未飽和，金鑰即可借用閒置份額。
3. 在請求抵達上游執行器之前，於熱路徑（`chatCore.ts`）中強制執行結果。

---

## 演算法：公平分享工作保存

在`src/lib/quota/fairShare.ts`實現。

### 模式

| 狀態                                       | 模式       | 行為                               |
| ------------------------------------------ | ---------- | ---------------------------------- |
| `globalUsedPercent < saturationThreshold`  | **慷慨的** | 密鑰可以藉用至全域限制減去消耗總量 |
| `globalUsedPercent >= saturationThreshold` | **嚴格的** | 嚴格執行個人公平份額               |

預設`saturationThreshold = 0.5` (env `QUOTA_SATURATION_THRESHOLD`)。

這兩種模式描述了預設借用模式`saturation`下的池。無論飽和度如何， `consent`模式下的礦池始終應用嚴格的規則。請參閱[同意借貸（每個池選擇加入）](#consented-lending-per-pool-opt-in) 。

### 按維度決策

對於池中的每個活動維度，引擎計算：

```
fairShareAllowed = poolLimit × (allocationWeight / 100)
consumed        = current rolling value for this key (from QuotaStore.peek)
remaining       = fairShareAllowed - consumed
```

對於`percent`維度， `consumed`來自歸因手冊（請參閱[百分比維度：每鍵歸因](#percent-dimensions-per-key-attribution)）。

然後：

- **`policy = hard`** ：如果`consumed > fairShareAllowed`和模式是嚴格的→**堵塞**。
- **`policy = soft`** ：如果`consumed > fairShareAllowed`和模式是嚴格的→**懲罰**（組合中降低優先權；切勿硬塊）。
- **`policy = burst`** ：無論公平份額如何，都允許存在全球空間。

### 絕對上限

分配上的`capValue` + `capUnit`是獨立於模式或策略的硬性上限。 `consumed >= capValue`始終存在的任何維度**區塊**的請求。對於`percent` cap， `consumed`只是歸屬於密鑰的部分。

### 多維度檢查

請求被阻止，如果**任何**池中的維度會阻擋它。維度是獨立的— 5 小時% 的耗盡不會影響每週% 維度。

### 借款

在慷慨模式下，分配未充分消耗的密鑰可以使用其他密鑰未分配份額的剩餘部分。公式為：

```
maxAllowed = globalLimit - consumedByOtherKeys
```

哪裡`consumedByOtherKeys = consumedTotal - consumedByThisKey`. teto 全域（該維度的`limit`池）總是硬上限。

### 同意貸款（每個池選擇加入）

每個池都有借用模式。 `saturation`是預設值並保留上述規則。在`consent`模式下， `hard`密鑰僅在其他密鑰同意借出的容量內傳遞其份額。管理員設定每個池的模式。每個密鑰持有者透過[貸款同意](#lending-consent)來設定自己的同意。

同意是從 0 到 100 的百分比以及以紀元毫秒為單位的可選截止日期。當截止日期在未來時，密鑰會借出該比例的閒置份額。

對於一個維度， `L`是有效限制：計劃限制乘以池中的帳戶。閘針對請求金鑰計算：

```
share_k         = w_k / 100 × L
idle_k          = max(0, share_k − consumed_k)
lent            = Σ over the other keys of lend_k / 100 × idle_k
taken           = Σ over the other keys of max(0, consumed_k − share_k)
borrowAvailable = max(0, lent − taken)
```

`w_k` is the key's weight, or `100 / n` for every key when no weight is above 0. `lend_k` is the key's active percentage, and 0 once its deadline has passed. The requesting key's own consent never counts. A `hard` key is refused once its consumption reaches its share plus `borrowAvailable`.

沒有分配要求的容量（100 減去權重總和）不可出借。沒有鑰匙同意借給它。

**例子。** `L`是1000。

| 鑰匙 | 重量 | 分享 | 已消耗 | 倫茲 |
| ---- | ---- | ---- | ------ | ---- |
| 一個 | 50   | 500  | 530    | 0%   |
| 乙   | 30   | 300  | 100    | 50%  |
| C    | 0    | 0    | 60     | 0%   |

- B 借出其閒置 200 美元中的 50%，即 100 美元。 C 已在其份額上多藉了 60 美元。 A可以藉40。
- A 的服務金額為 530，一旦消費達到 540，則被拒絕。
- 在 C 使用任何東西之前，如果 A 等於或低於其份額，C 可以藉 100。
- 在 C 使用任何東西之前，A 的金額為 530，C 可以藉用 70。

**零重量。**權重為 0 的密鑰的份額為 0。僅當其消耗量低於其他人借出的量時才提供服務。當沒有人借出時，它從第一次請求就被拒絕。

**截止日期。**沒有後台任務會使同意過期。每個請求都會將截止日期與自己的時間進行比較，並且等於該時間的截止日期已經過去。如果儲存的截止日期不是有限的數字，或超過了`Date`可以保存的最大日期，則視為已通過。

**`soft`和`burst`。**貸款並不限制他們。一旦超過其份額， `soft`密鑰就會被取消優先權。當泳池還有空間時， `burst`鑰匙就會通過。一旦池的總數達到其限制，池上限仍然拒絕每個密鑰。

**請求路徑上的成本。** `saturation`池的讀取內容與以前沒什麼不同。在`consent`池中，可數維度僅讀取等於或高於其份額的`hard`密鑰的其他密鑰，而另一個密鑰則借出。然後，它並行地對每個其他鍵進行一次讀取。讀取失敗算該鍵的消耗為 0。 `percent`維度不會增加任何讀取，因為歸屬簿包含所有金鑰。

**編輯池。**編輯會保留保留密鑰的同意。這適用於分配編輯、群組範圍內的替換和`ensure`呼叫。刪除的密鑰將失去其同意，並且添加回來的密鑰從 0 開始。管理路由傳回每個金鑰的同意並且從不寫入它。將池切換回`saturation`會保留所有儲存的同意，這在該模式下不起作用。再次將池切換到`consent`會重新啟動尚未超過截止日期的儲存同意。密鑰持有者可以在任一模式下清除儲存的同意。

**升級中。**如果列`lending_percent`和`lending_until`已存在，則遷移僅添加`borrow_mode`，並且儲存的百分比保持原樣。每個池都以`saturation`模式啟動。在池精靈中為每個池開啟`consent` 。不會從儲存的值推斷出任何內容。

**局限性。**

- 貸方可以在使用自己的份額之前發現資金池已達到上限。其他人借用的容量計入池的總量。
- 檢查在請求之前運行並且不保留任何內容。並發請求在記錄任何消耗之前讀取消耗，因此借出的容量可以多次使用，但受運行中請求的限制。 `saturation`模式的共享檢查具有相同的屬性。

---

## 滑動視窗計數器

實作於 `src/lib/quota/sqliteQuotaStore.ts` 和 `redisQuotaStore.ts`。

每個 `(apiKeyId, dimensionKey)` 有兩個分桶：

- `curr`：目前分桶（`floor(nowMs / windowMs)`）
- `prev`：前一個分桶（`curr - 1`）

有效滾動值：

```
effectiveBucketIndex = floor(nowMs / windowMs)
bucketStartMs        = effectiveBucketIndex × windowMs
elapsed              = nowMs - bucketStartMs
weight               = 1 - elapsed / windowMs

effective = prev × weight + curr
```

**精確度**：準確度約為 99%。在分桶邊界處，誤差最多為視窗大小的 1%
（這是雙分桶近似法的固有限制）。

### 並行處理

SQLite 驅動程式：針對每個 `(apiKeyId | dimensionKey)` 金鑰使用記憶體內互斥鎖，
以避免讀取－修改－寫入競爭。此模式仿照 `src/sse/services/auth.ts` 的防驚群機制。

Redis 驅動程式：使用 Lua EVAL 指令碼進行不可分割的遞增操作——以單一 Redis 命令執行。

---

## 驅動程式

### SQLite（預設、免安裝）

- 資料表：`quota_consumption`（請參閱遷移檔案 `073_quota_pools.sql` / `074_quota_consumption.sql`）。
- 最適合單一執行個體部署。
- 所有持久化資料皆儲存在現有的 OmniRoute SQLite DB（`DATA_DIR/storage.sqlite`）中。

### Redis（選用、多執行個體）

- 需要 `ioredis` npm 套件。
- 計數器儲存在 Redis 中；中繼資料（資源池／配額分配）仍儲存在 SQLite 中。
- 最適合需要共用計數器的多副本部署。

### 切換驅動程式

透過設定 UI（`/dashboard/settings` → 配額儲存區），或透過環境變數：

```bash
QUOTA_STORE_DRIVER=redis
QUOTA_STORE_REDIS_URL=redis://localhost:6379
```

DB 設定的優先順序高於環境變數。若 `driver=redis` 但未提供 URL，或未安裝
`ioredis`，工廠會回退至 SQLite 並記錄警告。

驅動程式選擇順序：

1. DB 設定 `quotaStore.driver`
2. 環境變數 `QUOTA_STORE_DRIVER`
3. 預設：`sqlite`

---

## 多維度

池可以有多個維度。每個維度都是獨立的：

```ts
QuotaDimension {
  unit: "percent" | "requests" | "tokens" | "usd",
  window: "5h" | "hourly" | "daily" | "weekly" | "monthly",
  limit: number,  // global pool ceiling for this dimension
}
```

**範例： Codex計劃**（5h% +每週%）：

```json
[
  { "unit": "percent", "window": "5h", "limit": 100 },
  { "unit": "percent", "window": "weekly", "limit": 100 }
]
```

請求必須滿足所有允許的尺寸。

### 維度百分比：每鍵歸因

百分比計劃會報告每個帳戶和計劃視窗的一個使用資料。提供者沒有為每個API金鑰提供計數器。

為了在密鑰之間分配該數字，每個池為每個帳戶和計劃視窗保留一個歸屬簿。 `src/lib/quota/percentLedger.ts`持有本書的規則。 `src/lib/quota/percentAttribution.ts`將書本轉化為執法部門使用的數字。結果是根據每個關鍵路線的令牌構建的估計。

#### 感動書籍的讀物

該書僅在所請求的計劃視窗的提供者自己的數字上移動。這些連接報告一：

| 提供者                | 規劃窗戶       |
| --------------------- | -------------- |
| Claude，透過OAuth連接 | `5h`, `weekly` |
| Codex                 | `5h`, `weekly` |

這些不算閱讀：

- 提供者客戶端標記為過時的回應
- 提供者未報告其百分比的Claude窗口
- 另一個視窗的數字，或是跨窗口的最壞情況
- 速率限制標頭回退
- 讀取失敗

其他提供者，包括帶有API密鑰的Claude ，都沒有書籍。與此變更之前一樣，每個按鍵的百分比尺寸均按 0 收費。

一次讀數共享飽和訊號的 30 秒快取。 Claude讀數的日期是在回應標頭中觀察到該數字或從使用端點讀取該數字（當該時間已知時）的日期。其他讀數的日期是該快取條目的建置時間。

#### 本書保留了什麼

每個記錄的請求都會將其令牌一次新增到每個池、帳戶和金鑰的計數器中。計數器只會增長。書中保留了三件事：

- 基線：書本開啟或視窗上次開啟時的數字
- 最後應用的數字
- 每個鍵，同一時刻的令牌計數器稱為其標記

當執行或使用路徑計算歸屬時，本書會更新。寫入是根據修訂號進行比較和設定的。一個作家在重新閱讀一次時失敗了。

#### 鍵的部分是如何計算的

每個鍵的部分都是在閱讀本書時計算的。自基線以來數字的增長在鍵之間按比例分配，每個鍵自其標記以來路由的令牌成比例。

Together，這些標記最多解釋每個`QUOTA_PERCENT_MIN_TOKENS_PER_POINT`標記中的一個點（預設 1,000）。他們沒有解釋的成長是外在的。基線也是外部的。

例如，一本書在 0 點打開。然後密鑰 A 路由 900,000 個令牌，密鑰 B 路由 100,000 個令牌。數字為 60 時，A 部分為 54 分，B 部分為 6 分。

低於其鑰匙標記的計數器已重新啟動並完整計數。沒有標記的金鑰，例如在視窗中間加入池的金鑰，會計算其所有令牌。落後於標記的數字會導致錯誤，該錯誤會在下次讀取時消失。它不會累積。

每個屬性都會閱讀`QUOTA_PERCENT_MIN_TOKENS_PER_POINT` 。不是至少 1 的有限數的值會回落到 1,000。

#### 閱讀如何改變書本

第一個符合規則適用：

1. **還沒有書：**閱讀打開書本。它的數字是基線，每個計數器都被標記。
2. **較舊的閱讀：**上次施加的讀數之前的讀數將被忽略。重置時間比儲存時間早 30 分鐘以上的讀數也是如此。
3. **新的提供者視窗：**重置時間比儲存的翻書時間晚30分鐘以上。該數字成為基線，並且每個計數器都再次標記。沒有櫃檯的鑰匙離開書本。
4. **結束視窗：**儲存的複位時間不在讀數資料時間之後意味著該視窗已結束。無論書的內容如何，閱讀都會改變書的內容。
5. **更高的數字：**只有最後一個人影在動。基線和標記保持不變。
6. **同圖：**圖形、基線和標記保留。只寫了書中缺少的重置時間。
7. **下圖：**永遠不會應用較低的數字。只有當三件事成立時，這本書才會翻過來。它比上次應用的讀數至少晚兩分鐘。沒有任何跡象表明窗戶是同一個打開的窗戶。低了不止一分。

當三件事成立時，該視窗就被視為同一扇打開的視窗。兩個重置時間都是已知的。兩者相距不到 30 分鐘。儲存的仍領先於讀取。該視窗內較低的數字沒有任何變化。

僅當復位時間早於攜帶該重設時間的讀數的資料時間時，才會儲存重設時間。當該讀數可用時，較高的數字會儲存其讀數的重置時間，否則保留儲存的讀數。只有當書籍沒有時，相同的數字才會記錄其閱讀的重置時間。它沒有改變其他任何東西。不翻書的下圖記錄了沒有重置的時間。

#### 當書被使用時

閱讀後，除非其儲存的重置時間不晚於當前時間，否則將使用該書。當在重設之前讀取的讀數（例如從快取提供的讀數）在重設之後觀察到時，就會發生這種情況。

如果沒有可用的閱讀，則僅當儲存的書籍仍然是當前視窗的書籍時才使用它。這在兩種情況下成立：

- 它的重置時間是已知的並且仍然領先
- 它沒有重置時間，並且最後一次更改它的讀數最多為 15 分鐘

否則就沒有任何歸屬，就像沒有書一樣。儲存的重置時間已過的書籍永遠不會收費。

#### 執行

密鑰在百分比維度上的消耗是其歸屬部分加上外部部分的份額。外部部分首先使用未分配聲明的容量（100 減去權重總和）。只有多餘的部分按重量在按鍵之間共用。

對於任何其他維度，將該消耗與密鑰的公平份額進行比較。當飽和訊號達到`QUOTA_SATURATION_THRESHOLD` （預設0.5）時，嚴格模式仍然啟動。每個數字都以有效限制進行縮放：每個帳戶的限制乘以池中的帳戶數量。

`capUnit: "percent"`的絕對上限僅計算歸因於金鑰的部分，並以相同的方式縮放。每個帳戶的限制為 100 個和 k 個帳戶。當服務帳戶的金鑰部分達到N/k點時，就達到 N 的上限。每個帳戶都會依照自己的帳簿進行檢查。例如，對於兩個帳戶，一個帳戶數字的 5 個點達到 10 的上限。

當無法讀取儲存時，不會對任何內容進行歸因，且每個鍵在該維度上的費用為 0。當一本書寫入失敗時，該歸屬將使用該書被閱讀時的狀態。失敗的令牌寫入會將該請求的令牌從記錄中刪除。這些失敗都不會阻止請求。

在`consent`池中，借貸公式使用每個金鑰在百分比維度上的消耗，如上所述。當另一把鑰匙借出時，這本書會被讀一次並歸屬於每把鑰匙。如果沒有可用的書，每把鑰匙的費用都是 0。然後，一把有重量的鑰匙就可以通過，而重量為 0 的鑰匙只有在另一把鑰匙借出時才可以通過。

#### 使用路線

`GET /api/quota/pools/{id}/usage`透過相同的函數報告相同的數字。百分比維度在`accounts`中的每個池連接有一個條目。其頂級`consumedTotal`和`perKey`鏡像第一個條目。

該路線也應用當前閱讀，因此它可以根據請求推進書籍。當沒有可用讀數或未應用較低的數字時， `internal + external`可能與`consumedTotal`不同。

#### 儲存和保留

兩家配額商店都保留了這本書。在SQLite上，自動資料庫清理在啟用後會刪除 60 天未更新的行。在Redis上，池連接的書籍和計數器共享一個金鑰。它在最後一次代幣寫入或帳簿更改後 60 天到期。不改變的書不會被重寫，因此截止值設定在最長計畫視窗之上。手動使用歷史重置也會清除SQLite上的書籍（請參閱限制）。

#### 限制

- 自基線以來帳戶數字的所有增長均按此後每個密鑰路由的代幣劃分。這種成長何時發生並不重要。
- 因此，在OmniRoute之外進行的使用將根據密鑰的令牌允許的情況進行收費。這包括在鑰匙第一次請求視窗之前、當書籍已經打開時進行的使用。
- 例如，在沒有關鍵路線的情況下，外部使用可提高帳戶60點。然後一個密鑰路由 30,000 個令牌，這個數字達到 60.6。
- 如果該書在使用前已打開，則鑰匙部分為 30 點。它還附帶7.65的外部使用，有四個重量為25的按鍵。
- 如果該書在使用後打開，則 60 分是基線。鑰匙部分為0.6分，承載15分的外部使用。
- 請求或訪問使用路線即可打開這本書。因此，這種使用是否算是基線取決於書的開啟時間。
- 在預設下限的情況下，在外部使用時路由 60,000 個代幣的金鑰會使帳戶增加 60 點，將所有 60 點作為自己的部分。
- 下限為50,000，其自身部分為1.2分。其他 58.8 是外部使用，按重量計費，就像任何外部使用一樣。
- 將`QUOTA_PERCENT_MIN_TOKENS_PER_POINT`設定為接近您計劃中的一分成本。外部使用包括來自池外金鑰的同一帳戶上的流量。
- 百分比上限適用於每種模式。當帳戶遠低於飽和閾值時，可以拒絕有上限的金鑰。
- 在視窗早期將外部使用點數限制為 10 點和 12 點。然後，路由 20,000 個代幣的金鑰在帳戶數字為 12.4% 時被拒絕。
- 分割是按代幣數量進行的估計。請求計為提示令牌加上完成令牌。快取折扣和型號價格不會改變該計數。
- 未以狀態 200 結束的請求不會記錄任何令牌。例如客戶端斷開連接的流以及消耗使用後的上游錯誤。
- 此類請求所引起的使用量將記入記錄令牌的金鑰，最多可達其令牌允許的範圍。其餘的都是外在的。它不會向後移動。報告沒有令牌使用情況的回應也不會記錄任何令牌。
- 正在進行的請求的使用可以顯示在整個請求的另一個活動金鑰的部分中。只有當請求以狀態 200 結束時，它才會移回。
- 開啟圖書時帳戶上已存在的使用情況算作外部使用。這包括升級、新池和新帳戶。在第一次閱讀之前在新視窗中使用也算作外部。
- 每個密鑰都以其在該使用中的權重份額開始，在容量之後沒有分配聲明。一個帳戶的使用率為 85%，五個密鑰的權重為 20，每個密鑰一開始就使用了 20 個密鑰中的 17 個。
- 在具有多個帳戶的池中，服務帳戶的數字將應用於總預算。本書對此沒有改變。
- 不應用提供者報告為開啟的視窗內的較低數字。向後移動超過 30 分鐘的重置時間將被視為舊讀數。
- 在這兩種情況下，書籍都會保持其狀態，直到儲存的重置時間過去。此後，直到閱讀完成後，書籍才會收費。
- 補救措施是手動重置使用歷史記錄 (`POST /api/settings/purge-usage-history`)。它清除SQLite資料庫中的歸屬簿及其令牌計數器。
- `all`期間清除所有書籍和櫃檯。較短的時期首先清除其中未寫的書籍。然後，它會清除未寫入其中的計數器，但僅限於沒有剩餘書籍的池連接。保存的書仍然在櫃檯上標記每個鑰匙。
- 人物沒有移動的書不會被重寫，所以更短的時間也可以清除目前視窗的書。下一次閱讀將以當前數字打開一本新書。
- 重置不會觸及Redis配額儲存。一本書以其視窗結束，或在最後一次寫入後 60 天到期。
- 當提供者沒有發送重置時間時，在兩次讀數之間重置並重新填充到舊數字之上的視窗看起來像是更高的數字。這本書保留了舊的基線和標記。
- 讀數以當地時鐘為準。當它運行得比提供者的時間早，或消息來源報告重置時間稍早時，本書可以提前發現該差異。
- 這段短暫的時間裡的成長被其中路由的代幣分割。下一個視窗的第一個讀數會修正它。當翻過的書沒有重置時間時，該校正需要比上次應用的讀數至少晚兩分鐘的較低數字。
- 共享Redis實例使用自己的時鐘儲存日期讀數，因此請保持這些時脈同步。時鐘落後的實例的讀數看起來較舊並且被忽略。
- 如果在儲存的重置時間之後沒有可用的讀數到達，則在讀數返回之前不會強制執行每個按鍵的百分比份額和百分比上限。如果沒有重置時間，則從上次閱讀更改書籍的 15 分鐘後開始。
- 在Redis商店中，閒置 60 天的書籍可能會在作者檢查和寫入之間過期。然後以高於 1 的修訂版重新建立它，這是一個有效狀態。

---

## 方案解析器

實作於 `src/lib/quota/planResolver.ts`。

優先順序（由高至低）：

1. **手動 DB 覆寫** — `provider_plans` 資料表，依各個 `connectionId` 設定。
2. **已知目錄** — `src/lib/quota/planRegistry.ts`（僅資料）。
3. **空白方案** — 無維度，需要手動設定。

### 已知目錄

| 提供者                | 維度                                                          |
| --------------------- | ------------------------------------------------------------- |
| `codex`               | `percent/5h/100`, `percent/weekly/100`                        |
| `glm`                 | `tokens/5h`（limit=0，未知）、`tokens/weekly`                 |
| `minimax`             | `tokens/5h`, `tokens/weekly`                                  |
| `bailian`             | `percent/5h/100`, `percent/weekly/100`, `percent/monthly/100` |
| `kimi`                | `requests/hourly/1500`                                        |
| `alibaba`             | `requests/monthly/90000`                                      |
| `openai`, `anthropic` | 無預設值 — 需要手動設定                                       |

---

## 管道整合

### PRE鉤子 (`open-sse/handlers/chatCore.ts`)

在身份驗證和策略檢查之後，在上游執行器之前運行：

```
resolveComboTargets / handleSingleModel
  → enforceQuotaShare(apiKeyId, connectionId, provider, estimatedCost)
      → getQuotaStore().peek() per dimension
      → fairShare.decideFairShare()
      → if block → return 429 (buildErrorBody, Hard Rule #12)
      → if allow + deprioritize → set quotaSoftPenalty=true on candidate
  → executor.execute()
```

**失效開放**：如果`enforceQuotaShare`拋出異常，則允許該請求通過`pino.warn`日誌。這可以防止配額引擎錯誤阻止所有流量。

**當容量恢復時。**在兩種借用模式下，對密鑰份額或池上限的拒絕均以以下兩個句子之一結束：

- `percent`視窗： `. The <window> window resets at <time>.`該時間是提供者報告的重置時間。
- 可計數單位： `. Enough <window> usage is expected to clear by <time>.`如果密鑰沒有發送任何其他內容，則時間是滑動視窗的上限。

`<time>`是UTC中的ISO 8601 瞬間。然後拒絕攜帶`Retry-After`：直到那一刻的整秒，加上一。等待那麼長時間的客戶端最多會在該時刻後一秒重試。當未知時刻時，拒絕既不攜帶句子也不攜帶標題。絕對的上限拒絕不會帶來任何影響。公共代碼仍然是`quota_share_blocked`。

共享拒絕不會影響共享連線。它沒有設定冷卻時間，沒有模型鎖定，也沒有提供者斷路器故障，並且池中的其他密鑰將繼續服務。當組合的每個目標都拒絕其共享的金鑰時，組合將立即回答 429。它的答案帶有`Retry-After`提示。嵌入路徑以相同的句子結束其拒絕，並且不發送`Retry-After`。

### POST hook（記錄消費）

成功回應後：

```
executor returns success
  → spendRecorder.recordConsumption(apiKeyId, connectionId, provider, actualCost)
      → getQuotaStore().consume() per dimension
      → fail-open: errors logged as pino.warn, never propagated to client
```

**漂移音符**：如果`consume`後回應失敗，則滾動計數器計數不足。來自提供者（例如`anthropic-ratelimit-unified-5h-utilization`）的飽和訊號修正下一個請求的全域估計。

### 組合軟懲罰 (`open-sse/services/combo.ts`)

當`decision.deprioritize === true`時：

```ts
if (candidate.quotaSoftPenalty) {
  score *= QUOTA_SOFT_DEPRIORITIZE_FACTOR; // default 0.7
}
```

處罰是在所有其他評分因素之後進行的。它降低了選擇飽和密鑰的自動組合機率，而無需對其進行硬阻止。

---

## UI演練

### `/dashboard/costs/quota-share` —主池頁面

組件（全部在`src/app/(dashboard)/dashboard/costs/quota-share/`）：

| 成分                   | 目的                                                 |
| ---------------------- | ---------------------------------------------------- |
| `QuotaConceptCard`     | 向新用戶解釋配額共享的介紹卡                         |
| `CreatePoolModal`      | 建立一個新的配額池（連接+名稱+初始分配）             |
| `PoolCard`             | 每個池的摘要：名稱、連線、分配計數                   |
| `DimensionBar`         | 每維堆疊條：每個鍵所佔+全域使用量                    |
| `AllocationTable`      | 包含已消耗、公平份額、 deficit/surplus、借用標誌的表 |
| `BurnRateChart`        | EMA燃燒率折線圖（透過`dynamic()`進行惰性 Recharts）  |
| `EditAllocationsModal` | 編輯池的分配權重、上限和策略                         |
| `BorrowModeField`      | 精靈中的借用模式選擇器（`saturation`或`consent`）    |
| `LendingBadge`         | 借出金鑰上的唯讀徽章，僅在`consent`池中              |

貸款徽章顯示百分比以及設定後的UTC中的截止日期以及指定的區域。它在使用快照時判斷截止時間。已過期或無法讀取的截止日期顯示為`lending expired`。

頁面掛鉤：

- `usePools` —每 30 秒取得一次`GET /api/quota/pools` 。
- `usePoolUsage` —按需取得`GET /api/quota/pools/[id]/usage` 。
- `useLocalStoragePoolMigration` —在掛載時運行一次以遷移舊的LS資料。

池嚮導的關鍵步驟有一個`Show usage by member to key holders`框。它設定池的`memberBreakdown`選項（請參閱[成員使用](#member-usage)）。在其下方，嚮導警告知道使用哪個鍵的人可以將條形與該鍵匹配。勾選該方塊後，當該步驟列出的鍵少於 3 個或多於 20 個時，它會這樣顯示，因為條形圖將保持隱藏狀態。它會對步驟中的鍵進行計數，但無法判斷哪些按鍵可以發出請求。

### `/dashboard/costs/quota-share/plans` —提供者計畫配置

- `ProviderPlanConfigClient.tsx`：用於選擇提供者、檢視已解析計畫（從目錄自動或手動覆寫）以及編輯維度的下拉清單。
- 更改寫入`PUT /api/quota/plans/[connectionId]`。
- 刪除將恢復為目錄或空白計劃。

---

## 自助服務配額API （選擇加入）

`GET /api/v1/me/quota/{provider}` （也在`/v1/me/quota/{provider}`提供服務）讓API金鑰持有者使用自己的金鑰讀取共享訂閱的數量以及阻止他們的內容。該路由是`src/server/selfService/quotaHandler.ts`上的一個薄殼；該視圖由`src/lib/quota/selfView.ts`構建，其回應合約是`src/shared/schemas/selfQuota.ts` （ `docs/openapi.yaml`中的`SelfQuotaView` ）。

### 啟用和身份驗證

- 功能標誌`QUOTA_SELF_PANEL`，預設`false`。當它關閉時，到達路由的請求會收到 404。使用`REQUIRE_API_KEY=true`時，客戶端API策略會在路由運行之前拒絕遺失或無效的金鑰，並傳回 401，無論標誌為何。沒有金鑰但已登入儀表板會話的請求會通過該策略並取得路由自己的答案。該標誌像其他標誌一樣解析（儀表板或REST覆蓋，然後是同名的環境變數）；參見[`FEATURE_FLAGS.md`](../reference/FEATURE_FLAGS.md) 。
- 每個池的顯示名稱和每個計劃的標籤均按照管理員編寫的內容傳回給池的密鑰持有者。在打開標誌之前，請檢查它們是否適合那些鑰匙持有者讀取。
- 密鑰僅從標頭讀取： `Authorization: Bearer <key>`或`x-api-key: <key>`。當兩者都發送時，使用第一個驗證的。查詢字串或 cookie 中的鍵將被忽略。伺服器的環境密鑰被拒絕 (401)。
- 密鑰需要`self:usage`範圍（403 沒有它）。
- 提供者段被修剪、小寫並根據`^[a-z0-9][a-z0-9._-]{0,63}$`檢查（否則為 400），然後透過提供者註冊表進行解析，因此`cc`等別名會讀取`claude`池。 `claude`和`anthropic`讀取相同的池。

### 每個可見性顯示什麼

| 能見度   | 需要                                                                            | 領域                                                                                                                                                                                                                       |
| -------- | ------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 自己分享 | `self:usage`                                                                    | `pools[]` （ref、名稱、提供者、策略、權重、上限）、 `dimensions[].yourShare`、 `accounts[]`和`yourShare` （在沒有`attributed`和`external` `percent`視窗上）、 `blocks`、 `availableModels`、 `expiresAt`、 `apiBaseUrl`    |
| 帳戶等級 | `self:usage` + `self:account-quota`，以及金鑰的`sharedQuotaProviders`中的提供者 | 在`percent`視窗的`yourShare`上新增`dimensions[].total`、 `accounts[].dimensions[].account`和`accounts[].modelWindows`、 `attributed`和`external` ，並在成員使用開啟的池上新增`members` （請參閱[成員使用](#member-usage)） |

- `sharedQuotaProviders`是每個金鑰的設定 (`PUT /api/keys/[id]/self-service`)： `null`是預設值，表示金鑰到達的每個提供者； `[]`意思是沒有。每個池的`accountVisible`都會說明適用於它的可見性。
- 僅針對金鑰可能使用其連線的帳戶顯示帳戶列和模型視窗。當金鑰具有允許的連線清單時，其外部的帳戶將保留其`Account N`條目，而無需`account`或`modelWindows`。空列表意味著沒有限制，就像`/v1/me/status`一樣。池總數 (`dimensions[].total`) 不依賴該清單。
- 單獨使用`self:usage`顯示的兩個數字來自其他密鑰的使用。計劃預算的`exhausted`反映了該計劃下每個按鍵的消耗。在權重全為零的池中，密鑰的`weight`為`100 / number of members`。兩者都是應用於金鑰的強制執行。
- A pool is identified only by `ref`, an opaque value bound to the calling key. Its display name (`name`) is included as the administrator wrote it. A `ref` is derived from the key and the pool with the server's API-key secret (`API_KEY_SECRET`). Clients must not persist it: it changes if that secret is rotated.
- 帳戶依池順序列出為`Account 1`、 `Account 2`、...。不會傳回池 ID、連線 ID、帳戶電子郵件或帳戶名稱，且回應會通過合約架構，從而刪除合約架構以外的任何欄位。
- 可數單位（`requests`、 `tokens`、 `usd`）被報告為配額門強制執行的池存儲桶− `limit` =計劃限制池中的×帳戶， `fairShare` =權重= `fairShare` × `limit` （當每個權重為 0 時均等）， `remaining` `consumed` = `consumed`為 0。
- `blocks.schedules`列出密鑰的調度視窗（`open`/`closed`、 `blackout`或`outside-window`、 `retryAfterSeconds`、保留樓層以及是否花費視窗預算）； `blocks.modelCaps`列出了每個模型的每小時上限和消耗量。
- 提供者每個池之外的金鑰透過`pools: []`獲得 200 ； `availableModels` （金鑰在`/v1/models`中看到的`qtSd/` id）、 `expiresAt`和`apiBaseUrl`仍然已填入。
- `apiBaseUrl`是`OMNIROUTE_PUBLIC_API_BASE_URL`，然後`OMNIROUTE_PUBLIC_BASE_URL`，否則是`null`。它絕不是請求本身的來源。

### `status`和`reason`

| `status`      | 意義                                                                                                                                                                                                               |
| ------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `ok`          | 當前讀數。                                                                                                                                                                                                         |
| `stale`       | 快取的帳戶讀取標記為過時，或自讀取後重置時間已過。數字被保留。一個重置時間已過的模型視窗標記整個`modelWindows`組`stale`。對於金鑰自己共享的`percent`視窗：這本書是在沒有帳戶讀取門的快取中進行確認的情況下讀取的。 |
| `unavailable` | 不讀書；數字是`null`，而不是`0`。 `reason`說為什麼。                                                                                                                                                               |

| `reason`                          | 什麼時候                                                                        |
| --------------------------------- | ------------------------------------------------------------------------------- |
| `store_unavailable`               | 無法讀取配額存儲，或無法讀取歸屬簿。                                            |
| `percent_attribution_unavailable` | 密鑰自己的`percent`視窗共用：該帳戶和視窗尚不存在歸屬簿，或該歸屬簿未列出密鑰。 |
| `percent_window_ended`            | 關鍵自己的`percent`窗口份額：這本書屬於一個已經結束的計劃窗口。                 |
| `account_not_used_by_key`         | 金鑰自己的`percent`視窗共用：帳戶的連線超出了金鑰允許的連線範圍。其書未讀。     |
| `window_not_reported`             | 提供者限制快取沒有讀取該計劃視窗。                                              |
| `connection_lookup_failed`        | 無法讀取帳戶的連線。                                                            |
| `not_supported`                   | OmniRoute無法讀取帳戶提供者的使用限制。                                         |
| `fetch_failed`                    | 沒有可用的快取讀取，並且提供者限制刷新失敗。                                    |
| `not_available`                   | 讀數沒有使用窗口，或者帳戶根本沒有讀數。                                        |

當無法讀取配額儲存時， `blocks`的儲存支援欄位（計畫預算的`exhausted`、模型上限的`consumed`和`reached`）也是`null` 。

### 貸款同意書

`PATCH /api/v1/me/quota/{provider}`記錄呼叫密鑰自己對一個池的同意。它使用`GET`的標誌、標頭和提供者規則。 `self:usage`作用域授權此寫入，儘管其名稱讀取為唯讀。

```json
{
  "pool": "qpr_0123456789abcdef0123456789abcdef",
  "lendingPercent": 30,
  "lendingUntil": 1893456000000
}
```

- `pool`是`ref`為該池傳回的`GET` 。
- `lendingPercent`是 0 到 100 之間的整數。值為 0 會清除同意及其截止日期。任一模式都接受`lendingPercent` 0 的主體。
- `lendingUntil`是可選的：紀元毫秒，或`null`沒有截止日期。它必須是未來且最多 8640000000000000。低於 100000000000 的值讀取為秒並被拒絕。
- 任何其他欄位都會被拒絕。超過 4096 位元組的正文將被拒絕。讀取在該大小處停止，因此較長的正文永遠不會保持完整。

檢查按此表的順序運行。每次拒絕都使用帶有固定訊息的標準錯誤主體。如果其中一項支票被拒絕，則不會產生任何影響。

| 地位 | 訊息                                                                                               | 什麼時候                                          |
| ---- | -------------------------------------------------------------------------------------------------- | ------------------------------------------------- |
| 404  | `Not found`                                                                                        | `QUOTA_SELF_PANEL`標誌已關閉。                    |
| 401  | `Valid API key required`                                                                           | 密鑰遺失或無效，或伺服器的環境密鑰。              |
| 403  | `API key lacks the self:usage scope`                                                               | 關鍵缺少`self:usage`。                            |
| 400  | `Invalid provider`                                                                                 | 提供者段無效。                                    |
| 429  | `Too many lending changes. Retry later.`                                                           | 鑰匙已經超過極限了。答案是`Retry-After`。         |
| 400  | `Body must be { pool, lendingPercent, lendingUntil }. lendingPercent is an integer from 0 to 100.` | 正文不是JSON、太長或與架構不符。                  |
| 400  | `lendingUntil must be a Unix time in milliseconds`                                                 | 截止日期以秒為單位。                              |
| 400  | `lendingUntil must be in the future`                                                               | 截止日期為請求時間或之前。                        |
| 404  | `Pool not found`                                                                                   | `ref`並未為該提供者指定該金鑰的池。               |
| 403  | `Lending is not enabled for this pool`                                                             | 池處於`saturation`模式， `lendingPercent`大於 0。 |
| 500  | `Failed to build quota view`                                                                       | 任何其他失敗。其原因已記錄在伺服器上。            |

每個金鑰的限制為每 60 秒 20 個請求。透過提供者檢查的每一個請求都很重要，即使是後來拒絕的請求或沒有任何改變的請求。除了金鑰的請求速率限制之外，它還有自己的計數器。

更改儲存同意的請求會寫入一條`quota.pool.lending.updated`審核記錄。它用舊值和新值命名鍵。同一個主體發送兩次，一次寫入，一次審核。答案是 200，具有完整的`GET`視圖，是在寫入後建構的。

`GET`視圖報表借貸情況如下：

- 每個池都帶有`borrowMode` （`saturation`或`consent`），以及密鑰自己的`lendingPercent`和`lendingUntil`。
- `lendingActive`是`true` ，僅在`consent`池中，百分比大於0且未達到截止日期。
- 在`consent`池中，每個可數`dimensions[].yourShare`都攜帶`borrowAvailable`。這是該密鑰現在可以在其份額之上使用的、由其他密鑰借出的內容。
- `borrowAvailable`使用門的公式。它會讀取所有其他金鑰，即使該金鑰位於其共用之下。對於`hard`鍵，它是每個其他鍵和可數維度的額外讀取，並行。
- `borrowAvailable` is `null` for a `soft` or `burst` key, and `null` when a read fails.
- `borrowAvailable`是所有其他金鑰一起的一個數字。在兩個鑰匙的池中，它是另一個鑰匙自己的數字。
- `percent` windows 或`accounts[]`中尚未報告`borrowAvailable` 。
- 在`saturation`池中，視圖報告使用`lendingActive: false`儲存的同意，而不使用`borrowAvailable`。

### 錯誤

該路由的每個回應，無論成功或錯誤，都帶有`Cache-Control: no-store`。在路由運行之前發生的拒絕不攜帶它，例如客戶端API策略的 401 或IP過濾器的 403。路由的錯誤使用固定訊息的標準錯誤正文：400（無效的提供者）、401（缺少或無效的金鑰）、403（缺少`self:usage`）、404（標記關閉）和 500 (`Failed to build quota view`)。 500 覆蓋請求到達路由後的任何失敗，包括密鑰查找本身；其原因記錄在伺服器上並且從未返回。 `PATCH`的錯誤在[貸款同意](#lending-consent)中列出。

### 限制

- `remaining`是密鑰公平份額中尚未使用的部分。這不是一個保證。當泳池還有空間時，仍可在泳池外領取鑰匙。一旦池的總數達到`limit`，池中的每個鍵都會被拒絕，無論它自己的`remaining`是什麼，並且沒有`self:account-quota`鍵無法看到該總數。
- `remaining`不考慮分配的絕對`cap` 。一旦其在上限單位視窗中的消耗達到上限值，執行就會拒絕該金鑰。
- 帳戶等級欄來自提供者限制快取，可能會延遲執行決策幾分鐘。重置時間已過的讀數會報告為`stale`。
- 僅針對具有計劃視窗對應的提供者報告每個模型視窗 (`modelWindows`)：目前的Claude和Codex 。對於其他提供者，當顯示帳戶資料時， `modelWindows`仍然存在，但`windows`清單為空。
- 密鑰自己的`percent`視窗份額是一個估計。它來自歸因手冊，並具有上面“百分比維度：每個鍵歸因”下列出的所有限制。
- `consumed`是執行數量與公平份額的比較。確切地說，它是`attributed`加`external`。 `attributed`是本書給出其路由的令牌金鑰的部分。 `external`是帳戶使用的金鑰部分，池密鑰不予考慮。
- 只有當池的`accountVisible`為 true 時才會傳送這兩個部分：金鑰具有`self:account-quota`且提供者位於其`sharedQuotaProviders`中。沒有它的金鑰單獨獲得`consumed` ，具有相同的`status`和`reason`。
- 透過這兩個部件及其自身重量，持有者可以計算出泳池外的使用量，並計入泳池的鑰匙中。具有帳戶範圍的持有人已看到帳戶總額。
- 在視窗中沒有路由任何內容的金鑰仍然可以從`consumed`讀取其外部費用，因為其屬性部分為 0。
- 例如，一本書在 0 處打開，密鑰 A 和 B 的權重各為 50。密鑰 A 路由 900,000 個令牌，密鑰 B 路由 100,000 個。然後，該帳戶達到限制 100 的 60%。則`attributed`對於密鑰 A 為 54，對於密鑰 B 為 6，且`external`對於兩者皆為 0。
- 視圖讀取這本書，但從不寫入其狀態。它不會打開一本書，也不會要求提供者閱讀。使用Redis存儲，讀取會在後台刪除被取代的修訂字段，就像門的讀取一樣。
- 共享僅是`ok`而門的快取保存帳戶的讀數。如果沒有，則為`stale`，因此在最近沒有請求的池中，它顯示為可能已過時。
- 在請求通過池之前，共享不可用。此請求開啟帳本，此時帳戶的數字將計為池外的使用量。
- 在具有多個帳戶的池中，每個帳戶條目使用該帳戶自己的帳簿和一個帳戶的限額。執法雙方均按帳戶數量進行縮放，因此比例相同。
- 每個模型的視窗不共享密鑰。本書不保留每個模型的資料。
- 視圖不會評估時間表的保留樓層：時間表可以顯示為`open`而請求因`schedule-reserve`原因被拒絕。
- 當同一密鑰的兩個池共享一個連接時，強制應用其中之一，並且視圖會列出兩者。
- 對於失敗的金鑰嘗試沒有每個位址的限制：在反向代理後面，呼叫者可以共用一個位址（這取決於轉送的用戶端位址是否可信），因此鎖定可能會拒絕通往每個金鑰持有者的路由。使用`REQUIRE_API_KEY=true`時，客戶端API策略會在路由運行之前拒絕無效金鑰，並使用該策略的 401 正文而不是該路由的 401 正文。

### 會員使用

管理員可以讓金鑰持有者查看視窗的使用如何在池成員之間分配。此選項是池的`memberBreakdown`，預設關閉。它是在池精靈中或使用`PATCH /api/quota/pools/{id}`設定的。 `GET /api/quota/pools`和`GET /api/quota/pools/{id}`報告了這一點。

只有當所有這些都成立時，視圖的維度才帶有`members` ：

- 池的選項已開啟
- 該池最多有 20 個分配的密鑰，其中至少三個可以發出請求：有效、未撤銷、未禁止且未過期
- 礦池的`accountVisible`為 true：金鑰有`self:account-quota`且提供者在其`sharedQuotaProviders`中
- 在`percent`視窗上，帳戶的連線是金鑰可以使用的連線之一
- 讀取了密鑰自己的該視窗份額：它的`status`不是`unavailable`

否則`members`不存在。它絕對不是一個空列表。

- 每個切片都是`{ slot, consumed, isYou }`。回應架構拒絕切片上的任何其他屬性以及超過 20 個切片的清單。切片按插槽順序列出。
- 每個指派的鍵都有一個切片，包括不能再發出請求的鍵。沒有用的成員顯示真正的零。
- 插槽 1 始終是詢問鍵， `isYou`為 true。其他槽號是鍵控雜湊的等級。它以`API_KEY_SECRET`為金鑰，涵蓋池、請求金鑰和成員。
- 因此持有者之間的數字並不一致。對於一位持有者來說，他們在兩次訪問之間保持不變。當密鑰加入或離開池時，或當該密鑰輪換時，它們可以更改。
- 在可數視窗上，切片是配額儲存中成員的計數器，與其自己的`consumed`計數器相同。
- 在`percent`視窗上，切片是成員的`attributed`部分，來自作為金鑰自己的共享讀取的同一本書。池外的使用永遠不會分割成切片。該電荷按重量分配，因此攜帶電荷的切片會顯示重量。
- 每個視圖並行讀取每個其他成員和可數視窗的一個值。在`percent`視窗上，除了分享者自己的書籍閱讀之外，切片的閱讀成本不高。當無法讀取一個值時，該視窗沒有`members`，且該鍵自己的共用保留。
- 每個池的選項和可用密鑰數量都會讀取一次，並且僅針對可以查看帳戶資料的密鑰。選項或可用密鑰計數讀取失敗會關閉該池的欄位。伺服器記錄警告，然後建立視圖的其餘部分。

這些酒吧沒有名字或 ID。他們仍然告訴密鑰持有者有關其他成員的資訊：

- 持有者仍然可以根據切片的值來匹配切片。
- 穩定的編號可以讓持有者隨著時間的推移追隨一位成員。
- 切片的數量顯示了池中分配了多少個鍵。
- 在三個密鑰的池中，知道其中一個密鑰使用什麼的人可以知道最後一個密鑰使用什麼。
- 當池中的可用鍵低於三個時，條就會消失。先前拍攝的視圖仍然顯示每個成員使用的內容。
- 在可數視窗上，池總數減去切片可以顯示不再指派的鍵的使用情況。
- 在一個帳戶上顯示零並在另一個帳戶上使用的成員可以顯示哪個成員使用哪個帳戶。
- 在採用`hard`政策的可數池中，停止按成員公平份額增長的切片暗示了該成員的權重。

### 使用系列（`GET /api/v1/me/usage`）

`GET /api/v1/me/usage?range=<range>` （也在`/v1/me/usage`提供服務）傳回呼叫鍵自己的請求的使用情況和成本：總計、每個UTC日、每天和模型、每個模型和每個提供者的一個條目。它共享上述配額路由的標誌、身份驗證規則、 `self:usage`範圍、 `Cache-Control: no-store`和錯誤行為。在`range`之前檢查密鑰。誤差為 400 (`Invalid range`)、401、403、404 和 500 (`Failed to build usage`)。

- `range`是`1d`、 `7d`、 `30d` （預設值）或`90d`之一。任何其他值、空值或重複參數都是 400。該集合在`90d`處停止以限制呼叫成本。此檢視僅讀取原始使用歷史記錄，而不會讀取不含密鑰的每日摘要。
- 行由呼叫鍵的 ID 選擇。鍵名稱列永遠不會匹配，記錄的沒有鍵 id 的行永遠不會被計數。
- 建置系列會對視窗中的鍵行執行五個分組查詢。建構的序列每個鍵和範圍重複使用 60 秒，重複使用的呼叫不會運作。它的`generatedAt`給出了它的年齡。
- 該視窗在系列建置完成後結束。稍後標記的行（例如通過時鐘偏差）不被計算在內。
- `coverage.retentionDays`是營運商的原始使用歷史保留設定（資料庫設定中的`retention.usageHistory` ）。當請求的範圍長於該設定時， `coverage.truncatedByRetention`為 true。它比較兩個數字，但不檢查行是否確實丟失。
- 提供者按照密鑰自己的請求的記錄返回。 Model 是最後一個`/`之後記錄的名稱，行按它分組。每個目標都被拒絕的組合請求將使用作為提供者的路由標籤（組合名稱`auto`或`combo`）和用戶端發送的模型字串進行記錄。其他被拒絕的請求，例如透過斷路器斷路器、模型冷卻或配額停放跳過，保留目標提供程序和模型。
- 除了計數和成本之外，回應還包含平均延遲、成功率以及第一個和最後一個請求的時間。
- `byModel`列出了請求最多的 50 個提供者和模型對。對於更多對，其條目加起來不會達到`summary`，並且`summary.uniqueModels`會計算每個記錄的模型拼寫。則`byModelTruncated`為真，且對落在切割兩側的模型顯示部分總數。
- 報告了兩項成本。 `costUsd`是計費成本，如使用情況分析所示。固定費率訂閱提供者（例如Claude Code 方案）的計數為 0 美元。 `listPriceUsd`使用量與標價相同，包括訂閱。模型沒有價格行的請求會計算其儲存的成本：提供者報告的成本，或記錄請求時計算的成本。只有兩者都沒有的請求才算為 0，並且沒有標記，因此總計可能是部分的。
- 回應合約是`src/shared/schemas/selfUsage.ts` （ `docs/openapi.yaml`中的`SelfUsageSeries` ）。

### 自助服務頁面

`QUOTA_SELF_PANEL`開啟後， `/quota/{provider}`就是一個公開頁面。密鑰持有者在此鍵入API密鑰，並查看提供者的該密鑰池。每個池子的每個池子視窗顯示一張卡，每個人都可以使用該池子，並且鑰匙自己共享。池中的每個帳戶都有自己的卡，有帳戶的用途和密鑰的份額。只有當金鑰可以看到帳戶資料時，才會顯示帳戶的使用情況。該頁面還列出了每個帳戶的每個模型限制以及金鑰本身的使用情況。當日程表目前封鎖該金鑰時，會出現一則通知。卡片列出了每個型號的鑰匙上限及其使用情況，並標記了已達到的上限。 `{provider}`是提供者 ID 或其別名（`/quota/claude`、 `/quota/cc`）。未知的提供者，以及標誌關閉時的每個`/quota/*`路徑，都會回答 404。自訂 OpenAI 或 Anthropic 相容節點上的池沒有頁面。 API仍然為他們解答。

該頁面沒有會話。密鑰僅在`GET /api/v1/me/quota/{provider}`、 `PATCH /api/v1/me/quota/{provider}`和`GET /api/v1/me/usage`的`Authorization`標頭中發送，而不會在URL中發送。伺服器接受的金鑰保存在選項卡的`sessionStorage`中。使用「記住在此裝置上」時，它會保留在`localStorage`中，而「忘記金鑰」則會將其從兩者中刪除。伺服器拒絕的密鑰將從儲存空間中刪除。

`consent`模式下的礦池顯示一張借貸卡。在那裡，鑰匙持有者設定了鑰匙閒置份額的 0 到 100 的整數百分比來出借。持有者還可以選擇同意的持續時間：直到關閉、1 小時、8 小時、24 小時、7 天或 30 天。持續時間從保存的那一刻開始計算。當截止日期有效時，持有者可以保留它。如果在「儲存」之前過了該截止日期，則該卡將不發送任何內容並要求其他選擇。如果為 0%，則不會發送截止日期。此卡顯示儲存的截止日期及其指定的時區。已過截止日期的同意將顯示為已結束。

對於`hard`密鑰，該卡還列出了每個池視窗目前借給該密鑰的其他密鑰。每一行都是所有其他鍵的一個數字。在兩個鑰匙的池中，它是另一個鑰匙自己的數字。視圖不報告的數字讀取為不可用，而不是零。對於`soft`或`burst`鑰匙，卡片上顯示沒有數字適用。

`saturation`模式下的礦池，其金鑰儲存的百分比大於 0，僅顯示提款。它說存儲的百分比在那裡沒有影響。它的“提款”按鈕發送 0，沒有截止日期。 `saturation`模式下的礦池儲存了 0，表示沒有借出卡片。儲存後，返回的視圖不再需要的卡片將保留其訊息，直到頁面視圖再次變更。

在持有人按下「儲存」或「提款」之前，不會儲存任何內容。每個壓力機都會發送一個`PATCH /api/v1/me/quota/{provider}`請求，而第二個壓力機在第一個壓力機等待處理時不會發送任何內容。主體帶有池的不透明`ref`從視圖、百分比和截止日期。答案是重建的配額視圖，頁面顯示它，無需第二次讀取。當兩個儲存重疊時，頁面會在最後一個答案後讀取一次配額。該頁面不會在瀏覽器儲存中保留同意。

拒絕更改會在卡片上透過從HTTP狀態中選擇的文字進行解釋。錯誤主體未被讀取。 401 表示密鑰未被接受並重新載入配額。 403 表示池未進行貸款更改，404 表示池已消失。兩者都提供了重新加載配額的按鈕。 400 或另一個 4xx 答案要求持有人檢查百分比和截止日期。 429 要求持有者等待，並在得到答覆時以`Retry-After`秒數等待。 5xx 答案、408 或網路故障表示變更可能尚未儲存，並保留鍵入的值。合約之外的答覆會重新加載配額。儲存失敗不會自行刪除密鑰。當拒絕後重新載入時，頁面會像任何被拒絕的讀取一樣刪除金鑰。

接受密鑰後，該頁面還會顯示帶有三個選項卡的「設定您的工具」卡。 「Claude Code」給了`~/.claude/settings.json`的`env`塊。 “Shell”給出與`export`行相同的變數。 「Claude Desktop」給出了其第三方推理視窗的值。這些模型是密鑰可能要求該提供者的配額共享模型。當金鑰沒有包含此類清單時，該區塊會改為啟用網關模型發現。網關位址是伺服器報告的公共API來源（`OMNIROUTE_PUBLIC_API_BASE_URL`，然後`OMNIROUTE_PUBLIC_BASE_URL`）。如果兩者都未設置，卡片會顯示一個佔位符並告訴持有者詢問管理員。鍵顯示為佔位符。 「包括我的密鑰」將整個密鑰放在螢幕上的文字中以及複製按鈕複製的內容中。這種情況會一直持續到盒子被清除、鑰匙被遺忘或更換、或頁面被留下為止。該卡不發送請求，也不提供文件下載。

API標記`stale`的讀數顯示為可能已過時。標記`unavailable`讀數會顯示其原因，而不是零。

在百分比計劃中，當API報告時，頁面會繪製密鑰自己的份額。它說這個數字是一個估計值並指出了它的兩個部分。每個模型的限制僅顯示帳戶。

當視窗帶有`members`時，其卡片也會顯示一個欄，每個成員會以插槽順序顯示一個段落。詢問鍵的部分使用強調色。其他部分循環顯示主題的圖表顏色。文字圖例列出了每個段落及其值，因此不依賴顏色。段標記為`You`或`Member N`，其中 N 是槽。

### 頁面專用連接埠

`QUOTA_PANEL_PORT`開啟第二個偵聽器，僅為自助服務頁面提供服務。除非設定了變量，否則它會關閉。 `QUOTA_PANEL_HOST`是綁定位址，預設為`127.0.0.1`。

偵聽器將這些路徑中繼到主端口，並為每個其他路徑應答 404：

| 小路                                                                     | 服務                   |
| ------------------------------------------------------------------------ | ---------------------- |
| `/quota/{provider}`                                                      | 頁面                   |
| `/api/v1/me/quota/{provider}`, `/v1/me/quota/{provider}`                 | 查看頁面讀取的配額     |
| `/api/v1/me/usage`, `/v1/me/usage`                                       | 頁面讀取的使用系列     |
| `/_next/static/`                                                         | 建構的腳本、樣式和字體 |
| `/favicon.ico`, `/favicon.svg`, `/icon-512.png`, `/apple-touch-icon.png` | 圖示                   |

`GET`和`HEAD`在沒有正文的情況下進行中繼。也中繼了一個帶有正文的請求：配額視圖路徑的`PATCH` ，頁面發送該請求以保存借出選擇。任何其他方法都會應答 404，除了CONNECT請求，其連線會在沒有應答的情況下關閉。聲明主體的任何其他請求都會回答 404，其連接將關閉。升級請求被拒絕並且它們的連線被關閉。帶有有點段或片段標記的路徑將被拒絕，如在API端口上。具有可列印ASCII之外的字元的請求目標也是如此。在該連接埠自行進行檢查之前， HTTP解析器會回答目標中的原始控製字元 400。框架保留供自己使用的請求標頭不會被轉發：以`x-middleware-`、 `x-invoke-`、 `x-nextjs-`、 `x-now-`或`x-next-`開頭的名稱，以及名稱`x-matched-path`和`next-resume`。請求在沒有它們的情況下被轉發。儀表板、登入頁面、管理API和推理路由無法透過此連接埠存取。

`PATCH`必須攜帶`Content-Type: application/json`，不含參數或僅帶`charset=utf-8` 。它必須攜帶一個從 1 到 4096 的`Content-Length` ，寫為純數字，並且沒有`Transfer-Encoding`。違反這些規則之一的`PATCH`會回答 404。在該連接埠自行檢查之前， HTTP解析器會回答 400 一些格式錯誤的長度，例如帶符號或重複的長度。連接埠在聯繫主連接埠之前讀取聲明的位元組，並最多等待 5 秒。此時尚未完成的主體會回答 404，其連接將關閉。在這種情況下，或當客戶端先離開時，沒有任何東西到達主連接埠。連接埠準確地中繼聲明的字節，具有相同的`Content-Length`。它們之後的位元組將作為連接上的下一個請求讀取。前面的TLS反向代理必須轉發`Content-Length`且不得重新分塊請求正文。主埠檢查`Authorization`標頭中的API鑰，就像`GET`一樣。

404正文是`{"error":"not_found","message":"Not found."}`。失敗的中繼會回應 502 (`api_bridge_unavailable`) 或 504 (`api_bridge_timeout`)，但沒有`detail`欄位。

偵聽器不會讀取`QUOTA_SELF_PANEL`，也不會開啟頁面。當標誌關閉時，頁面及其API在主連接埠上應答 404，並且偵聽器中繼該應答。

在開發伺服器（`next dev`）下，頁面不會透過此連接埠進行互動。開發熱重載套接字是升級請求，連接埠拒絕它。開發時使用主端口。

連接埠提供普通HTTP服務，頁面發送API金鑰。保留預設的綁定位址，並在其前面放置一個帶有TLS反向代理。除環回之外的綁定位址會記錄此通知：

```text
[Quota Panel] Bound to <host>. This port serves plain HTTP and the page sends API keys. Put a TLS reverse proxy in front of it.
```

不發送轉送標頭的環回對等體在主連接埠上被視為本機。因此同一主機上的代理程式必鬚髮送`X-Forwarded-For`。僅使用`OMNIROUTE_TRUST_PROXY=private` （或`lan`）的該標頭才信任私有位址上的代理。任何其他對等點都透過其連接位址進行報告，並且其發送的轉發標頭將被丟棄。

偵聽器一次最多擁有 256 個連線。客戶端有 10 秒的時間發送請求標頭，有 30 秒的時間發送整個請求。空閒的保持活動連線將在大約 5 秒後關閉。 60 秒內沒有任何活動的連線將會關閉。這些值是固定的。還要在前面的反向代理上設定連線和速率限制。前面的反向代理應將其空閒上游連線保持在 5 秒以內，或不重複使用它們。到主埠的中繼使用API埠 (`API_BRIDGE_*`) 的上游逾時。

當`API_PORT`未設定時，監聽器也會啟動。 `QUOTA_PANEL_PORT`必須是 1 到 65535 之間的端口，僅以數字形式書寫。它必須不同於儀表板端口和API端口。當即時WebSocket伺服器開啟時，它也必須與`LIVE_WS_PORT`不同（預設 20132）。任何其他值都不會開啟任何內容並記錄警告。有關拒絕值的警告會為變數命名，並且不會重複該值。已在使用的連接埠不會開啟任何內容並記錄此警告：

```text
[Quota Panel] Port <port> is already in use. The quota panel port stays off.
```

設定`OMNIROUTE_BASE_PATH`後，偵聽器期望該前綴下的上述每個路徑。在建置時和運行時使用相同的`OMNIROUTE_BASE_PATH` 。使用前導斜線且沒有尾隨斜線編寫它，例如`/omniroute`。另一種形狀，包括`/`和`/omniroute/`，將連接埠關閉並帶有警告，儘管建置接受這些形式。在任何情況下，第一段命名應用程式路由的基本路徑也是如此： `api`、 `v1`、 `v1beta`、 `_next`、 `quota`、 `dashboard`、 `docs`、 `login`、 `codex`、 `responses`、 `anthropic`、 `openai`、 `v0`或`connect`。

限制：

- 帶有尾部斜杠的`/quota/{provider}/`在此端口上應答 404。
- Service Worker 和 Web 應用程式清單不在此連接埠上提供服務。
- 此連接埠上不顯示儀表板中設定的自訂圖示。
- 當應用程式在基本路徑下運行時，不會顯示圖示。
- 該埠講普通的HTTP/1.1.
- 在進程重新啟動之前，不會重試失敗的綁定。
- 偵聽器對每個用戶端位址沒有連線或速率限制。
- 本節不涵蓋容器設定。

---

## 環境變數

| 多變的                               | 預設         | 描述                                             |
| ------------------------------------ | ------------ | ------------------------------------------------ |
| `QUOTA_STORE_DRIVER`                 | `sqlite`     | 使用的驅動程式： `sqlite`或`redis`               |
| `QUOTA_STORE_REDIS_URL`              | _（空的）_   | Redis URL, 例如`redis://localhost:6379`          |
| `QUOTA_SATURATION_THRESHOLD`         | `0.5`        | 0..1; `>= threshold`啟動嚴格模式                 |
| `QUOTA_PERCENT_MIN_TOKENS_PER_POINT` | `1000`       | 最多解釋百分比計劃視窗的一個點的令牌             |
| `QUOTA_SOFT_DEPRIORITIZE_FACTOR`     | `0.7`        | 0..1；軟政策組合分數的乘數                       |
| `QUOTA_CONSUMPTION_RETENTION_DAYS`   | `14`         | GC刪除舊`quota_consumption`儲存桶前的天數        |
| `QUOTA_PANEL_PORT`                   | _（未設定）_ | 自助服務頁面的專用連接埠。未設定表示沒有偵聽器。 |
| `QUOTA_PANEL_HOST`                   | `127.0.0.1`  | 為該連接埠綁定位址                               |

DB設定 (`quotaStore.*`) 覆蓋環境變數。

---

## 疑難排解

### 已設定 Redis 但無法連線

請確認已安裝 `ioredis`（`npm ls ioredis`），且可連線至 `QUOTA_STORE_REDIS_URL`。連線失敗時，factory 會退回使用 SQLite（以 `warn` 層級記錄）。

### `peek` 傳回過時資料／開放式失敗

如果 `peek` 擲回錯誤，`enforceQuotaShare` 會將結果視為「允許」（開放式失敗）。請檢查 `pino` 日誌中的 `quota:enforce` 與 `quota:factory` 項目，以找出根本原因。

### 消耗計數器偏移

如果實際提供者使用量與計數器不同，這屬於預期情況——雙儲存桶滑動視窗在視窗邊界約有 1% 的誤差，而且 `consume` 是在回應後以即發即棄方式執行。飽和度訊號（`saturationSignals.ts`）會以 30 秒 TTL 讀取真實的提供者使用率，並據此調整 `globalUsedPercent`。

### 集區的消耗速率顯示「無資料」

`computeBurnRate` 至少需要 2 個歷史樣本。先前沒有 `consume` 呼叫的新集區將顯示 `tokensPerSecond: 0` 和 `timeToExhaustionMs: null`。

---

## 從 localStorage 遷移

當 `/dashboard/costs/quota-share` 首次載入時，hook `useLocalStoragePoolMigration`
會檢查：

1. `localStorage.getItem("omniroute:quota-share:pools")` 不為空。
2. `GET /api/quota/pools` 傳回 `[]`（DB 為空）。

若兩者皆為真，則會將每個舊版資源池批次發送至 `POST /api/quota/pools`，
然後移除 localStorage 金鑰。此遷移具備冪等性：條件 2 可防止
重複遷移。

---

## 內部策略分類

`quota-share` 是一種**僅限內部使用**的路由策略（位於
`src/shared/constants/routingStrategies.ts` 中的 `INTERNAL_ROUTING_STRATEGY_VALUES`）。
它僅供系統建立的 `qtSd/` 資源池組合使用，並刻意從 `ROUTING_STRATEGY_VALUES` 中排除，
因此絕不會在 UI 或 API 中顯示為使用者可選取的選項。

---

## 測試覆蓋率

配額共享引擎提供兩層自動化覆蓋：

| 套房              | 命令                                                                   | 它涵蓋什麼                                                                                                                                                       |
| :---------------- | :--------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 單元（29 項測試） | `node --import tsx/esm --test tests/unit/quota-share-strategy.test.ts` | DRR調度程序、飽和門控、並發上限、 fairShare數學、積壓隊列                                                                                                        |
| 積分矩陣          | `npm run test:combo:matrix`                                            | 透過真實組合管道進行端對端路由決策； DRR公平性+透過即時接縫進行飽和度降低優先權（`registerQuotaFetcher`、 `setLKGP`、 `__setHeadroomSaturationFetcherForTests`） |

集成矩陣與所有 22 種公共策略一起在CI中運行。該單元套件可以獨立運作。

---

## DB架構摘要

遷移`078`、 `079`和`085`新增的三個表：

- `quota_pools` + `quota_allocations` —池定義和每鍵分配。
- `quota_consumption` —每個`(apiKeyId, dimensionKey)`滾動 2 桶計數器。
- `provider_plans` —手動提供者計畫覆蓋（每個connectionId的JSON維度）。

透過冪等`CREATE TABLE IF NOT EXISTS`遷移添加的所有表。

同意借貸添加了三列： `quota_allocations.lending_percent` （整數，預設 0）、 `quota_allocations.lending_until` （紀元毫秒，或`NULL`表示無截止日期）和`quota_pools.borrow_mode` （預設`saturation`）。它的遷移僅添加這些列，而不寫入現有行。

百分比歸屬簿新增了`quota_percent_ledger` （每個池、帳戶和計畫視窗一行）和`quota_percent_ledger_tokens` （每個池、帳戶和API密鑰一個代幣計數器）。 `src/lib/db/quotaPercentLedger.ts`讀取和寫入它們。
