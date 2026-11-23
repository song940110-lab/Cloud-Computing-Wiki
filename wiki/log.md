# Wiki Operation Log

## 專案初始化
- 主題：雲端運算（Cloud Computing）
- 方法參考：Andrej Karpathy 的 LLM Wiki
- 資料來源策略：官方文件＋技術教學文章
- 預計來源：7 篇
- Wiki 深度：基礎概念＋技術原理

## [2026-11-24] CC-002～CC-007 批次 Ingest 與整合
- CC-002：Google Cloud, What is Cloud Computing?（線上官方文章）
- CC-003：NIST SP 500-292, NIST Cloud Computing Reference Architecture（35 頁，2011 年 9 月）
- CC-004：NIST SP 800-146, Cloud Computing Synopsis and Recommendations（81 頁，2012 年 5 月）
- CC-005：Google Cloud, What is Cloud Architecture?（線上官方文章）
- CC-006：NIST SP 500-322, Evaluation of Cloud Computing Services Based on NIST SP 800-145（27 頁，2018 年 2 月）
- CC-007：Google Cloud, Shared Responsibilities and Shared Fate on Google Cloud（線上官方文章；頁面標示最後審閱日期 2023-08-21）

### 本輪新增與更新
- 新增六篇來源摘要頁：`wiki/sources/CC-002` 至 `CC-007`
- 更新基本概念、服務模式、部署模式及架構頁
- 新增安全及實際應用知識頁
- 更新 Index、Overview 及 Log

### 主要整合發現
- CC-003 將雲端參考架構整理為五種參與者及雲端供應商的架構元件。
- CC-004 從 SaaS、PaaS、IaaS 的環境分析效益、問題及建議，並討論效能、可靠性、經濟、法規與資訊安全議題。
- CC-005 以 Google Cloud 的角度說明前端、後端、網路、虛擬化、管理及安全等架構元件。
- CC-006 提供依 NIST 五項特徵、服務模式及部署模式評估雲端服務的工作表。
- CC-007 說明 Google Cloud 的 shared responsibility 與 shared fate，並指出不同服務模式下責任分配不同。

### 來源限制
- CC-002、CC-005、CC-007 為線上文章來源紀錄；摘要依官方網頁內容整理，未保存或複製全文。
- CC-007 的 Shared Fate 為 Google Cloud 自身提出的合作安全概念，需與通用 shared responsibility 概念區分。
- CC-004 發布於 2012 年；不應將其內容當作目前所有雲端產品的最新狀態。
- Google Cloud 入門文章的部署模式介紹未列 Community Cloud；Wiki 以 NIST 四種部署模式作為正式分類。

## Lint 紀錄
- 已建立相對連結及來源頁面。
- 本次尚未執行自動化連結檢查或完整語意 Lint；需在本機套用後再進行最終檢查。

## [2026-11-24] lint-and-correction | Wiki 七篇來源核對
- 狀態：完成修正套件；待使用者套用後進行本機最終檢查
- 檢查範圍：`wiki.zip`、`raw.zip`、`AGENTS.md` 及四份 NIST PDF 原文
- 原始來源確認：CC-001、CC-003、CC-004、CC-006 PDF 可讀取；CC-002、CC-005、CC-007 為線上文章來源紀錄，需以官方網頁作為原文，未複製全文
- 修正項目：
  - 補回 `sources/CC-001_NIST_SP_800-145.md`
  - 補齊 NIST 官方 DOI、作者、發布日期、文件頁數及可讀取範圍
  - 補齊 Google Cloud 來源網址、來源類型及本次取得日期
  - 更新 `index.md`，列出每個知識頁及七份來源摘要頁的用途
  - 在主題頁增加可追溯的 Source ID 相對連結
  - 將 raw 中 CC-002 檔名統一為 `CC-002_Google_Cloud_Computing.md`
- 保留事項：
  - 原有紀錄未刪除；本筆為追加紀錄
  - Google Cloud 文件仍標示為供應商觀點
  - NIST 四種部署模式仍作為 Wiki 正式分類
- 待處理：
  - 使用者套用後，需在實際編輯器環境再檢查連結及 AGENTS.md 規範
  - HTML 與 PDF 尚未製作

## [2026-11-24] historical-record-recovery | CC-001 | The NIST Definition of Cloud Computing
- 狀態：補登先前已確認的 Ingest 紀錄
- 依據：先前交付的 CC-001 更新套件中保留的 `log.md` 歷史內容
- 來源：NIST Special Publication 800-145；Peter Mell、Timothy Grance；2011 年 9 月
- 原始檔案：`raw/CC-001_NIST_SP_800-145.pdf`
- 當時建立／更新頁面：
  - `wiki/sources/CC-001_NIST_SP_800-145.md`
  - `wiki/concepts/cloud-computing.md`
  - `wiki/service-models/overview.md`
  - `wiki/deployment-models/overview.md`
  - `wiki/architecture/cloud-infrastructure.md`
  - `wiki/index.md`
  - `wiki/overview.md`
- 核心發現：NIST 定義包含五項基本特徵、三種服務模式及四種部署模式；並以實體層與抽象層說明雲端基礎設施。
- 未解決問題：原始文件未深入說明虛擬化技術、安全管理及完整應用案例。
- 註記：此筆為依先前交付版本補登的歷史紀錄，不代表本次重新執行 CC-001 Ingest。
