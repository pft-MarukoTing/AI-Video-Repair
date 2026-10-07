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
| Step 1 Upload your footage | `assets/page/step/step01.png` | Step01.png（10/6 重新做的版本，300×300，直接使用；Step02、Step03 於 13:28 又更新過） | 正式圖 |
| Step 2 Auto-suggested settings | `step02.png` | Step02.png（10/6 重新做的版本，300×300，直接使用；Step02、Step03 於 13:28 又更新過） | 正式圖 |
| Step 3 Fine-tune, then repair | `step03.png` | Step03.png（10/6 重新做的版本，300×300，直接使用；Step02、Step03 於 13:28 又更新過） | 正式圖 |
| Step 4 Compare, then save | `step04.png` | Step04.png（10/6 重新做的版本，300×300，直接使用；Step02、Step03 於 13:28 又更新過） | 正式圖 |
| Beyond Resolution 01 Video Denoise | `assets/page/video/video-denoise.mp4` | AME／Video Denoise_2.mp4（10/7 15:36 新版；ffmpeg crf 28 壓縮） | AE 成品 |
| Why Use 01 Restore Old Family Tapes | `assets/page/video/restore-old-family-tapes.mp4` | AME／Restore Old Family Tapes_2.mp4（10/7 15:36 新版；ffmpeg crf 28 壓縮） | AE 成品 |
| Beyond Resolution 02 Frame Interpolation | `assets/page/video/frame-interpolation.mp4` | AME／Frame Interpolation_3.mp4（10/7 15:36 新版；ffmpeg crf 28 壓縮） | AE 成品 |
| Beyond Resolution 03 AI Lighting | `assets/page/video/ai-lighting.mp4` | AME／AI Lighting_6.mp4（10/6 16:57 新版；ffmpeg crf 28 壓縮） | AE 成品 |
| Why Use 02 Concert | `assets/page/video/relive-every-concert.mp4` | AME／Relive Every Concert_4.mp4（10/7 15:36 新版；ffmpeg crf 28 壓縮） | AE 成品 |
| Intro 功能示範 Turn Old, Dark, Choppy Clips… | `assets/page/video/smooth-4k-quality-video.mp4` | AME／Smooth 4K-Quality Video_2.mp4（10/7 15:36 新版；ffmpeg crf 28 壓縮） | AE 成品 |
| Why Use 03 Live stream | `assets/page/img/live-stream.jpg` | AME／Live Stream.png（10/7 15:44，1200×848，子母畫面：小的 Before＋大的 After）；PNG 有透明角落，已壓平在白底存成 JPG（157KB） | **圖片**（依指示這一格不用影片） |
| Topbanner | `assets/page/video/top-banner.mp4` | AME／top-banner_2.mp4（10/6 11:59，2880×1254，10MB） | AE 成品；**沒有手機版素材**，手機/平板暫時裁左側（object-position 20%） |

全部區塊都已有素材。

## 壓縮紀錄

2026-10-06 16:17 由 Maruko 壓縮過所有圖片與影片（檔名、尺寸、編碼、時長都沒變，已逐一核對）：影片合計約 53MB → 12MB，圖片合計約 890KB → 143KB。PNG 透明背景保留。壓縮後影片與原檔畫面相似度 SSIM 約 0.97–0.98。
注意：影片的 moov 在檔案尾端（AME 輸出本來就是），瀏覽器會等整檔下載完才開始播放；之後若要改善可用 `ffmpeg -c copy -movflags +faststart` 無損重封裝。

## 前端互動範圍

- CTA 按鈕只做前端 hover 效果，未串接。
- FAQ 手風琴、漢堡選單、語言切換已做互動。

## Git / 上線狀態

**尚未 push 到 GitHub** — 頁面還在製作中，依指示先只留在本機。
