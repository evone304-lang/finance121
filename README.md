# 🎯 目標理財規劃器

以 PV(現值)、FV(未來值)、PMT(每期投入)為核心的目標導向理財試算網站。
純靜態單頁,無需建置,資料只存在使用者自己的瀏覽器。

## 資料夾結構(index.html 在最外層)
```
finance-planner/
├── index.html
├── _headers
├── README.md
├── LICENSE
└── .gitignore
```

## 部署到 Cloudflare Pages

### 方式 A:直接拖曳(最快)
1. Cloudflare Dashboard → Workers & Pages → Create → Pages → Upload assets
2. 輸入專案名稱,把整個資料夾(或 zip)拖進去,按 Deploy。

### 方式 B:GitHub 自動部署
1. 把此資料夾內容推到 GitHub 儲存庫(index.html 要在儲存庫最外層)。
2. Cloudflare → Workers & Pages → Create → Pages → Connect to Git,選該儲存庫。
3. Framework preset: None;Build command: 留空;Build output directory: 留空(或填 `/`)。
4. Save and Deploy。之後每次 push 都會自動更新。

## 免責聲明
本工具僅供試算與教育用途,不構成投資建議。報酬率為假設值,實際結果可能不同。
