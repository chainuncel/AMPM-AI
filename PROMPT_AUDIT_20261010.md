# Prompt Audit 報告（2026-10-10）

依 `/claude-api prompt-audit` 流程執行。本報告只稽核、不修改任何既有檔案。

## 前提假設（Step 0）

**範圍**：本倉庫工作目錄（分支 `claude/api-prompt-audit-844zpe`，commit `1a0fb69`）的全部 prompt surface。

**盤點結果（Step 1）**：倉庫只有 2 個 tracked 檔案，兩者都不是會送進模型的文字。

| 類別 | 本倉庫 |
| --- | --- |
| System prompt／組裝程式 | 無 |
| Tool definitions | 無 |
| Agent 設定檔（`CLAUDE.md`、`AGENTS.md`、`.claude/`、skills、rules、commands、subagents） | 無 |
| Request-building code（model ID、thinking、sampling、beta header） | 無（倉庫內沒有任何程式碼） |
| Few-shot／embedded examples | 無 |
| `README.md` | 倉庫說明，不是 prompt |
| `AMPM_AIOPS_DECIDED_STRATEGY_RECORD_20260818-20260819.md` | 策略記錄的逐字歸檔（README 與第 0 節都寫明「整理記錄，不是新版本」），不會被任何程式或 Agent 自動載入 |

**目標模型**：倉庫內沒有程式碼指定模型，請求本身也沒有指定。如果把策略記錄當成 coding agent 會讀的文字，就以執行本次稽核的模型 Claude Opus 5.5 為目標。

**非 Anthropic 供應商標記**：策略記錄 §90、§98、§101 提到 OpenAI、Codex、Local Qwen。這屬於多供應商的成本架構（硬目標是「NO PAID-AI RUNTIME DEPENDENCY」）。本報告只記錄這點，不建議改用其他供應商。

**Provenance（Step 2）**：兩個檔案的全部行數（13 + 2044 行）都來自同一個 commit `1a0fb69`（2026-08-19），沒有逐行演進的歷史可以追溯。

**略過、不在範圍內的檔案**：真正的 prompt surface 不在本倉庫，以下都沒有讀取：

- `ampm-site` 程式碼（VPS `/opt/ampm/heiyao/AMPM-AIOPS/ampm-site`）。根據 §93，裡面有 Ask layout、`compare_dialogue`、`cat_reviews`、news fetching、pricing 等腳本，如果有呼叫 LLM，system prompt 和 request code 會在這裡。這個 repo 不在本 session 可存取的 GitHub 清單中。
- VPS `/root/絕對法則/`：`絕對法則.md`（治理正本，`/root/開工儀式.md` 指向它）、`硬規矩.md`、`共同記憶.md`（約 400 KB）、`專欄編輯方針.md`、`品牌規格_AMPM.md` 等。檔案清單出自分支 `claude/absolute-rules-compliance-y80kpo` 的 `WORK_ORDER_STATUS_20260917.md`，屬於 Agent 指令面。
- `AMPM_FINAL_MASTER_TRANSFORMATION_WORK_ORDER_20260819_DRAFT.md`（正本在 VPS）。
- 分支 `claude/absolute-rules-compliance-y80kpo` 新增的 `WORK_ORDER_INDEX.md`、`WORK_ORDER_STATUS_20260917.md`：不在本分支範圍內。已經 grep 過，裡面沒有任何 prompt 或模型設定標記，內容是工單索引和盤點。

## 結果

**本倉庫的 prompt surface 是乾淨的：沒有需要移除或改寫的 dated pattern，proposed diff 為空。**

| Group | 結果 |
| --- | --- |
| 1 Dated prompt text | 0 |
| 2 Skill／設定檔 | 0 |
| 3 Tool descriptions | 不適用（無 tool definitions） |
| 4 Request config／架構 | 不適用（無 request-building code） |

策略記錄裡寫給模型或 Agent 的規範，都依 keep list 保留：

- §60～§63「Ask AMPM 不靠模型記憶、不能自己補 Facts、衝突時不挑答案」：這是產品政策與可追溯要求（§99），屬於只有作者知道的 context，不是寫給舊模型的 workaround。
- §95～§97「Gate 16 必須由 Owner 當下批准、Owner STOP、高風險 HOLD」：屬於 fragile operation 與安全規則，維持精確規定是正確的。
- §43、§45、§59、§100 的事件紀錄（felo 假 two-pass、fact_id collision 等）：放在指令檔裡會算 history narrative，但這份檔案的功能本來就是歸檔記錄，所以不適用。

## Proposed diff

（空）

## 下一步

要稽核真正的 prompt surface，需要把以下內容放進本 session 可存取的範圍（例如推上 GitHub repo），再重跑 `/claude-api prompt-audit`：

1. `ampm-site` 中 Ask AMPM 與內容生成腳本的 system prompt 和 API 呼叫程式碼（屬於 Group 1、3、4）。
2. `/root/絕對法則/` 底下的 Agent 指令檔（屬於 Group 1、2）。其中 `共同記憶.md` 約 400 KB，如果每次 session 都會載入，就特別值得檢查。
