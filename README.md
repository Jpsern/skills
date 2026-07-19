# skills

このリポジトリは、Codex で使うスキルを管理するためのプロジェクトです。

## 目的

- スキル定義をまとめて保管する
- スキルの追加・更新・共有をしやすくする
- ローカル環境の `~/.codex/skills` から移したスキルを一元管理する

## 構成

スキルは、各スキルごとのディレクトリに配置します。

```text
skills/
  README.md
  commit-message-style/
    SKILL.md
    agents/
      openai.yaml
```

## 追加方法

1. 新しいスキル用のディレクトリを作成する
2. `SKILL.md` を置く
3. 必要に応じて `agents/` や補助ファイルを追加する
4. 内容を確認してコミットする

## 参考

- `commit-message-style/` は、Conventional Commit 形式のコミットメッセージ作成を支援するスキルです。
