# promise82114.github.io
Official website of OuoukoDayo — a collection of personal projects, game tools, and experiments.

## 網站與部署

純靜態 HTML / CSS，無需安裝套件或編譯。GitHub Pages 使用 `main` 分支的根目錄（Deploy from a branch）；推送到 `main` 後自動發布。`.nojekyll` 停用 Jekyll 處理。

- 首頁：https://promise82114.github.io/
- EDF WB2 收集手帳：https://promise82114.github.io/edfwb2-checklist/
- 隱私權政策：https://promise82114.github.io/privacy.html
- 服務條款：https://promise82114.github.io/terms.html

本機預覽：`node server.mjs`，開啟 http://127.0.0.1:4176/ 。預覽伺服器僅提供網站公開檔案，不提供 Git 資料或維護脚本。

## Google Auth Platform

在 Google Auth Platform → Branding 填入：

- App name：`OuoukoDayo`
- User support email：`promise82114@gmail.com`
- Application home page：`https://promise82114.github.io/`
- Privacy policy：`https://promise82114.github.io/privacy.html`
- Terms of service：`https://promise82114.github.io/terms.html`

網站頁面不會自動修改 Google Cloud 設定，也不代表已通過 Google OAuth 審查。Authorized domains 依 Google Console 要求設定與驗證；Web OAuth client 的 Authorized JavaScript origins 使用 `https://promise82114.github.io`，不含次專案路徑。Drive API 與 `drive.appdata` 範圍的設定見次專案的 `docs/google-drive-sync.md`。

政策依目前次專案的實作撰寫：Token 僅存在記憶體，進度在瀏覽器與 Drive `appDataFolder` 間直接傳輸。未來若新增分析工具、伺服器或不同權限範圍，需同步更新政策內容。
