# Merge Queue & Manual Merge-Train Runbook (中文 (繁體))

🌐 **Languages:** 🇺🇸 [English](../../../../ops/MERGE_TRAIN.md) · 🇪🇹 [am](../../../am/docs/ops/MERGE_TRAIN.md) · 🇸🇦 [ar](../../../ar/docs/ops/MERGE_TRAIN.md) · 🇦🇿 [az](../../../az/docs/ops/MERGE_TRAIN.md) · 🇧🇬 [bg](../../../bg/docs/ops/MERGE_TRAIN.md) · 🇧🇩 [bn](../../../bn/docs/ops/MERGE_TRAIN.md) · 🇧🇦 [bs](../../../bs/docs/ops/MERGE_TRAIN.md) · 🇨🇿 [cs](../../../cs/docs/ops/MERGE_TRAIN.md) · 🇩🇰 [da](../../../da/docs/ops/MERGE_TRAIN.md) · 🇩🇪 [de](../../../de/docs/ops/MERGE_TRAIN.md) · 🇬🇷 [el](../../../el/docs/ops/MERGE_TRAIN.md) · 🇪🇸 [es](../../../es/docs/ops/MERGE_TRAIN.md) · 🇪🇪 [et](../../../et/docs/ops/MERGE_TRAIN.md) · 🇮🇷 [fa](../../../fa/docs/ops/MERGE_TRAIN.md) · 🇫🇮 [fi](../../../fi/docs/ops/MERGE_TRAIN.md) · 🇫🇷 [fr](../../../fr/docs/ops/MERGE_TRAIN.md) · 🇮🇪 [ga](../../../ga/docs/ops/MERGE_TRAIN.md) · 🇮🇳 [gu](../../../gu/docs/ops/MERGE_TRAIN.md) · 🇳🇬 [ha](../../../ha/docs/ops/MERGE_TRAIN.md) · 🇮🇱 [he](../../../he/docs/ops/MERGE_TRAIN.md) · 🇮🇳 [hi](../../../hi/docs/ops/MERGE_TRAIN.md) · 🇭🇷 [hr](../../../hr/docs/ops/MERGE_TRAIN.md) · 🇭🇺 [hu](../../../hu/docs/ops/MERGE_TRAIN.md) · 🇦🇲 [hy](../../../hy/docs/ops/MERGE_TRAIN.md) · 🇮🇩 [id](../../../id/docs/ops/MERGE_TRAIN.md) · 🇳🇬 [ig](../../../ig/docs/ops/MERGE_TRAIN.md) · 🇮🇹 [it](../../../it/docs/ops/MERGE_TRAIN.md) · 🇯🇵 [ja](../../../ja/docs/ops/MERGE_TRAIN.md) · 🇬🇪 [ka](../../../ka/docs/ops/MERGE_TRAIN.md) · 🇰🇭 [km](../../../km/docs/ops/MERGE_TRAIN.md) · 🇮🇳 [kn](../../../kn/docs/ops/MERGE_TRAIN.md) · 🇰🇷 [ko](../../../ko/docs/ops/MERGE_TRAIN.md) · 🇱🇹 [lt](../../../lt/docs/ops/MERGE_TRAIN.md) · 🇱🇻 [lv](../../../lv/docs/ops/MERGE_TRAIN.md) · 🇮🇳 [ml](../../../ml/docs/ops/MERGE_TRAIN.md) · 🇮🇳 [mr](../../../mr/docs/ops/MERGE_TRAIN.md) · 🇲🇾 [ms](../../../ms/docs/ops/MERGE_TRAIN.md) · 🇲🇹 [mt](../../../mt/docs/ops/MERGE_TRAIN.md) · 🇲🇲 [my](../../../my/docs/ops/MERGE_TRAIN.md) · 🇳🇵 [ne](../../../ne/docs/ops/MERGE_TRAIN.md) · 🇳🇱 [nl](../../../nl/docs/ops/MERGE_TRAIN.md) · 🇳🇴 [no](../../../no/docs/ops/MERGE_TRAIN.md) · 🇮🇳 [or](../../../or/docs/ops/MERGE_TRAIN.md) · 🇮🇳 [pa](../../../pa/docs/ops/MERGE_TRAIN.md) · 🇵🇭 [phi](../../../phi/docs/ops/MERGE_TRAIN.md) · 🇵🇱 [pl](../../../pl/docs/ops/MERGE_TRAIN.md) · 🇵🇹 [pt](../../../pt/docs/ops/MERGE_TRAIN.md) · 🇧🇷 [pt-BR](../../../pt-BR/docs/ops/MERGE_TRAIN.md) · 🇷🇴 [ro](../../../ro/docs/ops/MERGE_TRAIN.md) · 🇷🇺 [ru](../../../ru/docs/ops/MERGE_TRAIN.md) · 🇱🇰 [si](../../../si/docs/ops/MERGE_TRAIN.md) · 🇸🇰 [sk](../../../sk/docs/ops/MERGE_TRAIN.md) · 🇸🇮 [sl](../../../sl/docs/ops/MERGE_TRAIN.md) · 🇷🇸 [sr](../../../sr/docs/ops/MERGE_TRAIN.md) · 🇸🇪 [sv](../../../sv/docs/ops/MERGE_TRAIN.md) · 🇰🇪 [sw](../../../sw/docs/ops/MERGE_TRAIN.md) · 🇮🇳 [ta](../../../ta/docs/ops/MERGE_TRAIN.md) · 🇮🇳 [te](../../../te/docs/ops/MERGE_TRAIN.md) · 🇹🇭 [th](../../../th/docs/ops/MERGE_TRAIN.md) · 🇹🇷 [tr](../../../tr/docs/ops/MERGE_TRAIN.md) · 🇺🇦 [uk-UA](../../../uk-UA/docs/ops/MERGE_TRAIN.md) · 🇵🇰 [ur](../../../ur/docs/ops/MERGE_TRAIN.md) · 🇺🇿 [uz](../../../uz/docs/ops/MERGE_TRAIN.md) · 🇻🇳 [vi](../../../vi/docs/ops/MERGE_TRAIN.md) · 🇳🇬 [yo](../../../yo/docs/ops/MERGE_TRAIN.md) · 🇨🇳 [zh-CN](../../../zh-CN/docs/ops/MERGE_TRAIN.md)

