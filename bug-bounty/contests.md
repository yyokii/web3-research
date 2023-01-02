# Bug Bounty

テンプレート

```.md
# [コンテスト名]()

## Research

## Report

### [yoki {type}] title
### Summary
### Vulnerability Detail
### Code Snippet
### Tool used
Manual Review
### Recommendation

```

チェックリスト

* solidityのバージョンが0.8以上か :
* `tx.origin`を利用していない : 
  * Phishing with tx.origin 
* `block.timestamp`をコントラクトのメインロジックで使用していない : 
  * Block Timestamp Manipulation
* 機密情報にあたるものはない : 
  * Accessing Private Data

# [2022/12 Caviar contest](https://code4rena.com/contests/2022-12-caviar-contest)

[Caviar](https://goerli.caviar.sh/) is a fully on-chain NFT AMM that allows you to trade every NFT in a collection (from floors to superrares). You can also trade fractional amounts of each NFT too.
It's designed with a heavy emphasis on composability, flexibility and usability. 

## Research

* AMM
  * [AMM（自動マーケットメイカー）とは｜仕組みやリスクを解説](https://coinpost.jp/?p=304625)

  * [オーダーブックとAMMを解説！ | クリプト調査局](https://gg-crb.com/2021/06/11/%E3%82%AA%E3%83%BC%E3%83%80%E3%83%BC%E3%83%96%E3%83%83%E3%82%AF%E3%81%A8amm%E3%82%92%E8%A7%A3%E8%AA%AC%EF%BC%81/#toc2)

* ステーキング

  * [ステーキング | 仮想通貨ビットコイン（Bitcoin）の購入/販売所/取引所【bitFlyer（ビットフライヤー)】](https://bitflyer.com/ja-jp/s/glossary/staking)
  * ネットワークへの参加で報酬がもらえる仕組み。利子みたいなもの。

* fractional token
  *  NFTの所有権を分割したもの

* LPトークン
  * Liquidity Provider（流動性提供者）トークン

  * AMM型の分散型取引所（DEX）に流動性を提供する対価として受け取ることができる。また、提供した通貨を回収する際に必要となる証明書のようなもの。

* マークルプルーフ
  * コントラクトにはマークルルートを保存するだけでデータの検証を行うことができるのでガス代の節約になる
  * https://zenn.dev/jpyc/articles/73af0e7d914d86


## Report

no