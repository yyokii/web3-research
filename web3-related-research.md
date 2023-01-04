# Web3 Related Research

（メモ）

* pancake swap
* uniswap
* ブロックチェーンが提供する価値を明確にして、それが今後どんな風になっていくかを想像して流れを書き、それに沿うプロダクトをつくりたいかもしれない

## Web3

> Gavin Woodの定義 (ĐApps: What Web 3.0 Looks Likeより) 
>
> Web 3.0, or as might be termed the “post-Snowden” web, is a reimagination of the sorts of things that we already use the Web for, but with a fundamentally different model for the interactions between parties. Information that we assume to be public, we publish. Information that we assume to be agreed, we place on a consensus-ledger. Information that we assume to be private, we keep secret and never reveal. Communication always takes place over encrypted channels and only with pseudonymous identities as endpoints; never with anything traceable (such as IP addresses) . In short, we engineer the system to mathematically enforce our prior assumptions, since no government or organisation can reasonably be trusted. (原文まま) Web 3.0、あるいは「ポスト・スノーデン」webと呼ばれるものは、我々がすでにWebを利用している種類のものを再構築したものだが、当 事者間の相互作用については根本的に異なるモデルとなっている。公開されると想定される情報は、公開される。合意されたと思われる情 報は、合意記録簿に記録する。非公開と想定される情報は、秘密にし、決して公開しない。通信は常に暗号化されたチャネルで行われ、 エンドポイントには仮名IDのみを使用し、追跡可能なもの (IPアドレス等) は一切使用しない。つまり、政府や組織は合理的に信頼するこ とができないので、私たちは数学的に事前の仮定を強制するようにシステムを設計する。

> Chris Dixonの定義
>
> web3 is the internet owned by the builders and users, orchestrated with tokens. web3とは、トークンで組織化・統合された、ビルダーとユーザーによって所有されるインターネットである

> a16zの定義
>
> Web 3—a group of technologies that encompasses blockchain, cryptographic protocols, digital assets, decentralized finance and social platforms, NFTs, and DAOs—is the third generation of the internet. ブロックチェーン、暗号プロトコル、デジタルアセット、分散型金融・社会プラットフォーム、NFT、DAOを包含す る技術群であるWeb 3は、インターネットの第3世代である。

