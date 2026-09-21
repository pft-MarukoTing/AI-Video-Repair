# 交付說明 — AI Video Repair Prototype v1

日期：2026-09-21
基底：沿用 AI Auto Video Cut / AI Character Motion Swap 頁面的設計系統（tokens、Header/Footer、按鈕、FAQ 手風琴、Zig-zag 區塊樣式、Steps 區塊 grid layout）
內容來源：`https://yce-stage.perfectcorp.com/product-preview?cmsId=455&pageKey=ai-video-repair`（正式站文案，逐字擷取）

## 這次涵蓋範圍

整頁：Header → Topbanner → How It Works（單一功能介紹：Enhance）→ Repair Your Video in 4 Steps → Every Fix, Automated（Zig-zag圖文交錯 ×3：Denoise／Frame Interpolation／AI Lighting）→ FAQ（8則手風琴）→ Footer。

## ⚠️ 缺少的素材（目前全部用虛線佔位框代替）

這次沒有拿到 AI Video Repair 的實際影片/圖片，Topbanner、功能示範影片、Step 1–4 縮圖、Zig-zag 三組示範素材全部是 `media-placeholder` 佔位框。素材到位後告訴我對應檔名/位置，我再替換。

## 跟 AI Auto Video Cut 頁面的結構差異

- **Steps 這次是 4 步（不是 5 步）**：`.steps` 改成 `grid-template-columns:repeat(4,1fr)`，桌機一列四欄置中，沿用同一套 grid 機制（AI Auto Video Cut 是 `repeat(5,1fr)`）。
- 其餘結構（Intro 單一功能重點、Zig-zag 三組、FAQ 8則、Steps/Zig-zag 標題下的副標）完全比照 AI Auto Video Cut 頁面的做法。

## 本次依循的規則來源

沿用 AI Auto Video Cut／Motion Swap 頁面的設計 tokens／按鈕/FAQ/Zig-zag/Steps 規則，這次沒有拿到 Figma 設計稿，版面配置依「正式站文案結構」推導，不是照專屬設計稿還原。如果之後有這頁的 Figma 稿，麻煩提供再依實際稿調整。

## 前端互動範圍

- CTA 按鈕只做前端 hover 效果，未串接下一步功能。
- FAQ 手風琴、漢堡選單、語言切換按鈕已做前端展開/收合互動。

## 檔案結構

```
index.html
style.css
script.js
assets/YCO/icons/   （沿用 workspace 既有固定素材）
assets/YCO/logos/   （沿用 workspace 既有固定素材）
```

## Git / 上線狀態

**尚未 push 到 GitHub** — 頁面還在製作中，依指示先只留在本機，之後確認 OK 再建 repo push。