---

## 登陸發布分支

全隊列管理著`release/vX.Y.Z`的登陸。在登陸PR之前，請閱讀預設分支上`config/merge-queue/config.json`中的頂級`mode` 。請參閱[全方位隊列](OMNI_QUEUE.md)。

- **`shadow`**運行驗證並將登陸留給手動合併。將`omni-queue`應用到核准的PR最後一個頭。使用`npm run queue -- why <PR>`檢查資格。等待`npm run queue -- history --base <branch>`那個頭的判決。繼續`would-land`。在`culprit-found`或`would-dequeue`上，保留合併並修復原因。
- **陰影異常。**相對於當前基本提示具有綠色完整CI列車可以繼續行駛，而無需單獨的隊列判決。當PR頭已包含目前基尖時，同樣的例外情況也適用。
- **`live`**使用`omni-queue`標籤觸發登陸。隊列單獨登陸PR。將合併命令和直接推送保留到隊列中。

每次著陸都需要業主的授權和適用的必要檢查。僅在業主授權登陸後才可申請`omni-queue` 。接觸受保護路徑的排隊PRs也需要所有者對該PR進行`protected-approved`決策。

「活動版本需要綠色大門」規則集需要頭部有綠色`Gate / CI`和`Gate / Quality` 。切勿使用`--admin`繞過紅色大門。發布凍結區塊合併到凍結分支。參見[硬性規則 21](HARD_RULES_DETAIL.md) 。切勿標記、合併或推送另一個會話正在執行的拉取請求。參見[硬性規則 22](HARD_RULES_DETAIL.md) 。

## 火車拉動請求

