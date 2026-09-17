# AMPM-AIOPS 工單索引（Gate 0～17）

本檔是**索引**，不是新規格、不是新版本。

- 正式工單：`AMPM_FINAL_MASTER_TRANSFORMATION_WORK_ORDER_20260819_DRAFT.md`（正本在 VPS，不在本倉庫）
- 規格來源：[`AMPM_AIOPS_DECIDED_STRATEGY_RECORD_20260818-20260819.md`](AMPM_AIOPS_DECIDED_STRATEGY_RECORD_20260818-20260819.md)（第 0～107 節）
- 施工標的：`/opt/ampm/heiyao/AMPM-AIOPS/ampm-site`（VPS）
- 治理正本：`/root/開工儀式.md`（VPS）

## 本檔不做什麼（對應策略記錄 §0）

不建立 FINAL_v2、FINAL_NEW、FINAL_FIXED、平行架構、另一套評分制度、另一個新版產品概念。
本檔**不新增任何規格**，只把第 94 節已定的 Gate 順序，對應回記錄中定義其內容的節次，讓「哪一 Gate 依據哪一段」可追溯（§99：公開的事實與決策必須可追溯）。

## Gate 狀態語意

沿用 §19 的既有語意，不另立一套：

| 值 | 意義 |
| --- | --- |
| `UNKNOWN` | 理論上應該有資料，但現在沒有足夠 Evidence。**不能補 0、不能補平均、不能叫 AI 猜。** |
| `MISSING_REQUIRED` | 必要條件缺失，阻止進入下一階段 |
| `CONFLICT` | 可信來源對同一事實真正矛盾 |
| `PASS` | 已有實測證據通過 |

**目前所有 Gate 狀態一律為 `UNKNOWN`。**
原因：本倉庫只有策略記錄與本索引，**沒有任何 `ampm-site` 程式碼、資料庫、pipeline 產出或測試報告**；施工實況只存在於 VPS。在取得實測證據前把任何 Gate 標成 PASS，就是 §43「Two-pass 不准造假」與 §19「UNKNOWN 不能猜」明文禁止的行為。

## Gate 0～17

| Gate | 名稱 | 規格出處（節） | 狀態 | 判定 PASS 所需證據 |
| --- | --- | --- | --- | --- |
| 0 | Baseline / Restore | §2、§93 | `UNKNOWN` | 既有站台可 build、既有 URL 未破壞之還原點 |
| 1 | Canonical Data | §10、§11、§19、§99 | `UNKNOWN` | canonical 資料表、`raw_member_count` 與 `eligible_count` 分離、舊 Category 未被當已驗證 |
| 2 | Data Engine | §36～§41、§46～§48 | `UNKNOWN` | COLLECT→…→pipeline 實跑紀錄、Crawl Resilience、Anti-Cascade 實測 |
| 3 | Evidence | §37、§38、§40、§42～§45 | `UNKNOWN` | Official Source Registry、Snapshot/Hash/Diff、Confidence、穩定 `fact_id`、Evidence Durability |
| 4 | AMPM Standard | §64、§92 | `UNKNOWN` | 公開 Standard / Transparency 頁、Badge 與 Verification 機制 |
| 5 | Market Intelligence | §22～§28 | `UNKNOWN` | Category Heat V1、Competition Index V1、Seat Allocation、Stability Guard、Non-Eviction |
| 6 | Founding 100 | §29～§35 | `UNKNOWN` | Founding Selection 實跑、Lifecycle、Grace/Revalidation、Watchlist、Museum |
| 7 | AMPM100 UI | §3～§9、§12～§21 | `UNKNOWN` | 兩層 Category、Generalist/Specialist、Capability Badge、Score V1 五維、Tie-break、Coverage 門檻 |
| 8 | Radar | §49～§56 | `UNKNOWN` | Radar Event Flow 串起 News / Column / 貓日報之內容鏈 |
| 9 | Battles | §57～§59 | `UNKNOWN` | Battle 有 Evidence、pairing 不星狀退化 |
| 10 | Homepage / Nav / Brand | §75～§78 | `UNKNOWN` | Homepage、九宮格、Navigation、AMO / PIMI |
| 11 | Ask AMPM | §60～§63 | `UNKNOWN` | 不知道時的行為、資料庫外工具行為、Paid AI 掛掉時的降級 |
| 12 | SEO / GSC | §79～§84 | `UNKNOWN` | 保留既有 URL、Phase 1 SEO Freeze、Compare SEO、Opportunity Engine、語言策略 |
| 13 | Analytics / 404 | §85、§86 | `UNKNOWN` | Analytics 埋點、404 策略 |
| 14 | Self Audit | §98 | `UNKNOWN` | 主 Orchestrator 自行驗證 Worker 交件之紀錄 |
| 15 | Final Regression | §100 | `UNKNOWN` | 對 §100 全部 8 項已修問題之回歸測試 |
| 16 | **Production Deploy** | §95 | `MISSING_REQUIRED` | **永不自動 PASS。** 必須 Owner 當下明確批准，且走 `/root/deploy_guard.sh` |
| 17 | Post-launch Observation | §84、§87、§88 | `UNKNOWN` | 上線後 SEO 觀察、Worker 掛掉時之行為驗證 |

