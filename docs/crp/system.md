# CRP 系統架構

CRP 主要包含兩類輻射量測：

- **RADFET**：透過臨界電壓變化評估總游離輻射劑量（TID）；判讀時須考量溫度影響與校正方式。
- **NAND Flash**：觀測輻射造成的位元錯誤，並分析 Erased／Programmed 狀態及讀取驗證結果。

## 主要功能區塊

1. 輻射感測元件及相關類比量測電路。
2. 以 SmartFusion2 為核心的數位控制與韌體。
3. 用於科學紀錄及部分設定參數的非揮發性記憶體。
4. 與衛星平台連接的通訊介面。
5. Housekeeping（HK）狀態資料與 Science（SCI）科學量測資料。

## 硬體文件閱讀順序

建議先確認整體功能方塊圖、供電架構與 PCB 版本，再查看接線及介面文件。

完整電路與板件設計請至[CRP 私有 Repository](https://github.com/Mondayhs/compact-radiation-probe)查閱。**本公開頁面不提供可直接用於接線與供電的完整規格。**

接下來可閱讀[韌體開發與燒錄](programming.md)、[HK／SCI 資料流程](data-flow.md)或[第一次測試指南](../testing/first-test.md)。
