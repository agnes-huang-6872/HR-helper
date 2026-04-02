<div align="center">
<img width="1200" height="475" alt="GHBanner" src="https://github.com/user-attachments/assets/0aa67016-6eaf-458a-adb2-6e31a0763ed6" />
</div>

# HR-helper

這是一個使用 React + Vite 構建的專案。包含 Vite 環境設定、一鍵部署 GitHub Pages 及完整的 `.gitignore` 規範。

## 🚀 快速開始 (Run Locally)

**環境要求：** Node.js >= 18

1. 安裝對應套件：
   ```bash
   npm install
   ```
2. 設定環境變數：
   請參考 `.env.example` 建立 `.env` 檔案，並設定你的 `GEMINI_API_KEY`。
3. 啟動本機伺服器：
   ```bash
   npm run dev
   ```

## 📦 部署 (GitHub Actions)

專案已內建 GitHub Action (`.github/workflows/deploy.yml`)，將會自動部署到 GitHub Pages。

**設定步驟：**
1. 推送程式碼到 `main` 分支。
2. 進入 GitHub Repository 的 **Settings** -> **Pages**。
3. 在 **Build and deployment** 區塊，將 **Source** 設定為 **GitHub Actions**。
4. 等待 Action 執行完畢，專案即會正式上線！

## 🛡️ 版本控制規範 (.gitignore)

已設定排除：
- 依賴套件與打包產物 (`node_modules/`, `dist/`, `build/`)
- IDE/編輯器設定暫存檔 (`.vscode/`, `.idea/`, `.DS_Store`)
- 環境變數與機密資訊 (`.env`, `.env.local`... 等，但保留 `.env.example` 供參考)
- 系統 Log 記錄檔
