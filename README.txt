# 台股交叉策略每日推播（當沖用）

本專案會每日台灣時間晚上 6:00 自動分析台股「昨多、昨空」交叉策略，並將結果推送到你的 Telegram。

## 功能
- 使用 FinMind API 取得台股資料
- 全上市股票交叉條件篩選（紅K/黑K + 量 + 均線）
- 自動推播 Telegram
- GitHub Actions 每晚 18:00 定時執行

## 安裝與部署步驟

1. Fork 或建立新的 GitHub 專案
2. 上傳本專案三個檔案（main.py、README.txt、.github資料夾）
3. 到 GitHub 專案設定 Settings → Secrets → Actions 新增兩個 Secrets：
   - TELEGRAM_TOKEN：你的 Telegram Bot Token
   - TELEGRAM_CHAT_ID：你的 Telegram Chat ID
4. Commit 後，GitHub Actions 會每天晚上 6 點自動執行

---

有任何問題歡迎隨時詢問！
