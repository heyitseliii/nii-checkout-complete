# nii-checkout-complete

泥日教育 — 開課快手購課完成後的轉跳頁。

## 用途

同學在**開課快手**後台購買課程並完成結帳後，會被導向這個頁面，作為「報名完成」確認畫面。

## 🌐 網址（兩個版本）

| 版本 | 網址 | 部署來源 | 用途 |
|---|---|---|---|
| 🧪 **測試版** | <https://heyitseliii.github.io/nii-checkout-complete/> | GitHub Pages（`main` branch） | 給同事確認 |
| ✅ **正式版** | <https://thanks.nii.school/> | Cloudflare Pages（`production` branch） | 同學實際看到的頁面 |

## 🔄 改動 → 上線流程

```
改 index.html
  ↓
push 到 main branch
  ↓
🧪 測試版 1–3 分鐘後自動更新 → 分享給同事確認
  ↓
同事 Slack/Line 口頭 OK
  ↓
main merge 到 production branch
  ↓
✅ 正式版（thanks.nii.school）自動更新
```

**關鍵原則**：`main` 測試版隨時可改；`production` 正式版只在同事確認後才 merge。

## 📂 檔案結構

```
.
├── index.html   # 報名完成頁（單頁、內嵌樣式）
└── README.md
```

## 🧑‍💻 給同事的測試流程

1. 直接打開 **測試版網址**：<https://heyitseliii.github.io/nii-checkout-complete/>
2. 如要改文案或樣式，clone 這個 repo，在 `main` branch 改 `index.html`，commit & push

```bash
git clone https://github.com/heyitseliii/nii-checkout-complete.git
cd nii-checkout-complete
# 編輯 index.html
git add index.html
git commit -m "更新文案：xxxx"
git push origin main
```

3. 1–3 分鐘後看 **測試版** 確認改動
4. 跟 Eli 說「看起來 OK」→ Eli 會把 main merge 到 production → 上正式版

## ⚙️ 分支設定

- `main` → GitHub Pages 自動部署 → 🧪 測試版
- `production` → Cloudflare Pages 自動部署 → ✅ 正式版（`thanks.nii.school`）

## 相關專案

- [nii-business-landing](https://github.com/heyitseliii/nii-business-landing) — B2B 企業日文培訓 Landing Page
- [nii-student-handbooks](https://github.com/heyitseliii/nii-student-handbooks) — 各班學生手冊
