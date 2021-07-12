# For Builders

> 越多開發者上架各式各樣的 Cube，就能有越多用戶創造更多利潤發現組合，進而找到市場機會並將利潤最大化。

如 [Ben Thompson 的聚合理論](https://stratechery.com/2017/defining-aggregators/)開發者 Builder 能讓 Furucombo 對更多用戶更具吸引力，進而吸引更多 Builder 並形成良性循環。

## 在 Furucombo 上架 Cube 的優點

當前 DeFi 產業中，協議開發者面臨的主要挑戰

* 從頭開始引導流動性；
* 由於可組合性的性質，需要與其他協議進行交互；
* 缺乏前端資源來提供直觀的用戶體驗。

Furucombo 就是為了解決以上問題而存在。Furucombo 強調協議層上的 UX/UI，讓上架到 Furucombo 的Builder 能專注於核心底層功能來加速開發，且因在 Furucombo 上架的協議能夠輕易地和其他協議串接，更能輕易達到共享和吸引流量而不用重頭開始。

## 如何上架至 Furucombo

1. 在 COMBO 論壇上提出想上架的內容並收集大家的意見
2. 在 COMBO 治理平台上獲得 Governor 的投票支持
3. 根據 Cube Listing Policy 開發智慧合約來將自身協議串接至 Furucombo 上
4. 向 Operator 提交合約內容並安排資安稽核（現任 Operator：Furucombo 創始團隊）
5. Operator 使用多重簽名錢包在 Furucombo 系統中註冊通過稽核的合約
6. 鎖定 COMBO 至治理平台以正式啟用通過稽核的合約 -&gt; 完成上架！

## 安全層面

Furucombo 的整體安全性與 Furucombo 協議支援中的所有 DeFis 呈高度相關，亦即每個新上架的協議都會影響整體的安全性，因此我們強調從源頭，也就是從 Cube 開發質量和流程開始做規範。

#### Cube Listing Policy

1. 開發指南：包含了開發能串接至 Furucombo 上智慧合約的基本說明
2. 風險因子：不同類型的智慧合約會有不同的風險因子，像是 Flashloan cube 的風險通常會比 Swap cube 來得高，而不同的風險因子則會影響 COMBO 承諾金和稽核流程。
3. COMBO 承諾金：在 Furucombo 協議啟用通過稽核的合約時，需要在治理平台上鎖定一定數量的 COMBO 作為承諾金。若欲取回該筆承諾金，Builder 須先解鎖，而解鎖將觸發冷卻期，且相應的 Cube將立即被下架。

{% hint style="info" %}
擁有足夠數量 vCOMBO 的 Furucombo Governor 也可以提供承諾金以啟動通過稽核的合約。反之亦然，任何提供承諾金的人都可參與治理並擁有 Governor 的權利。
{% endhint %}

#### Regular Audit

Furucombo Operator（現任：Furucombo 創始團隊）將安排並定期進行內部和外部稽核，以確保隨著協議的發展，能有越來越多有經驗的專家以不同角度稽核及檢視合約。

#### Insurance Policy

當 Cube 執行惡意行為時，其相應的 COMBO 承諾金將被沒收並發送到 Furucombo Reserve，同時 Operator 會立即將該 Cube 從系統下架。

另一方面，Furucombo Governor 可以分配 Furucombo Treasury 的資金，為整體用戶從外部保險協議承保或購買保險，以應不時之需。

## Builder 究竟怎麼當？來舉個例子吧

#### 在你的 Cube 成功上架前:

1. 在[治理論壇](https://forum.furucombo.app/)上提出你的想法
2. 與社區的其他成員討論尋求共識及支持
3. 找到一位認同你的想法、願意幫你在治理平台上正式提案的 Governor。或者你可以自行取得足夠的 vCOMBO 以成為 Governor 並自行提案
4. 如果提案獲得多數 Governor 的支持並通過投票，你即可開始根據 Cube Listing Policy 開發智慧合約
5. 合約準備好後，提交給 Operator 並安排資安稽核（現任 Operator：Furucombo 創始團隊）
6. 如果通過稽核，Operator 將使用多重簽名錢包在 Furucombo 系統中註冊此通過稽核的合約
7. 你需要從公開市場獲得一些 COMBO 代幣，例如[從 Uniswap 買進 COMBO](https://furucombo.app/combo/c3gnmecke6ss71ddm290)，再將這些 COMBO 代幣鎖定到治理平台中來支付承諾金並且正式啟動你的 Cube。此外，你也可以事先向 Furucombo Governor 尋求贊助

#### 在你的 Cube 成功上架後:

1. 當你鎖定 COMBO 來支付承諾金後，你也成了 Furucombo Governor 之一。希望你能積極參與🙂
2. 隨著 DeFi 的快速發展，你需要不時跟進你的 Cube 連接的協議，例如你上架的是 Aave flashloan cube，當 Aave 合約有更新時，你可能需要升級 Cube 的智慧合約以使其能繼續正常工作。
3. 當你開發的 Cube 開始累積交易量後，你也可以從 Furucombo Governance 平台申請額外的獎勵金。

## 釋出計畫

{% hint style="info" %}
由於 DeFi 快速發展和難以預測的特性，我們的計劃有可能會因應市場變動而做動態調整。
{% endhint %}

| 項目 | 進度 |
| :--- | :--- |
| [Furucombo 協議合約開源](https://docs.furucombo.app/resources/smart-contracts) | 已上線 |
| 試辦外部開發者參與開發 \([Sushiswap and B.Protocol](https://furucombo.app/combo)\) | 已完成並上架 |
| Cube Listing Policy | 規劃中 |
| Cube 流量儀表板 | 規劃中 |
| 自動化啟動 Cube 的智慧合約 | 規劃中 |



