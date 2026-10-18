# imbue-skills

Imbue's skills for coding agents, published as one plugin marketplace that Claude Code and Codex install from.

## Plugins

- `imbue-mngr-skills` (`plugins/imbue-mngr-skills/`): skills that teach an agent how to use [mngr](https://github.com/imbue-ai/mngr), the CLI for running coding agents anywhere, for example to coordinate with other agents.
- `imbue-studio-skills` (`plugins/imbue-studio-skills/`): skills that teach an agent how to drive [Imbue Studio](https://github.com/imbue-ai/mngr/tree/main/apps/minds): its workspaces, its API, and its accounts. Imbue Studio is built on mngr, so install both.

## Installation

With the Claude Code CLI:

```bash
claude plugin marketplace add imbue-ai/imbue-skills
claude plugin install imbue-mngr-skills@imbue-skills
claude plugin install imbue-studio-skills@imbue-skills
```

With the Codex CLI:

```bash
codex plugin marketplace add imbue-ai/imbue-skills
codex plugin add imbue-mngr-skills@imbue-skills
codex plugin add imbue-studio-skills@imbue-skills
```

Through mngr, which offers these plugins alongside the others it knows about:

```bash
mngr extras claude-plugin
```

## Contributing

This repository is written only by an automated export from [imbue-ai/mngr](https://github.com/imbue-ai/mngr), on every push to its `main` branch.
Nothing is edited here directly; send issues and pull requests to that repository.
The plugins' sources there are `libs/mngr/skills_plugin/` and `apps/minds/skills_plugin/`, and this README, the marketplace manifest, and the LICENSE come from `mirror/skills_overlay/`.

`imbue-ai/mngr-claude-skills` is this marketplace's frozen predecessor; it is archived and no longer updated.
