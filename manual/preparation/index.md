[Arbitious利用マニュアル](../) ＞ 事前準備

# 事前準備

Arbitiousで裁定取引を行うために、次の準備が必要です。

1. 仮想通貨取引所の口座開設
1. 取引所への入金
1. APIキーの取得

以下、順番に解説します。

## 1. 仮想通貨取引所の口座開設

次の4取引所で口座を開設します(Coincheck以外)。

| 取引所            | 公式サイトURL    | 備考 |
|:-----------|:------------|:------------|
| **bitFlyer**         | [<https://bitflyer.jp/>](https://bitflyer.jp/) | |
| **bitbank<span>.</span>cc**      | [https://bitbank.cc/](https://bitbank.cc/)  | |
| **BTCBox**            | [https://www.btcbox.co.jp/](https://www.btcbox.co.jp/)  |  |
| **Quoine**         | [https://ja.quoinex.com/](https://ja.quoinex.com/) | |
| ~~Coincheck~~       | ~~https<span>://coincheck.com/ja/</span>~~   | ▲現在新規受付停止中のため開設不可(2018/5/1現在) |

- [口座開設方法：bitFlyer](./openaccount_bf)

- [口座開設方法：bitbank.cc](./openaccount_bb)

- [口座開設方法：BTCBox](./openaccount_bx)

- [口座開設方法：Quoine](./openaccount_qn)

## 2. 取引所への入金

次に、開設した口座へ運用資金を入金します。各取引所への理想的な資金配分率は次の通りです。

| 取引所 | 資金配分率 | 備考 |
|:----|:------|:--|
| bitFlyer | 30% | |
| bitbank<span>.</span>cc | 30% | |
| BTCBox | 30% | |
| Quoine | 10% | レバレッジ取引(最大10倍)のため、現物口座の入金額の1/3でよい。BTCは購入不要 |
| ~~Coincheck~~ | | ▲現在新規受付停止中のため開設不可(2018/5/1現在)|

次に、bitFlyer・bitbank・BTCBoxの各取引所で入金額の半額相当のBTCを購入します(Quoineはレバレッジ取引のためBTC購入不要)。  
たとえば運用資金100万円のとき、上記3つの取引所へは30万円を入金し、その後15万円分のBTCを購入します。Quoineへは10万円の入金のみ行います。

## 3. APIキーの取得

各取引所へログインし、APIキーを取得します。APIキーは、Arbitiousが自動で裁定取引を行うために必要となるものです。
APIキーの呼び方は取引所によって異なりますが、IDとKeyに相当する2つの値で構成されます。

| 取引所            | APIキー(ID) 呼称 | APIキー(Key) 呼称 |
|:-----------|:------------|:------------|
| bitFlyer         | API Secret | API Secret |
| bitbank<span>.</span>cc      | APIキー | シークレット |
| BTCBox            | 公開鍵 | 秘密鍵 |
| Quoine         | トークンID | トークン値 |
| ~~Coincheck~~       | アクセスキー | シークレットアクセスキー |


APIキーは決して他人に知られないように**厳重に取り扱ってください**。


- [APIキーの取得方法：bitFlyer](./getapikey_bf)
- [APIキーの取得方法：bitbank<span>.</span>cc](./getapikey_bb)
- [APIキーの取得方法：BTCBox](./getapikey_bx)
- [APIキーの取得方法：Quoine](./getapikey_qn)