1. 在目前版本的基礎尖端啟動一個火車分支。使用合併提交來整合確切批准的成員頭。透過避免擠壓和變基來保留他們的提交歷史記錄。
2. 為火車分支打開一個拉取請求。在當前基本提示上使用其自己的完整CI來驗證該PR 。著陸前重新檢查底座尖端和經批准的成員頭。當經過驗證的候選人發生變化時，刷新列車及其CI 。
3. 在適用的佇列模式下使用合併提交來登陸PR 。在即時模式下，佇列的`merge-ff`登陸方法會保留合併提交。原始成員頭可以從發布分支存取。 GitHub將成員PRs標記為已合併，並提交保留其作者。

一個公共範例是[PR #21071](https://github.com/cheaper-inference/OmniRoute/pull/21071) 。它合併了 18 位PRs成員，並於 2026 年 11 月 24 日進行了合併提交。

從`main`到下一個發布分支的同步也透過合併提交實現。稍後同步需要保留`main`祖先。請參閱[工作樹隔離](WORKTREE_ISOLATION.md#sync-back-landings-are-merge-commits-never-squash)。

## 本地合併訓練驗證器

```bash
scripts/release/merge-train.sh [--plan] [--fast] <base-branch> <PR#> [<PR#>...]
```

驗證器會取得基本頭和PR頭並將它們組合在一次性工作樹中。它在生成的樹上運行一次奇偶校驗套件。失敗的頭部獲取或合併衝突會彈出該PR ，腳本繼續處理剩餘的PRs。

- **`--plan`**列印所選模式的步驟並退出，無需建立工作樹或聯絡遙控器。與`--fast`結合檢查快速計劃。
- **`--fast`**運行常見的靜態閘、 `tests/unit/`和`npm run test:vitest`下選定的已更改`node:test`檔。使用快速模式時，每天至少對累積小費運行一次完整的本地驗證。
- **完整模式**新增純靜態閘並運行`npm run test:unit`和`npm run test:vitest`。

如果基礎探針可用，則在未觸及的基礎上重新執行失敗的靜態閘。此腳本會報告繼承的故障，並在每個已識別的違規行也出現在基礎上且總計數未增加時繼續。

| 出口 | 意義                                                                                   |
| ---- | -------------------------------------------------------------------------------------- |
| `0`  | 列印計劃或完成套件。套件摘要列出了所有繼承的靜態故障和彈出的PRs。                      |
| `1`  | 參數無效、沒有 Git 簽出、預檢失敗或沒有登上PR 。                                       |
| `2`  | 套件檢查失敗，不符合繼承條件。操作員可以將批次一分為二，彈出有問題的PR，然後重新運行。 |

本地通行證僅為所有者的檔案提供診斷證據。每次登陸仍然需要所有者授權、其自己所需的檢查以及影子隊列判決（如果適用）。

## 分層

- **根據PR。** CI和 Quality 選擇基於變更的路徑進行檢查。程式碼PRs運行快速品質閘和受影響的測試，並在CI中使用單獨的單元和Vitest作業。
- **每個隊列候選人。** CI和 Quality 在其佇列引用上運行組合候選者的完整設定檔。
- **每個發布提示。** Release-Green 在與其路徑過濾器匹配的推送上運行快速硬門。每天 3 次計畫的運行使用發布分支的全面掃描。
- **每個版本。**完整的CI矩陣包括E2E分片、包驗證、tarball 引導煙霧和覆蓋率檢查。請[參閱發布清單](RELEASE_CHECKLIST.md)。

## `merge-train.sh`新鮮結帳先決條件

預檢在創建工作樹之前運行。使用`npm ci`安裝相依性。確認`node_modules/.bin/tsc`可執行且`node_modules/node_modules`不存在。檢查`node_modules/.bin/bun --version`是否成功。

如果跳過Bun安裝後，請執行`(cd node_modules/bun && node install.js)`。提供者一致性和已知符號檢查使用Bun。驗證器將`npm run check:cycles:ratchet`作為阻塞門運作。獨立的`npm run check:cycles`指令是建議性的。

## 歷史

Mergify 合併佇列已於 2026 年 11 月 19 日停用。
