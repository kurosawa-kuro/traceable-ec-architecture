# traceable-ec-architecture

# 🛒 EC × サプライチェーン × データ分析 × ブロックチェーン  
## 実務で通用するポートフォリオ設計 - フルアーキテクチャ対応

---

## 📌 概要

このプロジェクトは、**EC業務とサプライチェーンのリアルな業務フロー**をベースに、  
以下の技術・構成を組み合わせて **実務でそのまま運用できるレベルの構成**を再現したものです。

---

## 🔧 技術スタック・構成

- **Next.js**（ユーザー・管理画面UI）
- **Go（Gin）**（マイクロサービスAPI）
- **AWS EKS / Fargate / CDK**（インフラ）
- **Cognito**（認証）
- **Prisma + PostgreSQL / Redshift**（データ永続 & 分析）
- **Hyperledger Fabric**（注文・出荷・在庫履歴の不変記録）
- **Tableau / Redash**（BIダッシュボード）
- OpenAI Rag

---

## 📌 特徴

| 項目 | 説明 |
|------|------|
| 🛍️ EC業務再現 | 注文、カート、購入履歴、返品、トップ表示などを忠実に再現 |
| 🧱 マイクロサービス設計 | order / inventory / shipment など分離してAPI化 |
| 🔐 セキュリティ設計 | Cognitoベースの認証、ユーザー状態管理（ACTIVE/DELETED等） |
| 🔗 履歴保証 | Hyperledger Fabricによるトランザクションの証跡記録 |
| 📊 データ可視化 | RedshiftにETLし、TableauでKPIを可視化 |
| 🧠 データ設計 | ViewHistory / CartItemなどを分析前提で設計（RandomForest/PCA向け） |

---

## 🎯 面接・実務アピールポイント

- **設計から永続化・分析・可視化まで一貫して設計可能**
- **インメモリで爆速PoC → DB化 → 分析まで段階的に構築できる力**
- **業務設計力と技術選定理由が明確に説明できる構成**

---

## 💡 次のステップ（予定）

- Fabricブロックを管理画面から可視化
- Redshift連携部分をLambda + Glueで強化
- GraphQLエンドポイント対応
