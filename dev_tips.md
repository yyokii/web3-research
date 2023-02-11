## Hardhat プロジェクトの作成

```
// ルートとcontractディレクトリ作成
mkdir {ProjectName}
cd {ProjectName}
mkdir contract
cd contract
npm init -y
npm install --save-dev hardhat @openzeppelin/test-helpers
npm install dotenv @openzeppelin/contracts

// hardhatプロジェクト作成
npx hardhat

// Sampleプロジェクトのテストが通るか確認
npx hardhat test
```

## その他

* [Web3開発テクニック50選を紹介](https://zenn.dev/nft/articles/web3-dev-techniques)
