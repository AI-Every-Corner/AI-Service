# AI Service 模組

## 專案概述
此模組負責與 **OpenAI API** 進行交互，實現文章回應的生成以及情感分析。該模組接收來自後端的請求，通過API調用生成多個AI回應，並將結果返回後端。

## 技術棧
- **Spring Boot**: 用於構建輕量的API服務。
- **OpenAI API**: 使用OpenAI提供的API進行自然語言處理。
- **RestTemplate/HttpClient**: 用於發送HTTP請求與OpenAI API交互。

## 主要功能
- **AI回應生成**：根據用戶發表的文章內容生成多個不同語氣的AI回應。
- **情感分析**：分析用戶文章的情感狀態，並根據結果生成適合的回應。

## API路由
- **POST /generate-response**: 傳入文章文本，生成多個AI回應。
- **POST /analyze-sentiment**: 傳入文章文本，返回情感分析結果。

## 文件結構
- `/src/main/java/com/yourproject/ai`: 包含Spring Boot應用的主要代碼。
  - `/controller`: 定義API控制器，處理來自前端或其他後端服務的請求。
  - `/service`: 與OpenAI API進行交互，處理回應生成和情感分析邏輯。
  - `/model`: 定義數據模型，用於表示API請求與回應數據。
  - `/config`: 配置OpenAI API金鑰等相關信息。

## 未來展望
優化AI回應生成邏輯：根據不同場景生成更加智能的回應，提升用戶體驗。
引入更多AI服務：擴展服務，支持更多基於AI的互動模式和場景。
