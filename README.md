# NCU 輻射探測酬載交接知識庫

本 Repository 用於維護 **DSRP → CRP／COSPAR-1** 的公開新人入門網站與工程交接文件索引。

> **文件狀態：交接草稿。** 本站內容不是經核准的飛行操作程序。韌體、硬體設計、詳細 ICD、帳號密碼與未公開測試紀錄，請放在有權限控管的私有 Repository。

## 網站網址

https://mondayhs.github.io/radiation-probe-docs/

## 本機預覽

```powershell
py -m pip install -r requirements.txt
mkdocs serve
```

網站文件位於 `docs/`，以 Markdown 編寫。編輯後請確認適用的韌體、硬體與 ICD 版本，再提交修改。

## 公開與私有資料分工

- **公開：** 新人導覽、任務概念、設計演進摘要、已核准的教學內容及工程資源索引。
- **私有：** 原始程式碼、電路設計、詳細介面、未公開測試資料及校正紀錄。

本站已設定要求搜尋引擎不要收錄，但仍為公開網站，不具備存取權限保護。
