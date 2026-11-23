# 雲端部署模式（Cloud Deployment Models）

NIST SP 800-145 定義四種部署模式。NIST SP 500-292 進一步以參考架構說明不同部署方式及其資源控制範圍。

## 1. 私有雲（Private Cloud）

來源依據：[CC-001](../sources/CC-001_NIST_SP_800-145.md)；架構補充：[CC-003](../sources/CC-003_NIST_SP_500-292.md)。（Private Cloud）
雲端基礎設施專供單一組織使用。可由該組織、第三方或兩者共同管理，也可設置於組織內部或委外託管。

## 2. 社群雲（Community Cloud）
雲端基礎設施專供具有共同關注事項的特定組織群體使用，例如共同任務、安全需求、政策或法規遵循要求。

## 3. 公有雲（Public Cloud）
雲端基礎設施開放一般大眾使用，由提供雲端服務的組織擁有、管理及營運。

## 4. 混合雲（Hybrid Cloud）
由兩種或以上不同的雲端基礎設施組成，這些基礎設施仍各自獨立，但透過技術連結，使資料及應用程式具有可攜性。

## 5. 比較

| 模式 | 使用對象 | 主要判斷 |
|---|---|---|
| Private Cloud | 單一組織 | 基礎設施專供單一組織 |
| Community Cloud | 特定組織群體 | 成員具有共同關注事項 |
| Public Cloud | 一般大眾 | 對大眾提供服務 |
| Hybrid Cloud | 依組合而定 | 至少兩種不同雲端基礎設施連結 |

## 6. 分類注意
Google Cloud 的入門文章以 Public、Private、Hybrid 三種方式介紹部署模式；這是該文章採用的簡化介紹。Wiki 的正式分類仍以 NIST SP 800-145 的四種模式為準，保留 Community Cloud。NIST SP 500-322 亦分別提供四種部署模式的評估工作表。

## 來源
- CC-001：NIST SP 800-145
- CC-002：Google Cloud What is Cloud Computing?
- CC-003：NIST SP 500-292
- CC-004：NIST SP 800-146
- CC-006：NIST SP 500-322
