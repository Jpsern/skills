---
name: commit-message-style
description: Generate conventional git commit messages with clear prefixes and concise subjects. Use when asked to write or improve a commit message, choose a commit prefix, or commit staged changes.
---

# Commit Message Style

このスキルは、git のコミットメッセージを conventional commit 形式で整えるためのものです。
ルール自体は英語のまま維持し、理解しやすいように見出しと補足を日本語化しています。

## Prefix の選び方

変更内容にいちばん近い種類を選びます。迷ったら、より小さい範囲の prefix を優先します。

- `feat`: new user-facing functionality
- `fix`: bug fixes
- `docs`: documentation-only changes
- `chore`: tooling, housekeeping, config, ignore files, or dependency maintenance
- `refactor`: behavior-preserving code changes
- `test`: tests only
- `perf`: performance improvements
- `build`: build or packaging changes
- `ci`: CI workflow changes
- `revert`: revert a prior commit

## Subject の書き方

件名は「prefix + 簡潔な命令形の要約」にします。短く、具体的に、英語で書きます。

- Use `prefix: imperative summary`
- Keep it short and specific
- Prefer lowercase except for proper nouns
- Avoid a trailing period
- Include a scope only when it improves clarity, for example `feat(selector): add list windowing`
- Write the subject line in English

## Body の書き方

本文には変更内容の要約を必ず入れます。追加の文脈が必要な場合のみ、その補足も1, 2文で加えます。

- Write the commit body in Japanese
- Include a concise summary of the change
- Add extra context only when it is useful
- Keep the body concise and factual

## 一貫した運用

以下の対応関係を保ちます。新機能なら `feat:`、不具合修正なら `fix:` のように、意味に合わせて選びます。

- Use `feat:` for new functionality and visible improvements
- Use `fix:` for bug fixes
- Use `docs:` for README, spec, or comment updates
- Use `chore:` for `.gitignore`, lockfiles, and repo maintenance
- Choose the smallest accurate prefix rather than overusing `feat:`

## 例

- `feat: add list windowing to selector`
- `docs: update selector usage`
- `chore: add node gitignore`

