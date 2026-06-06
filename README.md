# liff-sales-report-15b

中科 15B 業績 + 工時回報 LIFF。

- LIFF ID: `2010233112-XCCgtapU`
- Public URL: https://posiloop.github.io/liff-sales-report-15b/
- Endpoint URL（在 LINE Developers Console 設定）：同上
- Scope 必要：`profile`、`openid`、`chat_message.write`

## 員工清單

修改 `employees.json`（fetch 時帶 cache-buster `?v=Date.now()`，commit + push 即時生效）。

## 功能

- 自動帶入今日民國日期 / 場域 / 填寫人
- 來客數 → 自動算客單價
- 4 餐別（午餐 / 晚餐 / 燃肌餐 / 預訂餐）展開填餐數+營業額
- 全日營業額自動加總
- 本月累積：localStorage（key 按 ROC 年月），可手動修正
- 員工 +選 + 工時：上班/下班滑桿（0.5 步）、休息/加班滑桿（0.5 步，0–6h）
- 「其他」可手填員工姓名
- 送 Flex Message 進當前 LINE 聊天室
