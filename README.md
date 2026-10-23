# 玉珊二十歲生日闖關

網站：https://yushan1023.vercel.app

改了 `main` 分支、推上 GitHub 之後，Vercel 會自動重新部署，一兩分鐘後網站就更新。

## 檔案

- `index.html`：整個網站（文字、畫圖、遊戲都在這一個檔案裡）
- `photos/`：照片（`photos/mem/` 是第五關翻牌用的 8 張）
- `jfzj.mp3`：背景音樂《幾分之幾》
- `guitar.mp3`：第四關的吉他錄音
- `favicon.png`、`apple-touch-icon.png`：網站小圖示

## 常改的地方（都在 index.html，用搜尋找）

| 想改什麼 | 搜尋這個 |
|---|---|
| 最後的信 | `const LETTER=[`（一行一段） |
| 電話裡的話 | `const PHONE_LINES=` |
| 拆包裹後的紙條 | `<div class="note">` |
| 每關開頭角色說的話 | `const HOSTS=[`，每個角色的 `say:[...]` |
| 照片和照片下面的字 | `const PHOTOS=[` |
| 翻牌的照片說明 | `const N=8,MC=[` |

換照片：把新照片放進 `photos/`，用同一個檔名覆蓋就好（建議先縮到 640px 以內，存成 .webp 或 .jpg）。

## 改完自己先看

在這個資料夾開終端機，輸入 `npx serve .`，用瀏覽器打開它給的網址。
不要直接雙擊 index.html，那樣音樂和照片可能讀不到。
