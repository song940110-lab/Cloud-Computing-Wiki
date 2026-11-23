# 雲端服務模式（Cloud Service Models）

NIST SP 800-145 定義三種主要雲端服務模式：SaaS、PaaS、IaaS。差異在於供應商提供的能力，以及使用者可管理或控制的範圍。

## 1. SaaS（Software as a Service，軟體即服務）

來源依據：[CC-001](../sources/CC-001_NIST_SP_800-145.md)；技術與風險補充：[CC-004](../sources/CC-004_NIST_SP_800-146.md)，第 5 節。（Software as a Service，軟體即服務）
供應商提供在雲端基礎設施上執行的應用程式，使用者透過用戶端介面存取。使用者通常不管理底層網路、伺服器、作業系統及儲存空間，對應用程式設定的控制也較有限。

## 2. PaaS（Platform as a Service，平台即服務）
使用者將自行建立或取得的應用程式部署至供應商提供的平台。供應商管理底層基礎設施及平台元件；使用者管理部署的應用程式及部分託管環境設定。

## 3. IaaS（Infrastructure as a Service，基礎設施即服務）
供應商提供處理能力、儲存、網路等基礎資源。使用者可部署作業系統及應用程式，並管理作業系統、儲存及部署的應用程式；底層實體基礎設施仍由供應商管理。

## 4. 管理範圍比較

| 項目 | SaaS | PaaS | IaaS |
|---|---|---|---|
| 使用應用程式 | 使用供應商應用程式 | 部署自行建立／取得的應用程式 | 部署自行選擇的軟體 |
| 管理應用程式 | 通常有限 | 使用者管理 | 使用者管理 |
| 管理作業系統 | 供應商 | 供應商 | 使用者 |
| 管理底層實體資源 | 供應商 | 供應商 | 供應商 |

## 5. 服務評估

來源依據：[CC-006](../sources/CC-006_NIST_SP_500-322.md)，第 3～6 節。
NIST SP 500-322 提醒，產品名稱帶有「aaS」不代表它必然符合 NIST 的雲端服務定義。評估時應先檢查五項基本特徵，再判斷其服務模式，而不是只看供應商的行銷名稱。文件提供 Cloud Service Worksheet、Cloud Service Model Worksheet 及 Cloud Deployment Model Worksheet，協助使用者分析服務能力。

## 6. 安全責任與服務模式

來源依據：[CC-007](../sources/CC-007_Google_Shared_Responsibility.md)。
Google Cloud 的安全文件以其產品為例說明：
- IaaS：客戶承擔較多安全責任，Google Cloud 著重底層基礎設施及實體安全。
- PaaS：責任由雙方分擔；客戶仍須管理資料安全、用戶端保護及部分應用層控制。
- SaaS：供應商承擔大部分安全責任，但客戶仍須管理存取控制及其存放資料。
實際責任仍依各項服務及設定而異，不能將此表視為所有供應商的通用責任矩陣。（CC-007）

## 來源
- CC-001：NIST SP 800-145
- CC-003：NIST SP 500-292
- CC-004：NIST SP 800-146
- CC-006：NIST SP 500-322
- CC-007：Google Cloud Shared Responsibilities and Shared Fate
