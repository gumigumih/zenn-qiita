# 📘 技術記事のまとめ

このリポジトリは、私が執筆している技術記事やノウハウを管理するためのものです。Zenn や Qiita で公開している記事の一覧や、ローカルでの執筆環境についてまとめています。

## 📝 記事公開先

- 📚 Zenn: [https://zenn.dev/gumigumih](https://zenn.dev/gumigumih)
- 🧪 Qiita: [https://qiita.com/gumigumih](https://qiita.com/gumigumih)

## 🚀 Zenn CLI の使い方

Zenn CLI を使用すると、ローカルで記事の執筆やプレビューが可能です。

### 新しい記事の作成

```bash
npx zenn new:article --slug <記事のスラッグ>
```

対話形式でタイトルや公開設定を入力すると、`articles/` フォルダ内に新しい Markdown ファイルが作成されます。

### プレビュー実行

```bash
npx zenn preview
```

ブラウザで `http://localhost:8000` にアクセスすると、リアルタイムでプレビューが確認できます。

### 記事の投稿

Zenn では CLI からの直接投稿はできません。GitHub 連携を使って、`articles/` フォルダに Markdown ファイルを配置し、GitHub に Push することで記事が公開されます。

詳細: [https://zenn.dev/zenn/articles/zenn-cli-guide](https://zenn.dev/zenn/articles/zenn-cli-guide)

## 🛠 Qiita CLI の使い方

Qiita CLI は、ローカル環境で Qiita 記事の執筆、プレビュー、投稿を可能にする公式ツールです。

### 新しい記事の作成

```bash
npx qiita new <記事のファイル名>
```

このコマンドで `public/` ディレクトリ内に `<記事のファイル名>.md` が作成され、YAML 形式の Front Matter が自動的に挿入されます。

### プレビューの起動

```bash
npx qiita preview
```

ブラウザで `http://localhost:8888` にアクセスすると、リアルタイムで記事のプレビューが確認できます。

### 記事の投稿

```bash
npx qiita publish <記事のファイル名>
```

または、すべての記事を一括で投稿・更新する場合：

```bash
npx qiita publish --all
```
