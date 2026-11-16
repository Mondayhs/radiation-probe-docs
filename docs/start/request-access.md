# 申請工程文件存取權限

新人如果想閱讀完整的 **CRP ICD、測試 SOP、硬體文件或測試報告**，請先申請私有工程文件庫的存取權限。

## 申請步驟

1. **登入 GitHub**，點選下方的 **Request Access**。
2. 填寫「**姓名或團隊內可辨識的稱呼**」及「**GitHub Username**」，選擇與專案的關係與需要的資料。
3. 送出後，專案管理者會在 GitHub Issues 中看到申請，確認身分後發出私有 Repository 邀請。
4. **到 GitHub 通知或電子郵件接受邀請**，即可查看已授權的工程文件。

[**Request Access｜填寫存取申請**](https://github.com/Mondayhs/radiation-probe-docs/issues/new?template=access-request.yml){ .md-button .md-button--primary }

!!! warning "公開申請表的注意事項"
    申請使用的是**公開 Repository 的 GitHub Issue**，所以填寫的稱呼與 GitHub 帳號會被其他人看到。請使用團隊可辨識的名字、縮寫或英文名；**不要填寫學號、電話、私人電子郵件或其他敏感個資**。管理者若需要核對完整姓名，應另外透過私下聯絡方式確認。

## 我已提出申請，但還是無法查看？

- 確認你用來登入的 GitHub 帳號，與申請表中的 Username 一致。
- 確認是否收到邀請，並已在 GitHub 上點選 **Accept invitation**。
- 私有 Repository 的連結本身**不會自動授權**。
- 若申請超過預期時間，請透過團隊既有聯絡方式通知管理者。

## 管理者：如何審核

1. [查看 Access Request 申請](https://github.com/Mondayhs/radiation-probe-docs/issues?q=is%3Aissue+is%3Aopen+in%3Atitle+%22Access+Request%22)。
2. 確認申請者的團隊身分與 GitHub Username（必要時私下核對）。
3. 開啟[工程文件庫存取設定](https://github.com/Mondayhs/radiation-probe-engineering/settings/access)，選擇 **Add people**，輸入確認過的 Username 並發出邀請。
4. 邀請者接受後，回到原申請 Issue，回覆「已寄出邀請」並關閉。

!!! danger "目前 GitHub 權限限制"
    `radiation-probe-engineering` 目前屬於個人帳號 `Mondayhs`。GitHub 個人帳號的 Private Repository **Collaborator 具備寫入權限，不是唯讀**。因此只應邀請可信任的團隊成員；若希望新人只有讀取權限，建議未來轉移到實驗室 GitHub Organization，再依角色授予 **Read** 權限。

!!! info "不是自動一鍵核准"
    本版本已簡化為「填申請 → 管理者按連結邀請」。目前未使用有管理權限的 Token 自動授權，避免公開申請表引發錯誤授權或增加憑證風險。
