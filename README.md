# Gemini 英語口語助手

這是一個基於 Google Gemini AI 的英語口語練習助手，它能實時識別你的英語發音，提供即時反饋和糾正建議。

Make by [Box](https://x.com/boxmrchen)

## 功能特點

- 🎤 實時語音識別
- 🤖 AI 驅動的發音評估
- 📝 語法糾正
- 🔄 情景對話練習
- 🎯 針對性發音指導
- 💡 智能場景切換

## 系統要求

- Python 3.11+ (必須)
- 麥克風設備
- 網絡連接

## 前置需求

需要一個 Gemini 的 API Key，這個 API Key 每天免費四百萬次，足夠使用了。

到這個頁面 [https://aistudio.google.com/app/apikey](https://aistudio.google.com/app/apikey) 生成即可。

## 安裝

1. 複製倉庫：
```bash
git clone https://github.com/nishuzumi/gemini-teacher.git
cd gemini-teacher
```

2. 創建並啟用虛擬環境（推薦）：
```bash
python -m venv .venv
source .venv/bin/activate  # Unix/macOS
# 或
.venv\Scripts\activate  # Windows
```

3. 安裝依賴：

在安裝 Python 依賴前，請先安裝以下系統依賴：

- Windows: 無需額外安裝
- macOS: `brew install portaudio`
- Ubuntu/Debian: `sudo apt-get install portaudio19-dev python3-pyaudio`

```bash
pip install -r requirements.txt
```

## 使用方法

1. 設定環境
新建一份 `.env` 文件，將 `.env.example` 內容複製過去，然後修改。

`GOOGLE_API_KEY` 填寫谷歌 Gemini 的 API Key

### 開啟語音功能
這個功能按需開啟，`ELEVENLABS_API_KEY` 是語音功能的 API KEY。

獲取方式：
- 打開網站 [https://elevenlabs.io/](https://try.elevenlabs.io/2oulemau2lxk)
- 點擊右上角的 Try for free，進行註冊，有免費的 1000 個額度
- 到個人設置中，生成 API Key 填入即可

```bash
python starter.py
```

2. 按照提示說出英語句子
3. 等待 AI 助手的反饋
4. 根據反饋改進發音

## 交互說明

- 🎤 : 正在錄音
- ♻️ : 正在處理
- 🤖 : AI 反饋

## 許可證

MIT

## 貢獻

歡迎提交 Issue 和 Pull Request！
