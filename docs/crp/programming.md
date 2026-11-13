# SmartFusion2 韌體開發與燒錄

本頁提供**上手導覽**，並非完整的正式燒錄操作程序。

## 既有教學資料

- [CRP 韌體專案（私有）](https://github.com/Mondayhs/compact-radiation-probe)
- [SmartFusion2 燒錄教學影片](https://youtu.be/LCdHjrpG3Nc)
- [COSPAR-1 CRP 硬體燒錄注意事項影片](https://youtube.com/shorts/jd6NB5zPXXo)

上述影片連結來自原交接文件。正式對外使用前，仍應確認影片內容及公開權限。

## 開發與版本管理原則

- 每次操作都應記錄 **PCB 版本、韌體 Branch／Commit、ICD 版本與測試程式版本**。
- 進行實驗性修改時，請建立自己的 Git Branch，不要直接覆蓋正式基準版本。
- 必須依團隊核准的工具版本、燒錄檔案與板件操作程序進行。
- 燒錄後應確認實際執行的韌體版本，並保存相關 HK 或主控臺紀錄。

## UART Baud Rate 修改注意事項

變更 UART 鮑率（Baud Rate）時，不能只修改韌體，還必須確認接收端程式與通訊設定一致。請依對應版本的韌體、ICD 和整合測試結果操作。

## 待補正式操作資料

- [ ] 核准的供電與接線圖。
- [ ] SmartFusion2 工具鏈版本、安裝與專案設定。
- [ ] 編譯步驟、燒錄檔命名與檔案驗證。
- [ ] 燒錄失敗時的處理程序。
