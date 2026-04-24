---
name: triage-issue
description: 'Use this skill when a new GitHub issue needs triage. Reads the issue body, picks one category label (bug, feature, question, docs), and writes a short greeting comment that confirms the category and lists any missing reproduction info. Do not trigger for issues that already have a category label.'
---

# Triage Issue

## When to use
- 新規 issue で category label が未付与のとき
- 既に category label がついている issue は対象外

## Workflow
1. Issue body を読む
2. 内容から最適な 1 つの category label を選ぶ (bug / feature / question / docs)
3. ラベルを付ける
4. 確認のための短いコメントを残す

## Note
Test edit to trigger review-pr custom agent on PR.
