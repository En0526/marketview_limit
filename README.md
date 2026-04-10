# 市場監控 × 智能交易系統｜雲端即開即用版（`marketview_limit`）

## 立即使用（免下載）

**👉 點此開啟網站：** [https://trading-system-kkhs.onrender.com/](https://trading-system-kkhs.onrender.com/)

複製網址：`https://trading-system-kkhs.onrender.com/`  
（免安裝、免登入即可瀏覽示意功能；免費方案主機閒置後首次開啟可能需等待約數十秒喚醒。）

## 需要完整版功能？請下載本機專案

**👉 完整功能（與作者日常使用相同）：** [https://github.com/En0526/marketview_pro](https://github.com/En0526/marketview_pro)

請至該 repo clone 後依 README 在本機執行；雲端本倉庫僅為示意，報價／爬蟲等能力會明顯受限。

---

**開瀏覽器就能看盤、試用擇時與策略匹配**——不必先 clone、不必本機安裝，點連結就能體驗。

本倉庫為**為了上雲端（例如 Render）而維護的版本**：讓**沒有下載本專案程式碼的人**也能透過公開網址使用網站。

與本機完整版相比，**功能會在很大程度受限**，主要原因是**資料爬取／外部 API 請求**在雲端環境容易受到**服務商網路、頻率、出口 IP、防火牆與第三方來源限制**影響，行為與穩定性無法與本機開發環境完全一致。

若你需要與作者日常使用的**完整功能**，請直接開啟並 clone 本機完整版：**[https://github.com/En0526/marketview_pro](https://github.com/En0526/marketview_pro)**（點連結即可進入 repo，再依該專案 README 在本機部署執行）。

---

一個智能交易系統，具備擇時功能和策略自動匹配能力。

> **[網站使用指南（客戶必看）](網站使用指南.md)** — 線上示意版：[https://trading-system-kkhs.onrender.com/](https://trading-system-kkhs.onrender.com/)；完整版程式庫（可點）：[https://github.com/En0526/marketview_pro](https://github.com/En0526/marketview_pro)；洽詢見指南內說明

## 功能特色

- **市場監控**：即時顯示美股、台股及主要國際市場盤勢
- **擇時功能**：智能判斷最佳交易時機
- **策略匹配**：自動選擇最適合當前市場環境的交易策略
- **Web 介面**：一目了然的市場數據展示

## 專案結構

```
trading_system/
├── app.py                 # Flask 主應用
├── config.py             # 配置文件
├── market_data/          # 市場數據模組
│   ├── __init__.py
│   ├── data_fetcher.py   # 數據獲取
│   └── market_analyzer.py # 市場分析
├── timing/               # 擇時模組
│   ├── __init__.py
│   └── timing_selector.py
├── strategy/             # 策略模組
│   ├── __init__.py
│   └── strategy_matcher.py
├── templates/            # HTML 模板
│   └── index.html
├── static/               # 靜態資源
│   ├── css/
│   └── js/
└── requirements.txt      # 依賴套件
```

## 安裝與使用

### 1. 安裝依賴

```bash
pip install -r requirements.txt
```

### 2. 運行應用

```bash
python app.py
```

### 3. 訪問網站

打開瀏覽器訪問: http://localhost:5000

## 快速開始

### 1. 安裝依賴套件

```bash
pip install -r requirements.txt
```

### 2. 啟動應用程式

```bash
python app.py
```

### 3. 訪問網站

打開瀏覽器訪問: `http://localhost:5000`

## 詳細說明

請參考 [`使用說明.md`](使用說明.md) 了解每個 Python 檔案的詳細功能和使用方法。

## 開發計劃

- [x] 基礎環境設置
- [x] 市場數據獲取
- [x] Web 介面
- [x] 擇時功能實現
- [x] 策略匹配算法
- [ ] 回測系統
- [ ] 風險管理模組
- [ ] 更多技術指標
- [ ] 歷史數據分析

## 技術棧

- **後端**: Python, Flask
- **數據**: yfinance, pandas
- **前端**: HTML, CSS, JavaScript
- **圖表**: Chart.js

## License

MIT

