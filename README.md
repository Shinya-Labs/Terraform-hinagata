# 🌐 AWS Static Website Hosting with S3 + CloudFront
## 📌 プロジェクト概要
このプロジェクトは、AWSのS3とCloudFrontを使用して静的Webサイトをホスティングする構成をTerraformで自動化したものです。  
インフラ構築の基礎理解と、IaC（Infrastructure as Code）の実践を目的としています。

---

## 🛠 使用技術・サービス
- **AWS S3**：静的ファイルのホスティング
- **AWS CloudFront**：CDNによる高速配信
- **Terraform**：インフラ構成の自動化
- **Route 53（任意）**：独自ドメインの設定（今回は未使用）

---

## 🧱 アーキテクチャ図
※ draw.io や Excalidraw などで作成した構成図をここに貼り付けてください  
（例：`docs/architecture.png`）

---

## 🚀 デプロイ手順

1. AWS CLIとTerraformをローカルにインストール
2. `terraform init` で初期化
3. `terraform apply` でインフラ構築
4. `index.html` と `error.html` をS3にアップロード
5. CloudFrontのドメインでサイトを確認

---

## 💡 学んだこと・工夫した点
- S3のバケットポリシーによる公開設定
- CloudFrontのHTTPS対応とリダイレクト設定
- Terraformによる再現性のある構成管理

---

## 🔧 今後の改善点
- 独自ドメイン（Route 53）との連携
- ACMによるカスタムSSL証明書の導入
- CI/CDによる自動デプロイの実装

---

## 📂 ディレクトリ構成（例）


.
├── main.tf
├── variables.tf
├── outputs.tf
├── index.html
├── error.html
└── README.md

---

## 🧑‍💻 作者
- 名前：中村 真也（Shinya Nakamura）
- GitHub：@Shinya-Labs
- 資格：CCNA / LPIC Lv.2 / 学習中：LPIC Lv.3 305, AWS SAA

---

## 📣 ライセンス
MIT License
