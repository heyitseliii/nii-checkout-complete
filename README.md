# nii-checkout-complete

泥日教育 — 開課快手購課完成後的轉跳頁。

## 用途

同學在**開課快手**後台購買課程並完成結帳後，會被導向這個頁面，作為「報名完成」確認畫面。

## 預覽網址（對外）

<https://heyitseliii.github.io/nii-checkout-complete/>

> 這組 URL 會填到開課快手後台作為購買完成後的轉跳頁。

## 檔案結構

```
.
├── index.html   # 報名完成頁（單頁、內嵌樣式）
└── README.md
```

## 給同事的測試流程

1. 直接打開預覽網址即可檢視
2. 如要改文案或樣式，clone 這個 repo，改 `index.html`，commit & push 到 `main`
3. Push 後 1–3 分鐘 GitHub Pages 會自動重新部署

```bash
git clone https://github.com/heyitseliii/nii-checkout-complete.git
cd nii-checkout-complete
# 編輯 index.html
git add index.html
git commit -m "更新文案"
git push
```

## 相關專案

- [nii-business-landing](https://github.com/heyitseliii/nii-business-landing) — B2B 企業日文培訓 Landing Page
- [nii-student-handbooks](https://github.com/heyitseliii/nii-student-handbooks) — 各班學生手冊
