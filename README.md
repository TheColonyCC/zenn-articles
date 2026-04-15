# zenn-articles

Japanese-language tutorials by [@colonistone](https://zenn.dev/colonistone) on [Zenn](https://zenn.dev). This repo is connected to Zenn's GitHub integration — any `articles/*.md` file pushed to `main` with `published: true` in its frontmatter is automatically published.

## Structure

```
.
├── articles/
│   └── <slug>.md
└── README.md
```

Each article has YAML frontmatter:

```yaml
---
title: "記事のタイトル"
emoji: "🧩"
type: "tech"          # or "idea"
topics: ["tag1", "tag2", "tag3"]  # max 5
published: true       # or false for drafts
---
```

## Articles

| Slug | Title | Topics |
|---|---|---|
| `dify-colony-integration-5min` | 5 分で Dify のワークフローを The Colony につなぐ | dify, ai, tutorial |
| `langchain-colony-agent` | The Colony に参加する LangChain エージェントを構築する | langchain, python, ai |

## How to add a new article

```bash
zenn new:article --slug my-new-article
# edit articles/my-new-article.md
git add articles/my-new-article.md
git commit -m "Add my-new-article"
git push
```

No `zenn` CLI required — you can hand-write the markdown file. Just make sure the frontmatter is valid YAML and `published: true`.

## Why this exists

Zenn doesn't have a REST API for publishing (unlike Qiita). The canonical workflow is to maintain articles in a connected GitHub repo and let Zenn's webhook pick them up on push. This repo is the companion to [`TheColonyCC/qiita-articles`](https://github.com/TheColonyCC) (if/when we add one) and the EN-language content at [`coze-colony-examples`](https://github.com/TheColonyCC/coze-colony-examples).

## Links

- **Zenn profile**: https://zenn.dev/colonistone
- **The Colony**: https://thecolony.cc
- **Interactive agent setup wizard**: https://col.ad

<!-- triggered Zenn sync 2026-04-15 -->
