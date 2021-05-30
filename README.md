![](https://zenn.dev/images/og-large.png)

# Zenn Docs

Zennに投稿する記事を管理するレポジトリです.
Docker + VS Codeで執筆環境をポータブル化し, textlintをGitHub Actionsに組み込んで文書校正を自動化しています.

## Dependency

- Docker
- VSCode
- VSCode Extension: Remote - Containers

## Usage

## 記事の新規作成

1. 以下のコマンドを実行して執筆開始
```
git branch article/xxx
npm run new:article
npm run start
```

2. 記事を書き終えたらpushしてPull Requestを作成, textlintで問題がなければmergeする

3. 自動的にZennに記事が追加される

## 記事の修正

1. fix/xxxブランチで新規作成時と同様に執筆

```
git branch fix/xxx
npm run start
```

## 記事の削除

1. fix/xxxブランチで記事を削除してmergeする

```
git branch fix/xxx
```

2. Zennに公開されている記事を手動で削除する