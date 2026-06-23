# ryzy's claude marketplace

Personal [Claude Code](https://docs.claude.com/en/docs/claude-code) marketplace — my forks and curated picks.

## Plugins

| Plugin | What | Source |
| --- | --- | --- |
| `superpowers` | Core skills: TDD, debugging, planning, collaboration workflows | fork of [obra/superpowers](https://github.com/obra/superpowers) with my customizations |
| `superpowers-chrome` | Chrome DevTools access via the `browsing` skill | [obra/superpowers-chrome](https://github.com/obra/superpowers-chrome) |

## Install

```sh
claude plugin marketplace add ryzy/ryzy-claude-marketplace
claude plugin install superpowers@ryzy-claude-marketplace
claude plugin install superpowers-chrome@ryzy-claude-marketplace
```

## Maintaining the superpowers fork

`superpowers` is a fork I edit in [`ryzy/superpowers`](https://github.com/ryzy/superpowers). To pull obra's upstream:

```sh
git fetch upstream && git merge upstream/main   # resolve conflicts against my edits, then push
```

After pushing fork changes: `claude plugin marketplace update ryzy-claude-marketplace`.
