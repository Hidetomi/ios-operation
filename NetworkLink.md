# ネットワーク

## 観点

  - オンライン
    - 正常
    - 通信遅延
    - 通信100%欠損
  - オフライン
    - 未接続

## 方法

### オフライン手順

- Network Link Conditioner
  1. Apple Developer Center から Hardware IO Tools っていうユーティリティ群をダウンロード。
  2. 起動すると、再現したいネットワーク状況が色々選べて、スイッチをONにするとMac上の通信が制限される。
  3. 他にも、自分で通信状態を細かく指定したカスタム環境も作成できる。 up/downそれぞれのLoss率と速度などなど。
  4. 操作できるのはパケットロスの度合いと通信速度までで、ネットワークON/OFFののテストしたいときは直接MacのwifiをON/OFFしてやることになりそう。
  5. 100% Lossとか使うとTimeoutのテストが手軽にできる。 

[iOS シミュレータでオフライン時のテストをしたい](https://qiita.com/hirocueki2/items/e4d5d7db236468384875)
[iOSシミュレータでの通信状態のテストにNetwork Link Conditionerが便利だった](https://yudoufu.hatenablog.jp/entry/2016/05/28/120951)
