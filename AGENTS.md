# 專案工作流程規範 (Project Workflow Guidelines)

本文件定義每個專案在 **初始化 (Init)**、**開工 (Start of Work)** 及 **收工 (End of Work)** 時的標準作業程序 (SOP)。

---

## 1. 專案初始化流程 (Project Initialization)

當開啟或建立一個全新專案時，執行以下程序：

1. **環境檢查與初始化 (Environment Setup)**
   - 檢查專案目錄結構與必要設定檔（如 `.gitignore`, `package.json`, `requirements.txt` 等）。
   - 若為 Git 專案且未初始化，執行 `git init` 並設定遠端倉庫（Remote Repository）。

2. **建立專案說明檔 (Documentation)**
   - 在專案根目錄建立 `README.md`，說明專案目標、技術棧與使用說明。
   - 在專案根目錄建立 `AGENTS.md`，記錄專案專屬規範或指示。

3. **確定依賴與規範 (Dependencies & Standards)**
   - 確認使用的編程語言與套件管理工具（如 `npm`, `pip`, `uv` 等），並建立虛擬環境或相依套件清單。

---

## 2. 每日/每次開工流程 (Start of Work Workflow)

開始進行具體任務或開發前，執行以下程序：

1. **確認儲存庫狀態 (Check Status & Pull Updates)**
   - 執行 `git status` 檢查當前工作區是否乾淨。
   - 若有遠端分支，執行 `git pull origin <branch>` 確保本地程式碼為最新版本。

2. **審視任務目標 (Review Goal & Plan)**
   - 確認本次要完成的具體需求或待辦事項（Todo / Issues）。
   - 對於複雜任務，進行研究並規劃步驟（必要時建立 Implementation Plan）。

3. **環境與服務確認 (Check Environment)**
   - 確認開發環境與需要的服務/套件正常運作。

---

## 3. 每日/每次收工流程 (End of Work Workflow)

完成階段性開發或準備結束 turn / 離線時，執行以下程序：

1. **程式碼與成果驗證 (Verification)**
   - 執行建置、測試或驗證指令，確保新寫入的程式碼無語法錯誤或破壞性變更。

2. **清理臨時檔案 (Cleanup)**
   - 清理無用的測試腳本或臨時產出的快照檔。
   - 確保 `.gitignore` 已包含不需版控的暫存檔、金鑰與日誌。

3. **提交與推送 (Commit & Push)**
   - 執行 `git add .` 暫存變更。
   - 撰寫清晰符合規範的 Commit Message：`git commit -m "<清晰簡短的變更說明>"`。
   - 執行 `git push origin <branch>` 將最新進度推送至 GitHub / 遠端倉庫。

4. **更新文件與彙報 (Documentation & Summary)**
   - 更新 `README.md` 或相應變更記錄。
   - 向使用者簡要總結本次開工完成的項目與下一步計畫。
