# kaohsiung-travel（專案藍圖）

> 本檔為跨 Agent 通用的專案藍圖（AGENTS.md 開放標準）。任何 Agent 的每個 session 都應先讀本檔＋`handoff.md`。

## 專案簡介
<!-- 一段話：這個專案是什麼、目標是什麼 -->
高雄旅遊景點一頁式網站（單頁靜態網站），透過 GitHub Pages 自動部署，作為高雄旅遊景點展示與練習作品。

## 關鍵時程
<!-- 格式：- 事件名稱：日期（說明）；沒有就留白 -->

## 目標與路線圖
<!-- 用 checklist 追蹤，收工技能會更新這裡 -->
- [ ] 階段一：確認首版網站內容與呈現效果
- [ ] 階段二：擴充景點資料與版面設計

## 資料夾結構
<!-- 初始化時自動掃描生成，之後新增檔案要更新 -->
```
kaohsiung-travel/
├── index.html              # 高雄旅遊景點一頁式網站（唯一頁面）
└── .github/workflows/
    └── deploy.yml          # GitHub Actions：push 到 main 自動部署至 GitHub Pages
```

## 同步層級（本專案初始化至第 3 層級）

| 層級 | 平台 | 位置 | 讀取時機 |
|------|------|------|---------|
| L1 | 本地（雲端硬碟資料夾） | `AGENTS.md`＋`handoff.md` | 每個 session |
| L2 | GitHub | https://github.com/xa7515-crypto/kaohsiung-travel | 指定時 |
| L3 | Obsidian | kaohsiung-travel/專案工作流程.md | 有需要時 |

## 工作約定
- 任何 Agent、任何電腦：**開工先讀 `handoff.md`，收工必更新 `handoff.md`**
- 修改共用檔案前先讀最新內容，避免覆蓋其他 Agent 的變更
- 所有回應與文件使用繁體中文
- 修改前先確認計畫，優先保留原有資料結構

## 安全與隱私（不可違反）
- **不把 API key、密碼、憑證寫進 repo**，也不要貼進 `AGENTS.md`／`handoff.md`；一律放 `.env` 並列入 `.gitignore`
- **學生資料只用座號**，不出現姓名、學號、班級以外的個資、照片或聯絡方式
- 要公開分享前，先確認檔案裡沒有上述兩類內容