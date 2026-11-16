# sixzjd DSH Plugin Market Index

A [DSH](https://github.com/deepseek-ai/deepseek-harness) plugin market index (format 1) for sixzjd's self-developed plugins.

## Index source URL

Add either URL in **DSH Web → Plugins → Discover → Add index source**:

- GitHub Pages (CDN, recommended once live): `https://sixzjd.github.io/dsh-plugin-market-index/index.json`
- Raw GitHub (works immediately): `https://raw.githubusercontent.com/sixzjd/dsh-plugin-market-index/main/index.json`

> DSH 0.2.1+ only: enable the experimental **Custom plugin index** bundle first (Plugins → Experimental plugins), then the Discover tab appears.

## Plugins in this index

| Plugin | npm package | Version |
|---|---|---|
| Folder Attach | `dsh-folder-attach` | 0.1.5 |
| WorkBuddy Connect | `@sixzjd/dsh-workbuddy-connect` | 0.3.2 |
| OpenCode Connect | `@sixzjd/dsh-opencode-connect` | 0.3.1 |
| Usage Dashboard | `@sixzjd/dsh-usage-dashboard` | 0.6.5 |

## Updating

When a plugin is released: update its `version` and `publishTimestamp` in `index.json` (Unix seconds from `npm view <pkg> time --json`), then commit and push. The Discover cache TTL is 10 minutes; use the refresh button to pick up changes immediately.
