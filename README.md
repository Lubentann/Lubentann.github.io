# Lubentann.github.io

個人作品集首頁，網址：**https://lubentann.github.io/**

因為 repo 命名為 `<帳號>.github.io`，GitHub Pages 會直接掛在根網址，
不會多一層路徑 —— 這就是履歷上要放的連結。

## 架構

首頁只負責「介紹 + 導流」。每個作品維持自己的 repo 與 demo 頁，
新增作品時只要在首頁加一張卡片，不必動到既有專案。

```
Lubentann.github.io          ← 這個 repo（作品集首頁）
└─ 小逃 Trip  → 連到 Lubentann/trip-planner-pwa
```

## 新增一件作品

1. 截圖放進 `assets/`（建議 16:10，例如 960×600）
2. 打開 `index.html`，複製整段 `<article class="card">`，改標題／說明／標籤／連結
3. 沒有截圖時，刪掉該卡片裡的 `<img class="shot">` 那一行即可
4. 部署：

```bash
git add -A && git commit -m "新增作品：XXX" && git push
```

推上去約 30–60 秒後生效。

## 設計備註

- 單一 HTML 檔，無框架、無建置流程
- 自動支援深色／淺色模式（跟隨系統）
- 手機版面已處理（600px 以下按鈕改為滿寬）
- 配色與「小逃 Trip」同一個暖色系但更中性，之後加入其他品牌的作品才不會打架
