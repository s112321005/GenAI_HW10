# AGENTS.md — 旅遊計畫與景點知識庫 (Travel Planner Wiki)

本文件定義 AI Agent 在維護與累積本「旅遊計畫知識庫」時應遵守的架構、規範與自動化工作流。本專案採 Karpathy LLM Wiki 模式：AI 負責讀取原始資料、擷取知識、建立交叉連結與維護 HTML 網頁；使用者負責提供來源、引導探索與發問。

---

## 1. 專案架構 (Architecture)

本專案分為三層架構：

1. **Raw Sources (原始來源層)**：存放未經修改的原始旅遊資料（如部落格文章、貼文剪藏、景點介紹文字、訂單明細）。存放於 `raw/inbox/`。**AI 不得修改此目錄內的檔案。**
2. **The Wiki (知識整理層)**：由 AI 完全維護與產出的 Markdown 知識檔案庫（位於 `wiki/`）。包含景點頁面 (spots)、美食頁面 (food)、交通住宿 (transport)、行程規劃 (itineraries)。頁面之間需透過 Markdown 連結 (`[[頁面名稱]]` 或 `[頁面](路徑)`) 建立關聯。
3. **The Schema (規則設定層)**：即本文件 `AGENTS.md`，定義 AI Agent 的運作守則與檔案命名標準。

---

## 2. 專案目錄結構

```text
travel-planner-wiki/
│
├── AGENTS.md               # 本規則文件
├── index.html              # 展示用網站首頁（AI 自動維護與更新）
├── index.md                # 知識庫總索引 (Content Catalog)
├── log.md                  # 知識庫異動日誌 (Chronological Log)
│
├── raw/
│   └── inbox/              # 暫存未整理的旅遊文章、複製貼上內容
│
├── wiki/
│   ├── spots/              # 景點知識頁面 (Markdown)
│   ├── food/               # 美食與咖啡廳頁面 (Markdown)
│   ├── transport/          # 交通與住宿指南 (Markdown)
│   └── itineraries/        # 每日行程規劃 (Markdown)
│
└── pages/                  # AI 自動生成的單頁 HTML 展示網頁