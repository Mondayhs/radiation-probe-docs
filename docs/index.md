# 輻射探測酬載交接知識庫

**深空輻射探測儀（DSRP）｜小型輻射探測儀（CRP）｜COSPAR-1**

歡迎使用國立中央大學輻射酬載交接網站。本網站希望讓新進成員循序了解**任務背景、設計考量、工程資料位置與測試入門流程**，並保留 DSRP 實飛經驗延續至 CRP 的研發脈絡。

!!! warning "公開入門文件，非正式飛行操作程序"
    本網站目前為交接文件草稿。進行任何硬體操作前，應以對應的硬體版本、韌體 Commit、ICD 版本與團隊核准的測試程序為準。請勿將私有工程資料上傳至本站。

## 我想先了解……

<div class="grid cards" markdown>

- :material-school: **我是第一次接觸這個專案**

    [閱讀第一週上手指南 →](start/first-week.md)

- :material-satellite-variant: **DSRP 與 CRP 分別是什麼？**

    [認識兩項任務 →](mission/overview.md)

- :material-source-branch: **為什麼要從 DSRP 改版成 CRP？**

    [查看設計演進與改良項目 →](mission/design-evolution.md)

- :material-flask-outline: **我要準備第一次 CRP 測試**

    [閱讀測試入門指南 →](testing/first-test.md)

- :material-alert-circle-outline: **遇到異常，不知道從哪裡查**

    [查看異常排除索引 →](troubleshooting.md)

- :material-bookshelf: **我要找程式、ICD 或測試資料**

    [前往工程資源索引 →](resources.md)

</div>

## 建議學習順序

**認識任務 → 確認硬體與韌體版本 → 閱讀對應 ICD → 確認核准的接線與供電方式 → 觀察 HK → 驗證 SCI 並保存測試紀錄。**

!!! info "資料判讀提醒"
    **能持續收到 HK，不代表科學量測一定正常。** 判讀時應同時確認 SCI 紀錄、時間、原始資料與解析程式版本，避免將舊資料或解析錯誤誤判為新量測。

## 文件存放原則

本站只放可公開的入門教材與工程文件索引。完整韌體、電路設計、未公開測試資料及詳細介面文件，仍由具備權限的成員透過私有 GitHub Repository 存取。

## 需要工程文件權限嗎？

ICD、正式測試 SOP 與內部工程資料保存在 Private Repository。新進成員可先[申請存取權限](start/request-access.md)，提供 GitHub Username 與團隊內可辨識稱呼，經管理者確認後由 GitHub 發出邀請。

[**Request Access｜申請工程文件權限**](start/request-access.md){ .md-button .md-button--primary }

正式使用前，請先查看[版本與驗證狀態](maintenance/release-status.md)。
