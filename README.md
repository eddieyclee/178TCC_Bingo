# 178 TCC Bingo

多人即時賓果遊戲，支援手機掃 QR Code 加入。

## 部署到 GitHub Pages（步驟）

### 1. 建立 GitHub Repository
1. 登入 [github.com](https://github.com)
2. 右上角「+」→「New repository」
3. Repository name 填：`178-tcc-bingo`（或任意名稱）
4. 選「Public」
5. 點「Create repository」

### 2. 上傳檔案
1. 在剛建立的 repo 頁面，點「uploading an existing file」
2. 將以下 4 個檔案全部拖入：
   - `index.html`
   - `host.html`
   - `player.html`
   - `README.md`
3. 點「Commit changes」

### 3. 開啟 GitHub Pages
1. 進入 repo → 上方「Settings」
2. 左側選「Pages」
3. Source 選「Deploy from a branch」
4. Branch 選「main」，資料夾選「/ (root)」
5. 點「Save」

稍等 1-2 分鐘後，網址會是：
```
https://你的帳號.github.io/178-tcc-bingo/
```

### 4. 設定 Firebase（只需一次）
1. 前往 [console.firebase.google.com](https://console.firebase.google.com)
2. 建立新專案（免費）
3. 左側「Realtime Database」→「建立資料庫」→「測試模式」
4. 複製 Database URL（格式：`https://xxx-default-rtdb.firebaseio.com`）
5. 開啟主持人頁面，貼上 URL 即可

## 遊戲說明
- **主持人**：開啟 `host.html`，選格數和號碼範圍，建立房間後分享 QR Code
- **玩家**：掃 QR Code，填寫賓果卡數字，等待主持人叫號
- 叫號後號碼自動標記，完成連線顯示 BINGO 🎉

## 檔案說明
| 檔案 | 說明 |
|------|------|
| `index.html` | 首頁，選擇主持人或玩家 |
| `host.html` | 主持人頁面（電腦用） |
| `player.html` | 玩家頁面（手機用） |
