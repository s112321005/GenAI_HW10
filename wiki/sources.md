# 來源登錄與證據狀態

## 本次處理的五篇附件 Wiki 條目

下列條目來自使用者提供的 `travel-planner-wiki.zip`。它們是本次 ingest 的五筆資料單位，但附件沒有附上其宣稱的原始來源。此處登錄的是「資料來自哪個檔案」，不是對條目內每項事實的獨立驗證。

| Source ID | 附件中的知識頁 | 狀態 | 使用方式 |
|---|---|---|---|
| SRC-WIKI-01 | `wiki/food/fukudaya.md`（原 ID：SRC-20261116-01） | 附件內既有整理；原始來源缺失 | 只作為 Wiki 例子；營業時間、價格與交通細節不當成已核實事實 |
| SRC-WIKI-02 | `wiki/food/rice-curry-manten.md`（原 ID：SRC-20261116-02） | 附件內既有整理；原始來源缺失 | 用來說明料理類型與地區檢索，不引用即時價格 |
| SRC-WIKI-03 | `wiki/food/kanda-matsuya.md`（原 ID：SRC-20261116-03） | 附件內既有整理；原始來源缺失 | 用來說明傳統蕎麥麵條目的整理方式，不將營業資訊視為最新 |
| SRC-WIKI-04 | `wiki/food/tsukishima-monja-moheji.md`（原 ID：SRC-20261116-04） | 附件內既有整理；原始來源缺失 | 餐廳資訊僅為附件內容；文字燒的一般料理概念另以 SRC-EXT-01 核對 |
| SRC-WIKI-05 | `wiki/food/isehiro-yakitori.md`（原 ID：SRC-20261116-05） | 附件內既有整理；原始來源缺失 | 用來示範燒鳥條目與查詢，不引用即時菜單、價格或營業資訊 |

## 外部概念核對來源

- **SRC-EXT-01 — SAVOR JAPAN, “All About the Tokyo Specialty Food, Monjayaki”**。文章描述文字燒的基本材料、以鐵板烹調與小鏟食用方式，並比較文字燒和大阪燒。此來源只支援一般料理概念，不證明附件中的「もへじ」分店、菜單、價格或營業狀態。網址：https://savorjapan.com/contents/discover-oishii-japan/all-about-the-tokyo-specialty-food-monjayaki 。文章更新日為 2024-03-29；查閱日為 2026-11-23。

## 使用規則

1. 每個可作為教學事實的主張，必須能連回 Wiki 頁或外部來源。
2. 「附件原文有寫」不等於「現況已核實」。營業時間、價格、地址、付款方式與預約政策要標記為易變資訊。
3. 若要實際出發，應查詢店家官方頁面或近期可靠資料；本次成果不提供即時營業確認。
4. 新 ingest 項目應保留原始內容於 `raw/inbox/`，賦予唯一來源 ID，並記錄擷取日期及 URL／檔名後才進入 Wiki 整理。
