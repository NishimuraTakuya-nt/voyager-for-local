# Local GraphQL Voyager

このプロジェクトは、ローカル開発環境でGraphQLスキーマを視覚的に探索するためのGraphQL Voyagerツールを提供します。Express.jsを使用して、Webサーバー上でVoyagerを実行します。

## 特徴

- **GraphQL Voyager統合**: GraphQLスキーマをインタラクティブに視覚化。
- **Expressサーバー**: Voyagerツールを提供するためのシンプルなExpressサーバー。

## 前提条件

- Node.js (`.node-version`に指定されたバージョン)
- npm (Node Package Manager)

## インストール方法

1. リポジトリをローカルマシンにクローンします。
2. プロジェクトディレクトリに移動します。
3. `npm install`を実行して依存関係をインストールします。

## アプリケーションの起動方法

サーバーを起動するには、以下を実行します:

```bash
npm start
```

これにより、Expressサーバーが`http://localhost:3000`で起動します。ブラウザでこのURLを開いて、GraphQL Voyagerインターフェースにアクセスします。

## 設定

Voyagerツールは、設定されたGraphQLエンドポイントからGraphQLスキーマをフェッチします。
GraphQLサービスが正しく設定されたエンドポイントで実行されていることを確認してください。エンドポイントのURLは、`public/index.html`内の`introspectionProvider`関数で指定します。必要に応じて、この関数内のURLを適切なものに更新してください。

## 依存関係

- Express: Webサーバー上でVoyagerツールを提供します。
- GraphQL Voyager: GraphQLスキーマのインタラクティブな視覚化を提供します。