[web3Research2023](https://blockchain.bitflyer.com/pdf/web3Research2023.pdf)

web3の定義は様々あるようだが「Gavin Woodの定義」が最初の意である。それを実現する手段としてブロックチェーン技術があり、現在はweb3というとブロックチェーン技術を用いたもの、という解釈になっている。

そしてそこでは中央集権的な仕組みはなくても機能する。
→ 機能はするであろうが、特定事業者があることで得られていたメリットもありそう。それを担保できる仕組みはプロダクトのアイデアになるかもしれない。

## GameFi

## DeFi

## DAO

## NFT

Non-Fungible Token

* ロイヤリティを設定することで著作者が二次流通以降も報酬を得る仕組みを作れる
* デジタルデータに価値を付与できる
  * **ブロックチェーンが新たに付与する価値 = 発行者、オーナーシップを明確にできる**

## SFT

Semi-Fungible Token

>  FT (ERC20) とNFT (ERC721) の規格の課題の一つは、一つのスマートコントラクトがそれぞれ一種類のトークンしかサポート出来ない点で あった。例えば、ゲーム内で新しい種類のNFTアイテムを作るたびに、それに対応する新しいスマートコントラクトを作成する必要があった。しかし、SFT (ERC1155) を利用することで、一つのスマートコントラクトだけでゲーム内に様々なアイテムを作ることが可能になった

[web3Research2023](https://blockchain.bitflyer.com/pdf/web3Research2023.pdf)

> - **FT（トークン）【ERC-20】**
>   ”数値(Value)”の認識だけが可能。自分が持つ1Ethと相手が持つ1Ethの間に違いはなく識別はできない。ただ、相手から1Eth貰えば自分は2Ethに、相手は0Ethとなり、増減の記録は可能。代替可能性を持つ。
> - **NFT【ERC-721】**”モノ**(**ID)”の認識だけが可能。モノというとややこしいかもしれませんが、固有であることが認識可能。世界に一つだけの唯一性を持ったトークンを生成可能
>
> ですが、例えば個数制限はしたいけど同じ種類のアイテムが複数存在する”ゲーム内アイテム”や”チケット”のNFTを作る際に現状のNFTのERC-721では少し困ります。
>
> NFTは全てを固有のもの（ID）で認識するので、固有のNFTを個数分作成する必要があります。この場合、同じデータを持った別のNFTとなるので全ての作成にガス代がかかってしまうのと、コントラクトの変更等のデータ変更を一つ一つする必要があります。SFTを活用すれば、それらの問題を解決できます。

[【SFT】NFTの次なるムーブメント「Semi Fungible Token」とは？ERC-3525規格を用い、金融特化NFTを活用する「Solv Protocol」も事例として解説！](https://substack.com/inbox/post/94529671)

<image width="400" src="https://user-images.githubusercontent.com/20992687/210601117-c33d1e2a-1904-495c-ada7-7451a2512739.jpeg">
https://whitepaper.sftlabs.io/SFT%20Whitepaper.pdf より

固有のIDに加えてその数量(value)とその種別（slot）を持つのが特徴。
* valueがあることで同一規格のものを複数生成しなくて良い
* slotがあることで同一種別での統合、分割が可能
 

## アイデア

* githubなどの自分がよく使うサービスへの展開を想像すると良さそう、興味湧く
* 一部の色を塗れるとかの権利をtokenかするのも面白そう、hashmasksぽいけど
* イベントに合わせたNFTを作成できるもの
  * ボタン生成アプリみたいに、自由に自分達で作成できてもいいかも。それが発行されたら作成者にもお金が入るとか。

## Products

### Solv Protocol

[Solv](https://solv.finance/home)

* 金融系NFTの作成&売買ができるプラットフォーム
* Vesting Voucher, Convertible Voucher, Bond Voucher という3種類のプロダクト（金融商品NFT）の作成とそのマーケットを提供
* ERC3525を利用している
 
### [NFT] Hashmasks

[Hashmasks](https://www.thehashmasks.com/)

NFT × DeFi活用 になっているのがすごい

* 16,384枚限定
* 1作品保有で1にに10NCT溜まる
  * NCT（Name Change Token）
  * 1830NCTで名前をつけたり、変更したりする権利を実行できる
  * uniswapでNCTの取引可能
  * 2022/1月時点で1NCT≒10円、1作品で一日100円の収入
  * 名前がついた作品は元より価値があがることもある→NCTの価値が上がる
  * NCTは10年後発行されなくなる = 命名コストは高まる
* 作品の商標利用可能
* 作人自体に謎解き要素あり
* 作品、作者の情報が最初は非公開
* 人気、不人気（ロングテール）の存在。ロングテールなものを持っているオーナーが売りたくなる。そうなるとHashmasks全体の価値も少し下がる
  * 作品を預けて1MASK をもらえる。1MASK使うとプールからランダムで1作品もらえる。飽きたら預けるとかできる。
  * MASKトークンは預けられた作品の平均価格
  * SushiswapでMASKが取引されている
  * Hashmasksの作品には興味ないがプロジェクトは面白いので投資対象として参加したい、と思う人が出てくる。→MASKの価値が上がる = 預けられている作品の価値も上がる。ロングテールなものが価値を下支える。

#### 参考

* [なぜDeFiの次がNFTなのか？５つの理由【徹底解説シリーズ】](https://www.youtube.com/watch?v=sxPg4Isx7DE)

（所感）

デジタルコンテンツを持つことでそれが見せびらかし効果をもたらすことは今はそれほど大きくはない。が、それが重要になってきたらこういう作品はより価値高まる。
そうでない今は、それを取り巻く仕組みの面白さ、真新しさから興味が湧いて、とりあえずやってみて上手くいくと嬉しいという遊び/娯楽みたいな感覚が強そう。
**今は作品以外の価値や、リアルでのやり取りまでがあるものはより意味を持ちそう。**そういう意味ではhashmaskの謎解き要素や作者を少しずつ？公開していくのは作品それ自体以外での価値提供があって面白いなと。名前つけれるとかMASKでのガチャ要素もそう。**デジタルだからこそ容易になる仕組みは面白い。**

## Redings

* [なぜDeFiの次がNFTなのか？５つの理由【徹底解説シリーズ】](https://www.youtube.com/watch?v=sxPg4Isx7DE)
  * デジタルコンテンツに価値が付きだす、これがNFTのすごいことらしい
    → 何がなんでも価値がつけばいいというわけではないとも思う。価値がつくべきものってなんだろうか。アートとかはまあわかる気もする。
