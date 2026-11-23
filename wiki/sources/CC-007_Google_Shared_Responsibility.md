# CC-007｜Shared Responsibilities and Shared Fate on Google Cloud

## 來源資訊
- 文件名稱：Shared Responsibilities and Shared Fate on Google Cloud
- 發布機構：Google Cloud
- 文件類型：Google Cloud 官方安全架構文件
- 原始網址：https://docs.cloud.google.com/architecture/framework/security/shared-responsibility-shared-fate
- 取得方式：線上閱讀官方頁面
- 取得日期：2026-11-24
- 發布日期：官方頁面未在本次來源紀錄中確認；不臆測。
- 原始內容：保留官方網頁，不另行複製全文

- 發布機構：Google Cloud
- 文件類型：官方技術教學文件
- 原始網址：https://docs.cloud.google.com/architecture/framework/security/shared-responsibility-shared-fate
- 取得方式：線上閱讀
- 使用方式：閱讀、摘要及來源引用
- 原始內容：保留官方網頁，不另行複製全文
- 網頁標示最後審閱日期：2023-08-21

## 摘要
文章說明 Google Cloud 的 Shared Responsibility 與 Shared Fate。Shared Responsibility 用來描述客戶與雲端供應商在雲端安全上的任務分工；客戶需要了解其工作負載、服務設定、法規義務、組織安全標準及風險管理要求，並選擇與配置適當的安全控制。

## 依服務模式的責任概念（Google Cloud 的例子）
- **IaaS**：客戶承擔大部分安全責任；Google Cloud 負責底層基礎設施及實體安全。
- **PaaS**：供應商負責更多控制；應用層控制及 IAM 可能由雙方共同負責，客戶仍負責資料安全與用戶端保護。
- **SaaS**：供應商承擔大部分安全責任；客戶仍負責存取控制及其存放資料。
- **FaaS／Serverless**：文章指出其責任分配與 SaaS 有相似之處。

文章亦指出，供應商負責底層網路與基礎設施，客戶負責自己的存取政策及資料。

## Shared Fate
Google Cloud 將 Shared Fate 描述為比單純列出責任更緊密的安全合作方式，包括提供可信任平台、最佳實務指引、安全基礎設施程式碼、整合式安全解決方案，並與客戶合作處理安全挑戰。

## 其他考量
責任還會受到工作負載、產業法規、資料所在地及各項服務設定影響。文章提到錯誤設定、跨多項服務的控制重疊、法規變動及加密金鑰管理等挑戰。

## 對應 Wiki
- 安全：共同責任、Shared Fate、資料與存取控制。
- 服務模式：不同模式下的責任差異。

## 來源界線
Shared Fate 是 Google Cloud 提出的供應商合作安全觀點，不是 NIST 定義的通用服務模式或所有供應商共用的標準。各服務實際責任須依該服務的文件及合約確認。
