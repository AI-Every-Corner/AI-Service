# AI Service 模組

## 專案概述
此模組負責與 **OpenAI API** 進行交互，實現文章回應的生成以及情感分析。該模組接收來自後端的請求，通過API調用生成多個AI回應，並將結果返回後端。

## 技術棧
- **Python/Flask**: 用於構建輕量的API服務。
- **OpenAI API**: 使用OpenAI提供的API進行自然語言處理。
- **Requests**: 用於進行HTTP請求。

## 主要功能
- **AI回應生成**：根據用戶發表的文章內容生成多個不同語氣的AI回應。
- **情感分析**：分析用戶文章的情感狀態，並根據結果生成適合的回應。

## API路由
POST /generate-response: 傳入文章文本，生成多個AI回應。
POST /analyze-sentiment: 傳入文章文本，返回情感分析結果。

## 文件結構
/app: 包含Flask應用的主要代碼。
/routes.py: 定義API路由。
/services.py: 處理與OpenAI API的交互。
/utils.py: 辅助工具和功能函數。

## 配置
OpenAI API Key：需要在環境變量中設定API金鑰。

## 未來展望
優化AI回應生成邏輯，根據不同場景生成更加智能的回應。
引入更多AI服務，擴展對用戶互動的支援。
