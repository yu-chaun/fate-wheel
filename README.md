# 命運轉盤・糾結終結者

選擇困難時用的轉盤小網站：內建多個主題，也能自訂選項，按下「開轉」就隨機決定結果。純前端、單一 HTML 檔。

## 使用說明
1. 點快速主題（今天吃什麼、誰請客…）或自己在文字框輸入選項，一行一個。
2. 按「開轉！」，等轉盤停下，箭頭指到的就是結果。
3. 右下角會記錄每次結果。
4. 勾選「抽中後從轉盤移除」可以排出不重複的順序。

## 專案結構
```
fate-wheel/
├── public/index.html   # 整個網站
├── wrangler.jsonc      # Cloudflare 部署設定（指向 public）
├── README.md
└── .gitignore
```

## 部署到 Cloudflare
Workers & Pages → Create → Connect to Git → 選此倉庫。Build command 留空，Deploy command 用預設的 `npx wrangler deploy`。
部署後到專案的 Domains 分頁啟用 workers.dev 網址。
