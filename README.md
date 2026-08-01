# General AI Agent Knowledge Base (KB_aiagent)

本專案用於收集、整理與管理 AI Agent 相關教學、程式碼與影音逐字稿資源，並自動同步至 GitHub `MazingerSam/general_aiagent`。

## 🎯 專案目標

1. 彙整 **YouTube Sensebar 頻道** 等優質 AI 相關教學影片逐字稿與對照索引（含 AI Agent, Codex, Claude AI, AntiGravity, OpenCode 等）。
2. 提供 AI Agent 的自動化工作流（SOP）、自動下載與字幕解析工具。
3. 建立完整的知識庫（Knowledge Base）方便檢索與持續擴充。

## 🛠️ 技術棧與工具

- **Language**: Python 3.12+
- **Version Control**: Git / GitHub (`origin/main`)
- **Key Libraries / CLI**:
  - `yt-dlp`: YouTube 影片資訊與字幕檔自動下載工具

## 📁 目錄與重點檔案說明

- `youtube_videos.md`：收錄的 AI 相關影片清單與 YouTube 原創連結總表。
- `[NN]_[影片名稱].md`：各影片解析並匯出的對應逐字稿 / 字幕 Markdown 檔案。
- `AGENTS.md`：AI Agent 專案工作流程規範（包含初始化、開工、收工 SOP）。
- `.gitignore`：版本控制排除設定（暫存 JSON、下載字幕檔快取等）。

## 🚀 使用與執行說明

### 1. 環境準備與套件安裝
確保環境已安裝 Python 3 及 `yt-dlp`：
```bash
pip install -U yt-dlp
```

### 2. 開工與收工工作流 (SOP)
遵循 `AGENTS.md` 規範：
- **開工前**：執行 `git status` 與 `git pull origin main` 確保最新版。
- **收工後**：驗證產出檔無誤後，執行 `git add .`、`git commit` 與 `git push origin main`。
