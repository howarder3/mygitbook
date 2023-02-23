---
description: 冷錢包
---

# 冷錢包

* 轉帳 BTC 到鏈上
* Ledger&#x20;
* Native SegWit (default account type)&#x20;
  * Native SegWit accounts create Bitcoin deposit addresses starting with **bc1q**. Native SegWit accounts offer better protection against typos and are cheaper to spend from compared to SegWit or Legacy accounts.
  * 其中 Native SegWit 帳戶是預設帳戶類型，它可以創建以 bc1q 開頭的比特幣存款地址，相較於 SegWit 和 Legacy 帳戶，使用 Native SegWit 帳戶更加防範錯誤輸入，且花費比較便宜。
  * Native SegWit, also known as Bech32 addresses, is considered the most efficient and secure type of Bitcoin address. Transactions sent from Native SegWit addresses typically have lower fees and are faster to confirm than those sent from other address types. Additionally, Native SegWit addresses offer enhanced security features that make them less vulnerable to certain types of attacks.
* SegWit&#x20;
  * SegWit accounts create Bitcoin deposit addresses starting with a **3**. The SegWit upgrade reduced [network fees](https://medium.com/@jimmysong/understanding-segwit-block-size-fd901b87c9d4), sped up [transaction signing](https://segwit.org/segregated-witness-and-hardware-wallets-cc88ba532fb3) on hardware wallets, and enabled second-layer solutions like the [Lightning Network](https://lightning.network/).
  * SegWit 帳戶可以創建以 3 開頭的比特幣存款地址，SegWit 升級降低了網絡費用、加快了硬件錢包的交易簽署速度，並啟用了第二層解決方案，如閃電網絡。
  * SegWit addresses, also known as P2SH (Pay-to-Script-Hash) addresses, were introduced as an improvement to the original Bitcoin protocol to help address scalability issues. While SegWit addresses are still more secure than Legacy addresses, they are generally less efficient than Native SegWit addresses.
* Taproot&#x20;
  * Taproot accounts create Bitcoin deposit addresses starting with **bc1p.** Taproot is the newest Bitcoin account type. You can learn more about Taproot and how to add a Taproot account [**here**](https://support.ledger.com/hc/en-us/articles/4410908103185-Creating-a-Bitcoin-Taproot-account-in-Ledger-Live?docs=true).
  * Taproot 帳戶可以創建以 bc1p 開頭的比特幣存款地址，是最新的比特幣帳戶類型。
  * Taproot is a new Bitcoin protocol upgrade that aims to improve the privacy, security, and efficiency of transactions. It is compatible with all three address types and will provide enhanced security features to each. Once Taproot is activated, it is expected to become the default standard for Bitcoin transactions.
* Legacy
  * Legacy accounts create Bitcoin deposit addresses starting with a **1**. Legacy is the oldest and the least efficient type of Bitcoin account.
  * Creating a Legacy Bitcoin account in Ledger Live can be **useful to receive BTC from crypto exchanges that don't support withdrawing to newer account types like SegWit, Native SegWit or Taproot**.
  * Legacy 帳戶可以創建以 1 開頭的比特幣存款地址，是最古老且效率最低的比特幣帳戶類型。
  * 在 Ledger Live 中創建 Legacy 比特幣帳戶可以用於從不支持新型帳戶類型（如 SegWit、Native SegWit 或 Taproot）提取資產的加密貨幣交易所接收比特幣。
* [https://support.ledger.com/hc/en-us/articles/115005195945-Bitcoin-BTC-?support=true](https://support.ledger.com/hc/en-us/articles/115005195945-Bitcoin-BTC-?support=true)
* In summary, all three address types are considered safe, but Native SegWit is the most efficient and secure option. Taproot is a new protocol upgrade that will provide additional security features to all address types.\
