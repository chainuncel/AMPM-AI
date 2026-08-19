AMPM-AIOPS｜2026-08-18～2026-08-19 已定策略完整整理
適用網站：https://ampm-aiops.com
正式網站 Repo：/opt/ampm/heiyao/AMPM-AIOPS/ampm-site
治理正本：/root/開工儀式.md
==================================================
0. 這不是另一個版本
==================================================
這次 AMPM 轉型只有同一套方向。
不建立：
FINAL_v2
FINAL_NEW
FINAL_FIXED
另一套平行架構
另一套評分制度
另一個新版產品概念
FINAL 的作用是：
把已經確定的 AMPM 方向施工完成。
如果施工遇到：
路徑不同
程式 bug
adapter 問題
runtime 差異
資料格式差異
就直接做等效修正。
只有真的涉及：
產品方向改變
資料破壞
高風險授權
Production 行為
規格互相衝突
才需要 Owner 決定。
==================================================
1. AMPM 最後要變成什麼
==================================================
AMPM 不再以：
「收錄很多 AI 工具」
當主要定位。
不是：
500+ AI Tools Directory
工具大全
單純工具推薦站
Affiliate 工具清單
AMPM 的核心定位：
「持續監測現在最值得關注的 100 個 AI 工具，
讓使用者知道現在值得看誰、怎麼選、價格發生什麼變化、
誰正在上升、誰正在掉隊。」
正式中文定位：
AMPM 不收錄所有 AI 工具。
我們只追蹤現在最值得關注的 100 個。
英文定位：
AMPM is not a directory of every AI tool.
It is a continuously monitored market of the 100 AI tools worth watching.
品牌 tagline 保留：
Ask More. Pay Minimum.
AMPM 要從 Directory 變成：
AI Tool Decision Platform
+
AI Tool Market Intelligence
==================================================
2. 整個網站不是砍掉重做
==================================================
新產品層建立在現有網站上。
新的核心產品：
AMPM 100
AMPM Radar
AMPM Battles
Ask AMPM
Challengers
AMPM Standard / Transparency
原本網站既有：
Tools
Pricing
Free
Alternatives
Guides
News
Compare
Deals
Categories
全部保留。
它們繼續負責：
搜尋入口
SEO
長尾流量
資料支撐
比較內容
歷史內容
使用者查詢入口
不因 AMPM100 上線就刪掉原本 Tools。
不因 Battles 上線就重建全部 Compare URL。
==================================================
3. AMPM 100
==================================================
AMPM 100 是固定：
100 個 ACTIVE SEATS
不是：
今年 100
以後 130
再變 200
正式發布後：
ACTIVE MEMBERSHIP 永遠維持 100。
新工具不能直接變：
第 101 個。
新工具先進：
Discovery
Watchlist
Candidate
Challenger
達到進場條件後才：
ENTER
ENTER 發生時必須有對應：
DROP
使 Active 總數仍然 = 100。
==================================================
4. 100 是展示上限，不是觀察上限
==================================================
AMPM 可以觀察：
幾百個
幾千個
更多市場工具
但是正式 Active Recognition 只有 100。
所以：
100 = Recognition / Display Cap
不是：
Observation Cap
100 以外仍存在：
Trending Outside 100
Watchlist
Challengers
Dropped
Archive
Closed
Museum
因此 AMPM 不會因為只有 100 席就看不到新工具。
==================================================
5. 不做假的全球第 1～100 排名
==================================================
AMPM 不會把完全不同用途的工具硬排：
全球 #1
全球 #2
全球 #3
……
全球 #100
例如：
Coding #2
Video #2
不需要硬比較：
誰是全球 #17
誰是全球 #18
AMPM 顯示的是：
AMPM 100 Membership
Category Rank
AMPM Score
Category Heat
Competition Index
所以：
Membership = 有沒有進 AMPM100
Rank = 在同類工具裡的位置
Score = AMPM 評分
Heat = 這個市場類別最近熱不熱
Competition = 這個市場類別競爭多激烈
==================================================
6. Category 分類採兩層
==================================================
分類不是只做一層。
正式方向：
L1 = Primary Market Category
L2 = Subcategory / Specialist Market
--------------------------------------------------
L1 Primary Market Category
--------------------------------------------------
每個 Tool 只有一個 L1。
L1 用於：
AMPM100 Seat
Category Rank
Category Heat
Competition Index
ENTER / DROP
正式市場競爭
一個 tool_id 永遠只有：
一個 AMPM100 Seat。
--------------------------------------------------
L2 Subcategory / Specialist Market
--------------------------------------------------
一個 Tool 可以有多個 L2。
用途：
發現特殊需求
細分類工具
Specialist Market
Battle
能力探索
Subcategory Rank
Capability 顯示
例如一個 General AI 可以同時：
Coding
Research
Writing
Multimodal
但是：
四個能力 ≠ 四個席位。
仍然只有一個 Tool、一個 Seat。
==================================================
7. 分類依「使用者需求」，不是公司名稱
==================================================
Category 定義基礎：
使用者拿這個工具主要完成什麼工作。
不是：
哪家公司做的
品牌大不大
是哪種公司
產品名字聽起來像什麼
Generalist 可以存在：
General AI
然後用 Capability Badges 表示：
Coding
Research
Writing
Multimodal
等等。
Specialist 工具則可以存在真正有市場意義的專門 Category。
不能為單一工具硬造分類。
==================================================
8. Generalist / Specialist
==================================================
positioning_type：
GENERALIST
SPECIALIST
UNCLASSIFIED
這不是 L1 Category 本身。
而是工具的產品定位。
positioning_type 不准單靠 AI 推測。
沒有官方證據：
UNCLASSIFIED
positioning_evidence_tier：
UNVERIFIED
VERIFIED
==================================================
9. Capability Badge
==================================================
能力 Badge 有兩個 Evidence Tier：
SHADOW_CAPABILITY_BADGE
VERIFIED_CAPABILITY_BADGE
舊 description 或現有資料推測出來的能力：
只能先是 SHADOW。
找到官方產品頁 / docs / feature evidence：
才能升成 VERIFIED。
不能因為：
「大家都知道 ChatGPT 會這個」
就當正式 Evidence。
==================================================
10. 舊 Category 資料不能假裝已驗證
==================================================
既有 what / host_product / description 等資料：
可以當：
MIGRATED_LEGACY
SHADOW_CLASSIFICATION_INPUT
但不能直接變：
VERIFIED_CATEGORY
如果要真正改 Primary Category：
必須回官方：
產品定位
docs
official product page
官方功能說明
取得 Evidence。
沒有足夠證據就：
CATEGORY_REVIEW_REQUIRED
MANUAL_REVIEW
SHADOW_APPLIED
不能因 AI 覺得某類比較合理就直接覆蓋。
==================================================
11. raw_member_count 與 eligible_count 分開
==================================================
兩個數不能混。
raw_member_count：
這個 taxonomy 裡現在有多少工具。
eligible_count：
真正符合 AMPM100 Active Eligibility、
可以參與正式 Seat Allocation 的工具數。
即使：
raw_member_count 很多
但：
eligible_count = 0
正式 Category Seat Allocation 仍不能假裝成立。
至少：
eligible_count >= 2
才可以正式成為 independently allocated Primary Category。
不足 2：
NOT_INDEPENDENTLY_ALLOCATED
但該 taxonomy / subcategory 仍然可以保留作 Observation。
==================================================
12. AMPM Score V1
==================================================
AMPM Score：
0～100
固定五個主維度：
Utility = 30%
Value = 25%
Accessibility = 15%
Reliability = 20%
Momentum = 10%
公式：
AMPM Score =
Utility × 0.30
+
Value × 0.25
+
Accessibility × 0.15
+
Reliability × 0.20
+
Momentum × 0.10
這套權重已鎖定。
不能：
工程師自己改
AI 覺得不合理就改
為了湊 100 改
為了某品牌改
為 Affiliate 改
為 Sponsor 改
為流量改
==================================================
13. Utility
==================================================
Utility 回答：
這個工具在自己的主要 Category 中，
實際完成工作的價值有多高。
包含：
Core capability fit = 40%
Workflow breadth / completion = 25%
Output / result quality = 20%
Integrations / interoperability = 15%
==================================================
14. Value
==================================================
Value 回答：
相對花的錢，
得到的能力值不值得。
包含：
Price-to-capability efficiency = 50%
Plan flexibility / upgrade friction = 20%
Included usage / limits relative to peers = 20%
Lock-in / cancellation / portability friction = 10%
只有價格資料：
不能假裝 Value 已完整。
完全免費 / Open Source：
也不自動 Value = 100。
==================================================
15. Accessibility
==================================================
Accessibility 包含：
Usable free tier = 50%
Trial / low-risk entry = 20%
Platform / region availability = 20%
Onboarding friction = 10%
沒有免費版：
不是代表產品不好。
只影響 Accessibility。
不能再把同一件事情重複扣 Utility。
==================================================
16. Reliability
==================================================
Reliability 包含：
Product maturity / continuity = 30%
Release / maintenance continuity = 25%
Documentation / support quality = 20%
Platform / service stability evidence = 15%
Policy / pricing continuity = 10%
不能：
因為公司很大
所以 Reliability 自動很高。
需要 Evidence。
==================================================
17. Momentum
==================================================
Tool-level Momentum 是：
工具本身最近可驗證的產品動能。
後續已明確修正：
Search / Demand 不放在 Tool Momentum。
Search Demand 屬於：
Category Heat。
Momentum 不准因為：
搜尋很多
新聞很多
社群很紅
就直接加分。
必須有真正產品 / 市場事件 Evidence。
==================================================
18. Evidence Coverage 不等於產品分數
==================================================
Evidence Coverage：
不直接加 AMPM Score。
原因：
不能讓「資料最好抓的工具」
變成「評分最高的工具」。
Evidence Coverage 是：
Publishability / Eligibility Gate。
也就是：
這個分數能不能相信
能不能公開
能不能進 Active
==================================================
19. UNKNOWN / N/A / MISSING_REQUIRED / CONFLICT
==================================================
這幾種不能混。
N/A：
這項對該產品真的不適用。
UNKNOWN：
理論上應該有資料，
但現在沒有足夠 Evidence。
MISSING_REQUIRED：
Active Eligibility 必要欄位缺失。
CONFLICT：
可信來源對同一個事實出現真正矛盾。
規則：
UNKNOWN 不能補 0。
UNKNOWN 不能補平均。
UNKNOWN 不能叫 AI 猜。
MISSING_REQUIRED：
阻止 Active。
CONFLICT：
直接使 scoreable=false。
不能自己挑一個看起來最合理的答案消除 Conflict。
==================================================
20. Active AMPM100 最低 Evidence 要求
==================================================
Evidence Coverage：
HIGH：
>= 90%
且沒有 Critical Conflict
MEDIUM：
80～89%
或只有非關鍵歧義
LOW：
< 80%
或有 Critical Conflict
Active AMPM100 最低要求：
Coverage >= 80%
另外還必須：
沒有 Critical unresolved conflict
至少 4/5 主維度可形成可信分數
Primary Category 已確認
Identity / product status 已確認
Pricing / Free 在適用時已確認
不能是 LOW confidence
沒有達標：
不能硬塞 Active。
==================================================
21. Tie-break
==================================================
同 Category 同分時排序固定：
1. AMPM Score
2. Confidence
3. Evidence Coverage
4. Momentum
5. stable tool_id
不能使用：
last_verified
slug 隨機順序
random
Affiliate
Sponsor
流量
來決定平手。
==================================================
22. Category Heat V1
==================================================
Category Heat 回答：
「現在這一類 AI 市場真的正在升溫嗎？」
使用：
最近 28 天
vs
前一個 28 天
五個 component：
Verified Event Velocity = 30%
Credible Challenger Growth = 20%
Search / Demand Momentum = 20%
Major Release Intensity = 15%
Price / Free Competition Activity = 15%
每項先 normalization 到 0～100。
如果 component 缺資料：
不補 0。
至少要：
3/5 components
有有效資料才能重正規化。
少於 3/5：
Category Heat =
INSUFFICIENT_DATA
不能因 UNKNOWN 被當成高熱度。
==================================================
23. Competition Index V1
==================================================
Competition Index 回答：
「這一類現在競爭到底多激烈？」
固定概念：
Eligible Depth = 25%
Score Density = 25%
Challenger Pressure = 20%
Price / Free Pressure = 15%
Entry / Drop / Switching Pressure = 15%
不能只用：
「這類工具很多」
當競爭強度。
Heat 與 Competition：
都是 Market State。
不是工具品質分數。
不能混進 AMPM Score 製造循環加分。
==================================================
24. Category Seat Allocation
==================================================
100 席不平均分。
第一步：
只有 eligible_count >= 2 的 Category
才能正式獨立分席。
第二步：
每個 Eligible Category 先給：
2 Base Seats。
BASE_TOTAL =
2 × ELIGIBLE_CATEGORY_COUNT
剩下：
REMAINING =
100 - BASE_TOTAL
第三步：
計算 Allocation Pressure：
Category Heat × 45%
+
Competition Index × 35%
+
Eligible Candidate Depth × 20%
第四步：
剩餘 Seat 使用：
Hamilton / Largest Remainder Method
分配。
要求：
最後加總精確 = 100
不能：
99
101
91
73
==================================================
25. Seat Allocation 限制
==================================================
Category Seat：
不能超過這一類真正 eligible candidate 數。
單一 Category：
V1 最大 20 Seats。
超出的 Seat：
重新分配給其他符合資格 Category。
所有 allocation：
同樣 input
必須能 machine reproducible。
==================================================
26. Seat Stability Guard
==================================================
Heat / Competition 可以每天重算。
每天也可以產生：
shadow_seat_allocation
但是：
Shadow Seat ≠ Production Seat。
正式 Founding100 建立時：
用完整 eligibility + Hamilton
產生第一次正式 seat baseline。
Founding100 正式發布後：
不能因為單日流量或短期 spike
隔天就一直改 Category 席位。
Production Seat Change 必須：
同方向變化
至少連續 3 個 snapshots
持續成立。
一般 cycle：
單一 Category 最多 ±1 Seat。
整體一次：
最多 4 個 Seat movements。
==================================================
27. Seat Stability 的重大例外
==================================================
重大結構事件可以 bypass 一般 Stability：
產品關閉
產品合併
Category 重構
Critical Evidence 確認失效
重大市場結構變化
但必須留下：
reason code
Evidence
Sponsor
Affiliate
社群聲量
都不能成為 bypass reason。
Seat 改變只代表：
Category Capacity 改變。
不代表：
某工具自動 ENTER 或 DROP。
工具仍必須通過：
Active Eligibility
+
deterministic ranking。
==================================================
28. Non-Eviction 原則
==================================================
如果 Category 的目標 Seat 下降：
不是立刻把現有工具踢出去。
先形成：
SEAT_DEFICIT
再依正式評估週期處理。
避免因短期 Seat Allocation 波動直接造成不合理 DROP。
==================================================
29. Founding Selection
==================================================
現有網站工具：
全部先是 Candidate。
不是自動 Founding Member。
Founding Selection：
1. 建 Candidate Pool
2. 現有 tools 全部進 pool
3. 用免費 discovery 掃描市場漏掉的重要工具
4. Candidate 回官方 Evidence
5. 排除 Closed / Duplicate / 無實質產品 / Evidence 不足
6. 建 Category Map
7. 算 AMPM Score / Coverage
8. 算 Heat / Competition
9. 算 Seat Allocation
10. 選真正 Founding 100
11. machine 驗證 Active = 100
不能因現在資料庫只有 79、100 或其他數量：
就直接把它們宣布 Founding。
==================================================
30. Founding Member
==================================================
正式 Founding100 發布後：
標記：
FOUNDING MEMBER 2026
未來就算 DROP：
仍保留曾經是：
Founding Member
的歷史。
不能抹掉。
==================================================
31. Lifecycle
==================================================
既有 Legacy 工具不能因為：
migration 還沒完成
資料缺漏
parser 問題
舊 Evidence 不完整
就自動 DROP。
Legacy 工具先重新驗證。
基本狀態方向：
ACTIVE / CANDIDATE
→ REVALIDATING
重新驗證通過：
ACTIVE_ELIGIBLE
失敗：
QUARANTINED / CHALLENGER
如果正式失去 Seat：
之後仍可以透過 Challenger 重新競爭回來。
==================================================
32. Founding Grace / Revalidation Recovery
==================================================
Founding 初期允許：
較高頻率重新校正。
但是：
不能因 migration gap
直接懲罰 Legacy。
要先分辨：
產品真的變差
和
AMPM 自己還沒有查完。
如果是 AMPM 自己的資料問題：
不能冒充產品下降。
==================================================
33. 新工具的觀察期
==================================================
NEW_CANDIDATE：
先觀察 14 天。
大約：
每 2～3 天一個觀察 cycle。
至少：
3 個獨立 cycles。
如果 14 天後仍有真實不確定：
可以延長一次：
7 天。
新工具流程：
Discovery
→ Screening
→ New Candidate
→ Observation
→ Challenger
→ Qualifying
→ Enter Ready
→ ENTER
不能：
搜尋到一個新工具
今天就直接塞進 AMPM100。
==================================================
34. Watchlist / Challenger
==================================================
不是每個被發現工具都一定變 Challenger。
Evidence 太弱：
Watchlist
或
Rejected / Insufficient Evidence
真正具有競爭資格的：
Challenger
Qualifying
Enter Ready
才進正式 Competition Pressure。
==================================================
35. Museum / Archive
==================================================
產品不是抓不到一次就算死掉。
Museum 判定要有：
至少 3 個不同 weekly deterioration cycles
再加：
Deep Verification。
以下不能算產品衰退：
fetch failure
parser failure
migration failure
AMPM 自己程式壞掉
Archive / Closed / Museum：
不需要像 Active 一樣固定頻率監控。
==================================================
36. Data Engine 的目的
==================================================
Data Engine 的目的不是：
每天叫 Claude 幫 100 個工具人工查價。
而是：
讓機器自己發現真正變化。
基本概念：
machine sees change
rules verify
AI understands important change
AMPM decides
強 AI：
做 Judgment。
不做日常 Crawling。
==================================================
37. Official Source Registry
==================================================
每個 Active Tool
與重要 Challenger
建立官方 Source Registry。
來源：
official pricing
official free / limits
official docs
official help center / FAQ
official changelog
official blog
RSS / Atom
sitemap
official API
GitHub Releases / repo
structured JSON
JSON-LD
==================================================
38. Discovery Source 不等於 Evidence Source
==================================================
SearXNG
Google
搜尋引擎
搜尋摘要
可以：
找網址
發現新產品
發現可能事件
但是：
不能直接變正式 Evidence。
例如：
Search snippet 說：
"$20/month"
不能直接寫進 canonical pricing。
要回：
官方 pricing
官方 docs
官方 API
官方 structured data
驗證。
==================================================
39. Collector 順序
==================================================
優先使用免費 deterministic 方法。
順序概念：
HTTP direct
RSS / Atom
sitemap
official API
structured JSON / JSON-LD
HTML parser
必要時才：
Browser / Playwright
仍然真的需要語意判斷才：
local/free model
最後才：
paid strong AI / human
不能一開始就：
Claude Browser × 100 tools。
==================================================
40. Snapshot / Hash / Diff
==================================================
每次官方來源抓取保存：
source URL
fetched_at
HTTP status
content hash
normalized extract
parser version
然後比：
上一次 snapshot。
沒有實質變化：
NO CHANGE
NO CHANGE：
不呼叫 LLM。
==================================================
41. Data Engine 正式 Pipeline
==================================================
COLLECT
→ NORMALIZE
→ SNAPSHOT
→ DIFF
→ RULE VERIFY
→ CONFIDENCE
→ EVIDENCE QUEUE
→ EVENT
→ PUBLISH QUEUE
任何資料變化：
不能跳過 Evidence。
不能：
crawler 看見價格不同
就直接改網站。
==================================================
42. Confidence
==================================================
至少：
HIGH
MEDIUM
LOW
HIGH：
官方直接來源
結構清楚
重抓一致
可客觀核對
MEDIUM：
官方來源有
但是存在：
Billing
Region
語意
方案
時間
等歧義
LOW：
只有 secondary source
來源衝突
頁面被擋
不能穩定驗證
LOW：
不得自動修改 Public Canonical Fact。
==================================================
43. Two-pass 驗證
==================================================
Two-pass 不准造假。
合法驗證要有：
真實 attempt records。
不能：
同一 Browser
同一頁
連跑兩次
就叫：
兩個獨立 Evidence Channel。
同一資料的 verification：
必須是真正可重新追溯的獨立驗證。
今天已經抓到：
felo 曾出現假的 two-pass。
後續已作廢這種做法。
==================================================
44. Evidence Durability
==================================================
已經合法取得的 verification：
generator 重跑不能自己消失。
但如果原始值真的改變：
舊 verification 也不能盲目沿用。
所以：
資料沒變
→ earned verification 可保持
資料變了
→ verification 必須重新確認
不能：
每重跑 generator
就把 verified 全清掉。
==================================================
45. fact_id
==================================================
同一件 Fact 必須有穩定唯一 ID。
不能因：
Pro
Pro+
中文
特殊字元
清理後碰撞，
造成兩個不同方案被誤判為：
CONFLICT。
Cursor 的：
Hobby
Pro
Pro+
問題就是因此找到 fact_id collision。
這類 collision：
是 Data Engine Bug。
不是產品 Conflict。
==================================================
46. Crawl Resilience
==================================================
已鎖定：
Fetch failure
≠ Product decline
≠ Evidence invalidation
單次或短期：
403
429
5xx
timeout
DNS
Turnstile
Bot Fight
JS rendering failure
parser break
不能直接造成：
Score 降低
Rank 降低
Eligibility 失效
Seat 失效
DROP
==================================================
47. Stale Grace
==================================================
官方來源暫時抓不到：
保留：
last verified snapshot
進入：
Stale Grace
而不是：
把原本合法 Evidence 立刻清零。
如果有 alternate official source：
可以切換。
但重新驗證成功以前：
不能直接改 canonical fact。
==================================================
48. Anti-Cascade
==================================================
如果同一 provider
突然大量抓取失敗：
不能讓：
Rank
Seat
Membership
一起連鎖大變動。
要暫停這類 mutation，
先判斷：
是產品真的全部變了
還是 crawler / provider / network 壞掉。
==================================================
49. Radar
==================================================
Radar 不是一般 AI News Feed。
Radar 只記：
會改變使用者選擇
成本
可用性
或 AMPM 市場判斷
的事件。
Event Type：
PRICE
FREE
MODEL
FEATURE
ENTER
DROP
WATCH
RANK
DEAL
CLOSED
TRENDING
Radar 公開：
/radar/
每一筆 Radar：
必須能回 Evidence。
不能 AI 自己說：
「這工具最近很熱門」
就生 Radar。
==================================================
50. Radar Event Flow
==================================================
正式內容鏈：
Observed Change
→ Evidence
→ Verified Event
→ Radar
→ 必要時 News
→ 高影響才 Column / Research
→ Rank / Battle Re-evaluation
NO CHANGE：
不產生內容。
很小的低價值更新：
不自動生成長文章。
==================================================
51. Radar 還要做什麼
==================================================
Radar Event 可以觸發：
相關 Tool 重新評估
相關 Guide 重新檢查
相關 Compare 重新檢查
相關 Battle 重新計算
AMPM100 影響
News queue
Column / Research queue
share asset
RSS / Atom
social distribution queue
但是：
只有 Verified Event 才能進公開 Feed / Social Queue。
==================================================
52. News
==================================================
News 回答：
「發生了什麼？」
不是：
為了 SEO 大量自動生成薄文章。
News 必須來自：
真正事件。
資料來源不足：
不能靠 AI 標題擴寫。
==================================================
53. Column / Research
==================================================
Column / Research 回答：
「這件事為什麼重要？」
不是每個 Radar 都需要 Column。
只有高影響事件：
才升級。
==================================================
54. AMPM 的內容鏈
==================================================
內容不再互相獨立。
正式關係：
Radar：
發生什麼變化
News：
完整事件
Column / Research：
為什麼重要
AMPM100：
這有沒有影響排名 / Seat / 選擇
Battles：
這有沒有改變 A vs B 結論
==================================================
55. 貓日報
==================================================
貓日報不再強迫：
每天生 AI 垃圾內容。
方向：
Event-driven editorial / newsletter。
資料來源：
Data Engine
→ Radar
→ 貓日報
→ Email / Social / RSS / OG
→ 流量回 AMPM
初期：
Free weekly roundup
+
重大事件 breaking alerts
未來才可能有：
Pro。
==================================================
56. 未來貓日報 / Pro 概念
==================================================
免費：
幫你知道發生什麼。
Pro：
幫你知道該怎麼選。
可能包含：
完整市場週報
價格歷史
Category Heat
Challenger / ENTER Preview
深度 Battles
決策建議
這是後續商業方向，
不是現在靠大量內容硬上付費。
==================================================
57. Battles
==================================================
Battles 是：
真正有決策價值的比較。
不是：
把所有 A vs B 模板全部換皮。
既有 Compare 分三層：
Tier A：
真正 Battle
Tier B：
Useful Indexed Comparison
Tier C：
Thin / Weak Candidate
Tier C：
不能直接批量 noindex。
必須先看 GSC。
==================================================
58. Battles 必須使用 Evidence
==================================================
Battle 要有：
Battle template
scorecard
evidence-backed verdict
價格或 Free Plan 發生重要變化：
Battle verdict 可以重新計算。
Verdict：
必須回 canonical data。
不能：
Affiliate
Sponsor
人工偏好
決定勝負。
==================================================
59. Battles 不准星狀退化
==================================================
後續 QA 已經抓到：
例如 Coding 6 組全部：
aider vs X
這種 pairing 會造成單一工具壟斷曝光。
已經改成：
更均衡、deterministic 的 pairing。
不能讓商業欄位影響 pairing。
==================================================
60. Ask AMPM
==================================================
Ask AMPM 不靠：
模型記憶。
回答順序：
Canonical Data
→ Evidence
→ AMPM Standard
→ Battles
→ Radar
模型只能：
理解
整理
說明
不能：
自己補 Facts。
==================================================
61. Ask AMPM 遇到不知道
==================================================
資料不足：
回答：
目前證據不足 / 尚未確認。
多來源衝突：
顯示：
Conflict / Uncertainty。
不能自己挑：
看起來最合理的答案。
==================================================
62. Ask AMPM 問到資料庫外工具
==================================================
可以回答：
Outside 100
Not Tracked
Watchlist
Not Enough Evidence
不能：
假裝它是 AMPM100 Member。
==================================================
63. Ask AMPM Paid AI 掛掉
==================================================
Paid Model unavailable：
Ask 不能整個死掉。
要有：
deterministic data fallback。
因此：
Paid AI 不是 Ask 的核心生存依賴。
==================================================
64. AMPM Standard / Transparency
==================================================
公開 Transparency 要說清楚：
AMPM100 怎麼選
Score 怎麼算
哪些是客觀資料
哪些是 Editorial Judgment
Evidence 怎麼驗證
Confidence 怎麼分
多久重查
錯誤怎麼更正
Commercial Independence
Affiliate / Sponsor 如何隔離
Methodology Version
Change Log
主要公開 URL：
/transparency/
==================================================
65. Challenger
==================================================
Challenger 顯示：
正在 AMPM100 外面，
但有可能搶 Seat 的工具。
不是任何新工具都叫 Challenger。
它必須具有：
一定 Evidence
競爭資格
足夠市場意義
==================================================
66. ENTER / DROP
==================================================
ENTER / DROP 是市場事件。
不是人工按一下。
正式發生時要留下：
時間
原因
Score
Rank
Category
Evidence
當時 Seat 狀態
競爭者
歷史
ENTER + COMPETITIVE_DROP：
在正式 evaluation 中應該是 atomic change。
不能 ENTER 完了 Active 變 101。
==================================================
67. Affiliate / Sponsor / Ads 完全隔離
==================================================
AMPM 可以賺錢。
可以有：
Affiliate
Google Ads
Sponsored Placement
未來 Pro
未來 Data/API
但是：
Affiliate
Sponsor
Ads
全部不能影響：
AMPM Score
Category Rank
AMPM100 Seat
ENTER
DROP
Battle Verdict
Ask Recommendation Weight
Evidence 判斷
原則：
先排名
後變現。
==================================================
68. Affiliate Lifecycle
==================================================
Affiliate 狀態：
NONE
→ DISCOVERED
→ APPLY_REQUIRED
→ PENDING
→ ACTIVE
→ BROKEN
→ CLOSED
Agent 可以：
自動發現 affiliate program。
但是：
Discovery ≠ Approval。
不能偽造 referral URL。
==================================================
69. Affiliate Resolver
==================================================
ACTIVE：
CTA 統一走：
/go/{tool-slug}/
不是 ACTIVE
或 link broken：
Fallback：
Verified Official URL
不能讓使用者進死連結。
每日檢查：
HTTP
redirect chain
destination domain
status
last_checked
consecutive failures
==================================================
70. Affiliate Owner-only
==================================================
以下一定 Owner-only：
OTP
2FA
KYC
身分文件
稅務
銀行
付款帳戶新增
法律合約接受
Agent 不得自己完成。
Private affiliate profile / payout / KYC 資料：
不能進：
public repo
public build
public log
debug report
==================================================
71. Murf AI
==================================================
Murf AI 已由 Owner 提供正式 Partner Approval。
Referral：
https://get.murf.ai/r0mnpebg2adn
既有 affiliates.json 的 murf-ai：
從 PENDING 更新為 ACTIVE。
不需要改 tools.json。
不建立重複 Affiliate Schema。
前台仍由：
/go/murf-ai/
Resolver 控制。
==================================================
72. AdSense
==================================================
AdSense 最近實際退件原因：
缺乏價值的內容
Low Value Content
所以：
不能把：
cookie consent 修好
privacy 補完
disclosure 存在
ads script 正確
直接說成：
AdSense 一定 Ready。
==================================================
73. AdSense 要分兩層
==================================================
ADSENSE_TECHNICAL_READINESS
和
ADSENSE_CONTENT_VALUE_READINESS
分開。
目前施工確認：
Technical：
已做到同意後載入 Ads、
Disclosure、
Privacy、
Contact、
/go/ noindex 等技術項目。
但是 Content Value：
要看真正網站內容。
==================================================
74. AdSense Content Value 真正要補的是什麼
==================================================
需要真正出現：
AMPM 自己的 Verdict
Verified Evidence
可用 AMPM100
有決策價值的 Battles
Radar
News / Research
不是單純工具清單
不是 Affiliate Bridge
所以：
技術 PASS
不等於：
Google 一定會核准。
目前不能因技術修好就重新送審。
==================================================
75. Homepage
==================================================
首頁要從：
工具目錄入口
升成：
AMPM Decision Platform 入口。
保留：
AMO
PIMI
原本 Logo
九宮格品牌語言
不是把品牌全部改掉。
==================================================
76. 九宮格
==================================================
九格對應：
AMPM100
Radar
Battles
Ask
Free Watch
Price Watch
Trending
Challengers
Standard
視覺方向：
可以變亮
更鮮明
更有科技感
但：
不能亂成彩虹。
保留同一套品牌感。
==================================================
77. Navigation
==================================================
主要入口：
AMPM100
Radar
Battles
Tools
Free / Pricing
News / Guides
Ask
Transparency
使用者進站應能快速理解：
AMPM 是做什麼的。
==================================================
78. AMO / PIMI
==================================================
AMO / PIMI 是 AMPM 自有 IP。
保留。
第三方 Tool Logo / Brand：
不能讓人誤以為是 AMPM 自有品牌。
==================================================
79. SEO 原則
==================================================
這次：
產品轉型 ≠ SEO Reset。
不是：
重新做一次 SEO。
既有重要 URL：
/tools/:slug/
/guides/:slug/
/compare/:slug/
既有語系 URL
全部優先保護。
==================================================
80. Phase 1 SEO Freeze
==================================================
目標：
unexplained REMOVED = 0
unexplained MOVED = 0
不做：
mass URL rename
mass canonical change
mass noindex
mass delete
無證據搬 URL
==================================================
81. Compare SEO
==================================================
新 Battles：
不能因此把所有：
/compare/:slug/
重建。
原 URL 原則上保持。
Thin / Weak Compare：
要先看 GSC。
不能 AI 看內容短：
就直接 noindex。
==================================================
82. SEO Opportunity Engine
==================================================
利用既有 GSC 資料建立：
Freeze Map
Opportunity Map
CTR Leak Map
Rising Query Map
Rising Page Map
優先原則：
先把 Google 已經願意測的頁面往前推。
不是：
每天再生 100 個新頁。
==================================================
83. Language Strategy
==================================================
zh-Hant：
Primary。
English：
Global / Secondary。
Japanese：
Maintenance / Selective Expansion。
Korean：
Freeze Expansion。
不能：
刪現有 ja / ko URL。
也不再：
無差別大量擴張韓文內容。
==================================================
84. SEO 上線後觀察
==================================================
正式 deploy 之後才開始：
D+1 / D+3：
事故檢查
D+7：
Injury Check
D+14：
Early Benefit Check
D+28：
First Real Evaluation
D+90：
更完整評估
不能：
看一天流量掉
就宣告策略失敗。
主要看：
moving average
GSC query/page trend
CTR
position
index/canonical 狀態。
==================================================
85. Analytics
==================================================
Cloudflare Visits：
不能直接當真人。
流量分：
HUMAN
VERIFIED_SEARCH_CRAWLER
AMPM_INTERNAL
OTHER_AUTOMATION
AMPM Internal 至少包括：
Data Engine
Link Sentinel
Health Check
Pricing / Free collector
VPS known traffic
Audience Dashboard：
優先看 HUMAN。
==================================================
86. 404
==================================================
不能看到很多 404：
全部 redirect 首頁。
404 必須分類：
bot scan garbage
old valid URL
bad internal link
missing asset
stale sitemap / redirect
language route
malicious probing
只有真正有價值舊 URL：
才做對應 redirect。
垃圾 bot URL：
不建立幾千條 redirect。
==================================================
87. Survival Architecture
==================================================
網站不能依賴：
Paid VPS
才能活。
正式公開生存層：
Git Source / Data
→ Hugo Static Build
→ Cloudflare Pages
→ ampm-aiops.com
VPS：
Worker。
Windows：
Worker。
免費 compute：
也可以當 Worker。
==================================================
88. Worker 掛掉時
==================================================
如果 VPS / Windows worker 掛掉：
網站仍在線。
最後一次 Verified Data：
仍然能讀。
只是：
更新暫停。
所以：
VPS 不是唯一 Storefront。
==================================================
89. Domain / SEO 資產優先
==================================================
如果未來真的只能選：
VPS 費用
或
Domain 續費
優先：
Domain / SEO Asset。
不能為了 VPS：
讓 Domain / 搜尋資產消失。
==================================================
90. Paid AI 也不能是生存依賴
==================================================
硬目標：
NO PAID-AI RUNTIME DEPENDENCY。
即使：
Claude
OpenAI
Codex
Anthropic
額度歸零：
網站仍在線。
AMPM100 仍可顯示。
Verified Data 仍可讀。
Deterministic Data Engine 仍可運作。
只有：
真正困難語意判斷
才進 queue / HOLD。
==================================================
91. Growth / Distribution
==================================================
Verified Radar Event 可以產生：
RSS / Atom
share asset
OpenGraph
distribution queue
social-ready content
Social API 掛掉：
不能阻塞 Radar。
可以降級成：
READY_TO_POST
核心產品仍然正常。
==================================================
92. AMPM100 Badge / Verification
==================================================
可以建立：
AMPM100 Badge
Verification endpoint
backlink / public verification
但：
Badge
Backlink
Social Traffic
全部不能回灌：
Score
Rank
Seat
避免變成：
誰幫 AMPM 宣傳
誰排名比較高。
==================================================
93. 現有網站基礎不是從零開始
==================================================
現有 Repo 已經有：
tools.json
tool_health
labels
plan_details
free_details
compare_dialogue
cat_reviews
news
affiliates
i18n
noindex_en
現有 Layout 已有：
tools
compare
free
alternatives
categories
news
guides
deals
audit
robots
sitemap
Ask
picker
rating
現有腳本包括：
add_tool
completeness
data check
freshness
link check
sitemap check
daily price/free
hourly discovery
GSC
news fetching
pricing
maintenance
self-check
所以這次不是：
全部砍掉重寫。
而是：
把現有基礎接成新的 AMPM Decision Platform。
==================================================
94. 目前正式 Gate 順序
==================================================
Gate 0：
Baseline / Restore
Gate 1：
Canonical Data
Gate 2：
Data Engine
Gate 3：
Evidence
Gate 4：
AMPM Standard
Gate 5：
Market Intelligence
Gate 6：
Founding 100
Gate 7：
AMPM100 UI
Gate 8：
Radar
Gate 9：
Battles
Gate 10：
Homepage / Nav / Brand
Gate 11：
Ask AMPM
Gate 12：
SEO / GSC
Gate 13：
Analytics / 404
Gate 14：
Self Audit
Gate 15：
Final Regression
Gate 16：
Production Deploy
Gate 17：
Post-launch Observation
==================================================
95. Gate 16
==================================================
Gate 16 永遠不是 Agent 自動 PASS。
Production Deploy：
必須 Owner 當下明確批准。
正式 deploy：
走：
/root/deploy_guard.sh
不能：
AI 自己覺得做好了
就發布。
==================================================
96. Owner STOP
==================================================
最高優先：
Owner STOP。
如果 Owner 說：
停
立即停。
Task Completion：
不能壓過 STOP。
==================================================
97. Low-risk / High-risk
==================================================
低風險：
可回滾
規格明確
普通 bug
adapter
parser
一般 code fix
validation fix
工程 Agent 自己做。
不用：
每一步問 Owner。
高風險：
destructive
reset / clean
大量刪除
大量 rename / move
force push
DNS
Production Deploy
mass URL
canonical
noindex
付款
OTP
KYC
法律授權
才需要 HOLD。
==================================================
98. 工程 Agent 原本應有的工作方式
==================================================
FINAL 本來就寫：
自己能查的事情自己查。
不能把 Owner 當：
Terminal Operator
Log Collector
Debug Relay。
低風險工作：
直接做。
每個 Gate PASS：
自動下一 Gate。
Codex 不在：
不是停工理由。
Worker 交件：
主 Orchestrator 必須自己驗證。
不能：
一直重新規劃 AMPM。
==================================================
99. 現在真正的資料原則
==================================================
整套 AMPM 最核心的資料要求：
公開的事實與決策必須可追溯。
包含：
價格
Free
方案
功能
Badge
Category
Score
Rank
Heat
Competition
ENTER
DROP
Radar
Battle Verdict
Ask Answer
沒有 Evidence：
不能假裝是 Verified Fact。
資料不足：
UNKNOWN
REVIEW_REQUIRED
INSUFFICIENT_EVIDENCE
都是合法結果。
==================================================
100. 目前施工中已經發現並修過的重要問題
==================================================
已實際抓到過：
fact_id collision
Hamilton Seat Allocation 加總錯誤
evidence generator 重跑會清掉 earned verification
felo 假 two-pass
Battle pairing 星狀退化
acceptance test 用 flag 驗證 flag
sitemapindex 假檢查
Browser 被錯當 default collector
這些都不是重新設計產品。
是施工時發現：
實作沒有符合原本已定策略
所以修正。
==================================================
101. Cost Architecture 最後方向
==================================================
機械工作：
程式做。
一般抓取：
免費做。
規則：
程式做。
Local Qwen：
處理中間難度。
Strong AI：
只處理真正需要理解 / 判斷的事情。
最終目的：
付費 AI 越來越不像 Runtime Dependency。
把付費 AI 時間：
拿來建機器。
不是：
永遠讓 AI 人工操作網站。
==================================================
102. AdSense 與產品價值的關係
==================================================
AMPM 要解掉 Low Value Content：
不能只靠：
多寫文章
補法律頁
塞廣告
增加工具數
真正要出現的是：
AMPM 自有 Market Data
Verified Evidence
History
Score
Category Rank
Heat
Competition
Challenger
ENTER / DROP
Radar
Battle Verdict
AMPM Decision
Original Research / Column
也就是：
從「別人資料的工具目錄」
變成：
「AMPM 有自己持續監測、驗證與判斷的市場資料」。
==================================================
103. 最終使用者應該感受到什麼
==================================================
使用者來 AMPM：
不是只看到：
「這裡有很多 AI 工具。」
而是可以知道：
現在值得看哪些工具
哪些真的有免費方案
價格最近有沒有變
哪個 Category 正在變熱
哪個工具在上升
哪個 Challenger 快進榜
誰剛 ENTER
誰被 DROP
A 和 B 現在怎麼選
這個結論根據什麼 Evidence
資料最後什麼時候驗證
AMPM 為什麼這樣判斷
==================================================
104. 整套策略最終關係
==================================================
Official Sources
↓
Data Engine
↓
Snapshot / Diff
↓
Evidence
↓
Confidence / Conflict / Freshness
↓
Verified Facts
↓
AMPM Standard
↓
AMPM Score
↓
Category Rank
↓
Category Heat / Competition
↓
Seat Allocation
↓
Candidate / Challenger / Active
↓
AMPM100
↓
ENTER / DROP
↓
Radar
↓
News / Column / Research
↓
Battles
↓
Ask AMPM
↓
使用者決策
↓
SEO / Social / Newsletter / Affiliate / Ads
其中：
Affiliate / Ads / Sponsor
只能存在於最後的商業層。
不能反過來污染：
Evidence
Score
Rank
Seat
ENTER
DROP
Battle
Ask。
==================================================
105. 最終原則
==================================================
AMPM 不靠：
工具數量最多
建立價值。
AMPM 靠：
固定 100 席
持續監測
官方證據
價格 / 免費變化
歷史
Score
Category Competition
Challenger
ENTER / DROP
Radar
Battles
Ask
公開 Standard
建立差異。
100 是：
市場選擇制度。
Evidence 是：
公信力基礎。
Radar 是：
變化層。
Battles 是：
決策層。
Ask 是：
查詢層。
Tools / Pricing / Free / Guides / News / Compare：
是資料與 SEO 支撐層。
Affiliate / Ads：
是變現層。
Paid AI / VPS：
都不能成為網站能不能活的單點依賴。
==================================================
106. 這次策略沒有包含的事情
==================================================
沒有決定：
把網站全部換成另一套 framework。
沒有決定：
砍掉 Hugo 重做。
沒有決定：
砍掉原本 SEO URL。
沒有決定：
為了 AMPM100 刪除 Tools。
沒有決定：
所有 Compare 都 noindex。
沒有決定：
大量生成薄頁。
沒有決定：
用 Affiliate 排名。
沒有決定：
讓 Claude 每天人工爬 100 工具。
沒有決定：
為了湊 100 降 Evidence 標準。
沒有決定：
建立 FINAL_v2。
沒有決定：
現在直接 Deploy。
==================================================
107. 目前最重要的施工事實
==================================================
AMPM 的產品方向已定。
現在剩下的核心工作不是重新想策略。
而是讓現有系統真正產生足夠：
Verified Evidence
Verified Category
Verified Capability
Scoreable Dimensions
Active Eligible Candidates
真正 Founding Selection
可用 AMPM100
有 Evidence 的 Radar
有 Evidence 的 Battles
有 Evidence 的 Ask
原創決策內容
直到系統能真正回答：
「為什麼它進 AMPM100？」
「依據什麼？」
「同 Category 為什麼排這裡？」
「最近發生什麼？」
「這個 Battle 為什麼這樣判？」
「證據在哪裡？」
這才是昨天到今天已經定下來的 AMPM。

這份的 FINAL 核心內容可直接對到正式工單：產品轉型範圍、AMPM100、Radar、Battles、Ask、Evidence、SEO、生存架構與商業隔離均已寫入 FINAL。 Data Engine 的官方來源、Collector、Snapshot/Diff、Confidence 與「NO CHANGE = 0 LLM」也來自正式工單。 AMPM_FINAL_MASTER_TRANSFORMATION_WORK_ORDER_20260819_DRAFT.md Score 固定權重與 UNKNOWN/Eligibility 規則同樣已在 FINAL 鎖定。 Category Heat、Seat Stability、Affiliate Automation 與 Crawl Resilience 是同一 FINAL 後續硬化內容，不是另開版本。 SEO 與 Survival Architecture 也明確要求保留既有 URL、Cloudflare Pages 作 Public Site、VPS/Windows 作 Worker。
