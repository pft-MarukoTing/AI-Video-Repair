# 交付說明 — AI Video Repair Prototype v2

日期：2026-10-05（v1: 2026-09-21）
基底：沿用 AI Auto Video Cut / Motion Swap 頁面的設計系統
內容來源：`https://yce-stage.perfectcorp.com/product-preview?cmsId=468&pageKey=ai-video-repair`（正式站文案，逐字擷取；與 Figma `11120:27244` 同步）
素材來源：`~/Downloads/261020_Al Video Repair.aep_AME`（AE 輸出）＋ `~/Downloads` 底下陸續產出的圖

## 頁面結構（v2，對應 cmsId=468）

Header → Topbanner → Intro（單一功能：Turn Old, Dark, Choppy Clips…）→ 4 Steps → Beyond Resolution（Zig-zag ×3）→ Why Use YouCam AI Video Repair（Zig-zag ×3，新增）→ FAQ（10 則）→ Footer。
Zig-zag 每列有「Try It Now」＋「Download App」兩顆按鈕（跟 Figma／正式站一致）。

## 素材放置對照（我自己判斷放的，放錯請告訴我）

| 區塊 | 檔案 | 來源 | 狀態 |
| --- | --- | --- | --- |
| Step 1 Upload your footage | `assets/page/step/step01.png` | Soft cyan UI accent refresh-1.png（天藍色新版） | 正式圖 |
| Step 2 Auto-suggested settings | `step02.png` | Sky Blue Interface Recolor-3.png（1080p/30fps 那張；檔名編號 -3 但內容是 Step 2） | 正式圖 |
| Step 3 Fine-tune, then repair | `step03.png` | Sky blue UI accent recolor-2.png（Denoise/AI Lighting 那張；檔名編號 -2 但內容是 Step 3） | 正式圖 |
| Step 4 Compare, then save | `step04.png` | Sky Blue UI Accents-4.png | 正式圖 |
| Beyond Resolution 01 Video Denoise | `assets/page/video/video-denoise.mp4` | AME／Video Denoise.mp4（12:00 新版，5 秒） | AE 成品（6MB） |
| Why Use 01 Restore Old Family Tapes | `assets/page/video/restore-old-family-tapes.mp4` | AME／Restore Old Family Tapes_1.mp4（14:19 新版） | AE 成品（7MB） |
| Beyond Resolution 02 Frame Interpolation | `assets/page/video/frame-interpolation.mp4` | AME／Frame Interpolation_1.mp4（最新版；舊版 Frame Interpolation.mp4 圖示是 lighting/denoise，沒採用） | AE 成品（8MB） |
| Beyond Resolution 03 AI Lighting | `assets/page/img/ai-lighting.jpg` | Before AI_ Bright Sunset, Shadowed Faces.png | **暫放「Before」靜態圖**（等 before/after 成品） |
| Why Use 02 Concert | `assets/page/img/concert.jpg` | Indie Band Concert in Vivid Detail.png | **暫放靜態圖**（Downloads 另有 concert 原始影片，等 AE 成品） |
| Why Use 03 Live stream | `assets/page/img/livestream.jpg` | Clean gaming livestream moment.png | **暫放靜態圖**（備選：Restored cooking livestream in a bright kitchen.png） |

仍是佔位框：Topbanner、Intro 功能示範（`AI_Video_repair_1200x848.mp4` 原本在 Downloads，後來不見了，沒有採用）。

## 前端互動範圍

- CTA 按鈕只做前端 hover 效果，未串接。
- FAQ 手風琴、漢堡選單、語言切換已做互動。

## Git / 上線狀態

**尚未 push 到 GitHub** — 頁面還在製作中，依指示先只留在本機。
