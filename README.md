# 復盤統整工具 - Vercel 部署說明

## 資料夾內容
- index.html　　← 主要網頁
- api/chat.js　 ← 後端中繼（保護你的 API Key）
- vercel.json　 ← Vercel 設定

## 部署步驟

### 第一步：上傳到 Vercel
1. 前往 https://vercel.com 登入
2. 點「Add New Project」→「Upload」
3. 把這整個資料夾（review-tool）壓縮成 zip 上傳
   或是把三個檔案直接拖曳上去

### 第二步：設定 API Key（重要！）
部署完成後：
1. 進入你的專案設定（Settings）
2. 點左側「Environment Variables」
3. 新增一個變數：
   - Name：ANTHROPIC_API_KEY
   - Value：你的 API Key（sk-ant-api03-...）
4. 點 Save

### 第三步：重新部署
設定完 Key 之後，點「Redeploy」讓設定生效。

### 第四步：完成！
Vercel 會給你一個網址，直接發給學員使用。

## 注意事項
- API Key 存在 Vercel 的環境變數裡，學員完全看不到
- 費用由你的 Anthropic 帳號承擔（每次約 $0.01 美金以內）
- 可以在 Vercel 設定自己的網域
