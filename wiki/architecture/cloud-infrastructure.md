# 雲端基礎設施架構（Cloud Infrastructure）

## 1. NIST 參考架構的定位

來源依據：[CC-003](../sources/CC-003_NIST_SP_500-292.md)，第 2、3 節。
NIST SP 500-292 建立供討論、比較雲端服務使用的廠商中立高階參考架構。它描述角色、活動及功能，不是特定供應商的實際系統設計，也不是指定唯一實作方式。

## 2. 五種主要參與角色
1. **Cloud Consumer（雲端消費者）**：與雲端供應商建立業務關係並使用服務的個人或組織。
2. **Cloud Provider（雲端供應商）**：負責讓雲端服務可供使用的個人、組織或實體。
3. **Cloud Auditor（雲端稽核者）**：獨立評估雲端服務、系統運作、效能及安全的單位。
4. **Cloud Broker（雲端代理者）**：管理雲端服務使用、效能及交付，並協調供應商與消費者關係。NIST 描述服務中介、服務整合及服務套利等類型。
5. **Cloud Carrier（雲端承載者）**：提供供應商與消費者之間的連線及服務傳輸。

## 3. 雲端供應商的主要架構元件
NIST SP 500-292 第 3.2 節以三層模型描述服務協調（Service Orchestration）：

### 3.1 Service Layer（服務層）
提供雲端消費者存取服務的介面，涵蓋 SaaS、PaaS、IaaS。不同服務模式可以彼此建立在上層或獨立提供。

### 3.2 Resource Abstraction and Control Layer（資源抽象與控制層）
透過軟體抽象方式管理實體運算資源。例子包括 Hypervisor、虛擬機器、虛擬資料儲存及其他資源抽象元件。控制元件負責資源配置、存取控制及使用量監控，支援資源池化、動態分配及可衡量服務。

### 3.3 Physical Resource Layer（實體資源層）
包含 CPU、記憶體、網路設備、儲存設備，以及電力、冷卻、通訊等設施資源。

## 4. 雲端服務管理
NIST 將雲端服務管理分成三個面向：
- **Business Support**：客戶管理、合約、會計及定價等業務支援。
- **Provisioning and Configuration**：服務供應、配置及服務等級管理。
- **Portability and Interoperability**：資料、系統及服務在不同雲端環境間的可攜性與互通性。

## 5. Google Cloud 對雲端架構的教學整理

來源依據：[CC-005](../sources/CC-005_Google_Cloud_Architecture.md)。
Google Cloud 將雲端架構描述為整合硬體、虛擬資源、軟體能力及虛擬網路系統的藍圖。文章列出前端平台、後端平台、雲端交付模式及網路等組成。
- 前端：使用者介面、用戶端應用程式及裝置。
- 後端：應用程式、服務、執行環境、儲存、基礎設施、管理及安全。
- 架構層次：硬體、虛擬化、應用程式與服務。

## 6. 架構概念示意

```text
使用者／用戶端（Frontend）
          |
        網路
          |
雲端服務介面（Service Layer）
          |
資源抽象與控制層
(Hypervisor、VM、虛擬儲存、資源配置)
          |
實體資源層
(CPU、記憶體、網路、儲存、機房設施)
```

此圖為依 NIST 及 Google Cloud 文字內容整理的教學示意，非原始文件圖表。

## 來源
- CC-001：NIST SP 800-145
- CC-003：NIST SP 500-292，第 2、3 節
- CC-005：Google Cloud What is Cloud Architecture?
