# あいう日文入門

給初學者的日文學習網頁 App（繁體中文介面）。

- **五十音**：平假名、片假名（清音、濁音、拗音），點字發音，三種測驗
- **單字**：214 個入門單字、14 類（含日期、數量、錢、方位、生活常用），單字卡＋間隔複習
- **文法造句**：19 課基本句型，例句發音＋排積木造句
- **首頁**：連續學習天數、每日目標、建議下一步、錯題本

不需登入，進度存在使用者自己的瀏覽器。發音使用裝置內建的日語語音。

## 檔案

- `public/index.html`：整個 App（單一檔案，無需建置）
- `public/manifest.webmanifest`、`public/sw.js`、`public/icons/`：手機安裝（PWA）用的設定、離線快取和圖示
- `wrangler.jsonc`：Cloudflare Workers 靜態網站設定

## 部署

網址：https://japanese-learnning.hoya-chen.workers.dev

Cloudflare Workers（名稱 `japanese-learnning`）已連結這個 repo，每次推到 `main` 會自動部署。
手動部署：`npx wrangler deploy`
