# Web3 Related Research

（メモ、調べたいトピックなど）

* https://twitter.com/wecandaoit_jp/status/1629687021487919104 ここの知らないワードを調べる
* ゼロ知識署名
* ICP
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

## ブロックチェーン

### パラチェーン

> パラチェーンとは、ポルカドットのメインチェーンである “Relay Chain” に接続しているシャードチェーンを指す
> ブリッジ機能により、イーサリアムやビットコインなど、外部のブロックチェーンをパラチェーンとして接続することができる

[web3Research2023](https://blockchain.bitflyer.com/pdf/web3Research2023.pdf)


### Astar

* X-VM
  * イーサリアムの仮想マシン (EVM)
  * WebAssembly (WASM) の仮想マシン
* DApps Staking
* Layer2 Solution

Layer2: オンチェーンからTXをオフチェーンに渡し、オフチェーン側で渡されたTXを全て実行。その時のStateをstate channelでオンチェーンに戻し検証
[web3Research2023](https://blockchain.bitflyer.com/pdf/web3Research2023.pdf)

主な開発ツール
* Swanky-cli
  * ethereumで言うところのHardhatのwasm開発用
* OpenBrush
  * ethereumで言うところのOpenZeppelin


## ブロックチェーンらしさ

* ユーザーが作成したコンテンツの所有者は作成者自身のものとなる
  * プラットフォーマー（YoutubeやTwitter）のものとなる場合、それを利用して広告を載せることがビジネスとなる。
  　　* （本題ではないが、）　そもそも広告はそんなに嫌？CM自体の面白さがあったり、流行りをしれるので絶対回避したいものではない。嫌だとすれば広告削除機能がなかったり合っても価格がたかいとか
* 透明性: 誰でもアクセス可能である
* 永続性: 管理者がいなくとも動き続ける
* 厳密性: コントラクトが自動処理を行う
  * ≒ 意思決定の自動化
* データの安全性: 改竄が難しい

[シリコンバレーのエンジニアはＷｅｂ３の未来に何を見るのか](https://www.amazon.co.jp/%E3%82%B7%E3%83%AA%E3%82%B3%E3%83%B3%E3%83%90%E3%83%AC%E3%83%BC%E3%81%AE%E3%82%A8%E3%83%B3%E3%82%B8%E3%83%8B%E3%82%A2%E3%81%AF%EF%BC%B7%EF%BD%85%EF%BD%82%EF%BC%93%E3%81%AE%E6%9C%AA%E6%9D%A5%E3%81%AB%E4%BD%95%E3%82%92%E8%A6%8B%E3%82%8B%E3%81%AE%E3%81%8B-%E4%B8%AD%E5%B3%B6%E8%81%A1/dp/4815617864)

## GameFi

* プロダクトそれ自体に魅力がないと、すぐにユーザーが離れて関連トークンは暴落する

## DeFi

## DAO

スマートコントラクトを用いた仕組みの自動化による
* 透明性
* 参加者による民主制の実現

が可能であることが魅力。

## NFT

Non-Fungible Token

* ロイヤリティを設定することで著作者が二次流通以降も報酬を得る仕組みを作れる
* デジタルデータに価値を付与できる
  * **ブロックチェーンが新たに付与する価値 = 発行者、オーナーシップを明確にできる**

NFT Artは所有権を示すだけで、コピーできるから微妙という意見があるが、購入者や作者はコピーできることに意味を感じている。
デジタルアートをNFT化することは
* 作者: コアなファンに所有権をという価値を与える（= 人気の可視化）。主にDiscordを通じてコアなファンとの繋がりが生まれる。二次流通でもロイヤリティで儲かる。従って作品が購入された後も発信する/拡散されることは嬉しい（ファンの獲得 + コミュニティ形成 + ロイヤリティによるインセンティブ（芸術家はこれへの興味薄そう））。つまりNFT Artの販売を通して生まれる繋がりに価値を感じている。
* 購入者: 主にDiscordを通じて作者との繋がりが生まれる。プロフィールアイコンなどにしてweb上で「見せびらかし」（物理的な作品より「見せびらかし」が自然にできる。）。Artに人気が出ることは承認欲求が満たされるし、資産の価値上昇にもなるのでみんなに見て欲しいという欲求が生まれる。

NFT Artによる所有権の付与は、コアなファンであることの可視化であり、それにより作者と購入者の繋がりが生まれる。それこそがNFT Artの価値である。
従ってコピーできることは問題ではなく、作者や購入者はむしろコピーされることによる人気拡大を望むだろう。  
[(1) 【落合陽一】伊藤穰一と考える「インターネット98 to 22」 NFT、イーサリアム、デジタル通貨…「Web3.0」で世界はどう変わるのか？ - YouTube](https://www.youtube.com/watch?v=wBkjYQtu0rs)

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

## Wallet

* ウォレット
  * アドレスとその秘密鍵が集まったもの（アドレス:秘密鍵 = 1:1） 
* ホットウォレット: オンラインで管理
  * カストディアルウォレット: 第三者が秘密鍵を管理
  * ノンカストディアルウォレット: ユーザー自身が秘密鍵を管理
  * custodialは保管、保護の、という意味
* コールドウォレット: オフラインで管理


## Verifiable Credential
内容の検証がオンラインで可能な自己主権型のデジタル証明。  
[発行者](Issuer) が【保持者】(Holder) に対して発行した証明書を第三者である【検証者】が検証することができるしくみ。

![vc-data-model](https://user-images.githubusercontent.com/20992687/221598124-a3897c76-bffc-4027-b466-a15def35a6f8.png)  
引用: Verifiable Credentials Data Model v1.1

- **保有者(Holder)** : VCの所有者。 1 つ以上の**VCを所有し**、それらから**検証可能なプレゼンテ ーションを生成する**。例としては、学生、従業員、およびあるサービスの顧客などがある。
- **発行者(Issuer)** : 1 つ以上の対象についてのClaimを行い、Claimから**VC**を作成し、 Holderに送信することによってエンティティが果たす役割。発行者の例としては、企業、NPO、業界団体、政府、および個人がある。
- **サブジェクト(Subject)** : claimの対象となる実体。例えば、人間、動物、物などが含まれる。多くの場合、**VCの保有者と同一だが、そうでない場合もある。たとえば、親（保有者）が子供（対象者）の検証可能なクレデンシャルを保持する場合や、ペットの所有者（保有者）がペット（対象者）の**VCを保持する場合がある。これらの特殊なケースの詳細については、後述
- **検証者(Verifier)** プレゼンテーションを通じて、1 つ以上の**VC**を検証する役割。検証者の例としては、雇用者、セキュリティ要員、および Web サイトがある。
- **検証可能なデータ・レジストリ(Verifiable Data Registory**) システムが、識別子、キー、および他の関連データ（検証可能なクレデンシャル・スキーマ、失効レジス トリ、発行者公開キーなど）の作成と検証を媒介する役割で、**VC**を使用するために必要な場合がある。構成によっては、対象者に相関可能な識別子を必要とする場合がある。検証可能なデータ・レジストリの例には、**信頼できるデータベース、分散型データベース、政府 ID データベース、および分散型台帳**が含まれる。エコシステムで利用される検証可能なデータレジストリは、多くの場合、1種類以上ある。

「検証可能なプレゼンテーション(Verifiable Presentation)」とは、

> 1 つ以上のVCから派生したデータで、特定の検証者と共有されるもの。 ある種の検証可能なプレゼンテーションは、元のVCを含まないが、そこから合成されたデータを含むことがある。例えば、ゼロ知識証明などを利用し、詳細は開示しないが条件を満たしていることを証明することができる。

### 参考
* [Verifiable Credentials と 譲渡不可NFTを組み合わせたデジタル賞状の発行について](https://www.digital.go.jp/assets/contents/node/basic_page/field_ref_resources/b2cdde1e-f172-4277-9204-20bd006660f1/415114c7/20221021_meeting_web3_outline_01.pdf)
* [Verifiable Credentialsとは? -part.1 — 0xKantaro](https://mirror.xyz/kantaro.eth/jhpZpWcF697BKjeGGqlPA0IIMfsuJPCpLjfPC5oiLys)

## DID

![スクリーンショット 2023-02-28 0 22 15](https://user-images.githubusercontent.com/20992687/221610048-afcc6c1c-2ef0-4fff-931d-e7e728a59bed.png)  
引用: [DID(分散型ID)とは？概要説明から活用事例まで](https://zenn.dev/sakazuki_xyz/articles/did-introduction)

DID(Decentralized Identifier)
グローバル、ユニークかつ永続性のあるID。
ブロックチェーンなどの暗号技術を用いることにより一切の組織または政府から独立してユーザーが作成、所有、管理できるIDとなる。
Verifiable Credentialにおける、保有者/発行者IDで利用することがある。

構造: did:[method-name]:[method-specific-id]

- did
  - URIスキームのID
- DID method
  - DIDを運用する仕組みの種類
    - https://w3c.github.io/did-spec-registries/#did-methods
- DID Method-Specific Identifier
  - DID Methodの中の特定のIDです

### 参考
* [分散型IDのアプリケーション応用 2021-0617-IEICE-DPF-shigeya](https://www.ieice.org/~dpf/wp-content/uploads/2021/04/2021-0617-IEICE-DPF-shigeya.pdf)

## Products
 
### [VWBL](https://vwbl-protocol.org/)

* viewable
* [VWBL完全理解書](https://ango-ya.notion.site/VWBL-483519de492d4ce09559f2a20069a77b)
* デジタルコンテンツ自体に価値がある場合は見れない、ということも大事になる
* プレビューは誰でも見れるがNFT持っている人だけコンテンツを見れる
* VWBL = NFT + アクセスコントロール
* ビジネスモデル
  * コンテンツ流通の省コスト化
    * 手売りのような1:1の仕組み、手数料が余計にない
  * コンテンツ管理の省コスト化
    * 認証管理機能の開発が必要なくなる
  * 収益ポイント
    * 鍵管理ネットワーク手数料
    * トークンエコノミクス
    * ガス代
* 閲覧件の提供も可能

### [Fully On-Chain](https://fullyonchain.xyz/)

Solidityでsvgを生成しそれをmintするコントラクト。
0から作品を作成 or On-Chain上のsvgを合成して作成が可能になる。
 
* [Fully On-chain](https://fullyonchain.xyz/)
* [On-chain Asset Store](https://assetstore.wtf/en/group)
* [DotNounsToken | Address 0x1e3516211fe0cb030802237b4c4ce8277733a3b9 | Etherscan](https://etherscan.io/address/0x1e3516211fe0cb030802237b4c4ce8277733a3b9#code)

### [Nuance](https://www.home.nuance.xyz/)

* ブログサービス

### [Slash](https://coinpost.jp/?p=414201&fbclid=IwAR1pyoUJQ7gfcESS6ucZzZzRIhtESIChbIJYDLigFMPoUjfbmdTLohh2Eyg)

資料が諸々いけてる
https://youtu.be/kxJgnOV54Ns
 
#### 課題
* 消費者側、どんなトークンでもスワップせずに支払たい
* 事業者側、いろんなトークンで管理したくない
* 簡単に決済したい（相手のウォレットアドレスの記入ミス、金額入力ミスをなくしたい）

#### 解決策
web3版Stripe。あらゆるDEXとスマートコントラクトで接続しエクスチェンジの処理を自動的に完了させる機能を備えた決済サービス
リンクやQRで決済可能

#### 詳細
* Slash Web3 PaymentはあらゆるDEXとスマートコントラクトで接続しエクスチェンジの処理を自動的に完了させる機能を備えた決済サービス
  * 消費者側の「どんなトークンでもスワップせずに支払いしたい」と事業者側の「ステーブルコインで管理したい」というどちらもの想いを叶える決済ツール
* 事業主は簡単なセットアップで審査なく、クリプト決済を開始できる。ECサイトへの連携や、実店舗であればQRコードでの決済にも対応
* 消費者は、DEXでサポートされているトークンであればどんなトークンでも支払うことが可能。消費者が支払いに使ったトークンをDEX上で自動的にスワップし、事業者の元にはステーブルコインで届く。
* 事業者側に手数料はかからず、消費者が支払いの際にガス代と共に支払う。
* 独自トークンを発行し、決済手数料はそれと連動して変動させる
* 独自トークンホルダーによる投票で利益の寄付先の決定
* 関連プロジェクト
  * NFTの中にトークンを格納できる「NFT Vault」
  * SBTを活用したKYCソリューションと優良顧客（ロイヤルカスタマー）向けのサービス

[【Slash Web3 Payment】消費者は好きなトークンで支払い、事業者はステーブルコインで受け取り。どんな事業者でも簡単にクリプト決済を導入できる決済ツール！関連サービスや展望も考察！](https://substack.com/inbox/post/94739082)
 
### [Solv](https://solv.finance/home)

* 金融系NFTの作成&売買ができるプラットフォーム
* Vesting Voucher, Convertible Voucher, Bond Voucher という3種類のプロダクト（金融商品NFT）の作成とそのマーケットを提供
* ERC3525を利用している
 
### [NFT] [Hashmasks](https://www.thehashmasks.com/)

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

## アイデアメモ

* 旅行関連とかお金動かす系は"意味"がありそう
* "職人芸"となっている技術の保存先としてブロックチェーンを利用するの良さそう。それをデータ化、言語化するのは他の方法（IOT、データ分析、リサーチ）で行う。後世に残すべきものだし、それを利用して利益を得ることもできそう。
* githubなどの自分がよく使うサービスへの展開を想像すると良さそう、興味湧く
* 一部の色を塗れるとかの権利をtokenかするのも面白そう、hashmasksぽいけど
* イベントに合わせたNFTを作成できるもの
  * ボタン生成アプリみたいに、自由に自分達で作成できてもいいかも。それが発行されたら作成者にもお金が入るとか。
* Web2時代のもののweb3版を考えるのはアイデアのもとになりそう
  * Stripeのweb3版としてのSlash

## Readings

見たり読んだりしたがまとめてはいないものの感想

* [なぜDeFiの次がNFTなのか？５つの理由【徹底解説シリーズ】](https://www.youtube.com/watch?v=sxPg4Isx7DE)
  * デジタルコンテンツに価値が付きだす、これがNFTのすごいことらしい
    → 何がなんでも価値がつけばいいというわけではないとも思う。価値がつくべきものってなんだろうか。アートとかはまあわかる気もする。
