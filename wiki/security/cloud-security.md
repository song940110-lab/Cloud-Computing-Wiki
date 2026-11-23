# 雲端資料與安全（Cloud Data and Security）

## 1. 安全是跨層面議題

來源依據：[CC-003](../sources/CC-003_NIST_SP_500-292.md)，安全與隱私相關章節。
NIST SP 500-292 指出，安全是橫跨參考架構各層的議題，從實體安全到應用程式安全皆須考量。雲端安全不只是供應商的責任，也涉及雲端消費者及其他參與角色。

文件列出的安全需求包括：
- 身分驗證（Authentication）
- 授權（Authorization）
- 可用性（Availability）
- 機密性（Confidentiality）
- 身分管理（Identity Management）
- 完整性（Integrity）
- 稽核與安全監控
- 事件應變及安全政策管理

## 2. NIST SP 800-146 提醒的風險

來源依據：[CC-004](../sources/CC-004_NIST_SP_800-146.md)，第 8、9 節。
NIST SP 800-146 討論雲端系統在效能、可靠性、經濟、法規遵循及資訊安全方面的問題，包括：
- 網路依賴、延遲及供應商服務中斷。
- 資料可攜性、互通性及災難復原。
- 資料所在地、司法管轄及合規要求。
- 非預期資料揭露、隱私、多租戶隔離。
- 瀏覽器安全、硬體信任及金鑰管理。
- 虛擬機器蔓延、VM 隔離及資料清除。

## 3. Google Cloud 的 Shared Responsibility

來源依據：[CC-007](../sources/CC-007_Google_Shared_Responsibility.md)。
Google Cloud 說明，客戶需了解自身的法規義務、組織安全標準及風險管理計畫，並設定保護資料與工作負載所需的安全控制。

以 Google Cloud 的服務分類為例：
- **IaaS**：客戶承擔較多安全責任；供應商主要負責底層基礎設施與實體安全。
- **PaaS**：供應商負責較多控制；應用層控制及 IAM 可能由雙方共同負責，客戶仍負責資料安全與用戶端保護。
- **SaaS**：供應商承擔大部分安全責任；客戶仍負責存取控制及其選擇儲存的資料。
- **FaaS／Serverless**：Google 文件指出其責任分配與 SaaS 有相似之處，實際仍需看服務。

Google 亦指出，供應商始終負責底層網路與基礎設施，客戶始終負責自己的存取政策及資料。

## 4. Shared Fate
Shared Fate 是 Google Cloud 在 shared responsibility 之外提出的合作安全概念。Google 描述其做法包括提供可信任的雲端平台、最佳實務指引、安全基礎設施程式碼，以及整合式安全解決方案，並與客戶更密切合作。

**注意：** Shared Fate 是 Google Cloud 的供應商觀點，不應當成所有雲端平台通用的正式標準。

## 5. 資料與治理
使用雲端服務前，應確認：
- 哪些安全控制由客戶負責。
- 哪些控制由服務本身提供。
- 哪些預設控制可以繼承或作為稽核證據。
- 資料所在地及適用法規。
- 資料備份、移轉及離開供應商時的可攜性。
- 服務合約及 SLA 中的雙方責任。

## 來源
- CC-003：NIST SP 500-292，第 3.4、3.5 節
- CC-004：NIST SP 800-146，第 8、9 節
- CC-007：Google Cloud Shared Responsibilities and Shared Fate