## 橫跨全 Gate 的兩條線（非獨立 Gate）

| 線 | 內容 | 節次 |
| --- | --- | --- |
| 商業隔離層 | Affiliate / Sponsor / Ads 完全隔離、Lifecycle、Resolver、Owner-only、Murf AI、AdSense 兩層與 Content Value | §67～§74 |
| 生存架構層 | Survival Architecture、Worker 掛掉時、Domain / SEO 資產優先、Paid AI 不得為單點依賴 | §87～§90 |

補充：成長與分發 §91、Cost Architecture §101。

## 施工授權邊界（§96、§97）

- **Owner STOP 最高優先**：Owner 說停即停，Task Completion 不得壓過 STOP。
- **低風險自己做**：可回滾、規格明確、普通 bug、adapter、parser、一般 code fix、validation fix。不用每一步問 Owner。
- **高風險必須 HOLD**：destructive、reset / clean、大量刪除、大量 rename / move、force push、DNS、Production Deploy、mass URL、canonical、noindex、付款、OTP、KYC、法律授權。

## §100 已發現並修過的重要問題（回歸測試清單）

1. `fact_id` collision
2. Hamilton Seat Allocation 加總錯誤
3. evidence generator 重跑會清掉 earned verification
4. felo 假 two-pass
5. Battle pairing 星狀退化
6. acceptance test 用 flag 驗證 flag
7. sitemapindex 假檢查
8. Browser 被錯當 default collector

以上皆屬「實作沒有符合原本已定策略」之修正，不是重新設計產品。

## §107 剩餘核心工作

讓現有系統真正產生足夠的：Verified Evidence、Verified Category、Verified Capability、Scoreable Dimensions、Active Eligible Candidates、真正 Founding Selection、可用 AMPM100、有 Evidence 的 Radar / Battles / Ask、原創決策內容。

直到系統能真正回答：為什麼它進 AMPM100？依據什麼？同 Category 為什麼排這裡？最近發生什麼？這個 Battle 為什麼這樣判？證據在哪裡？

## 驗證阻斷紀錄

本索引由雲端隔離容器產出。該容器**無法**存取：`/root/開工儀式.md`、`/opt/ampm/heiyao/AMPM-AIOPS/ampm-site`、正式工單檔案、VPS 上任何施工產出。
已核對之 GitHub 範圍：`chainuncel/AMPM-AI`（全分支全歷史，僅 2 個 md 檔、0 Issue、0 PR）、`chainuncel/OTTO`（空庫）、`chainuncel/chainuncel.github.io`（僅 `index.html`，與 AMPM 無關）。
因此本檔只能索引「已定規格」，不能代替施工驗收。
