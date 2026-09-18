# pudu-task-telemetry

Skill for measuring bounded local AI subtasks with [Pudu AI](https://github.com/devjaime/pudu-ai) hardware evidence and installed [Ollama](https://ollama.com) models.

This is the skills.sh / Agent Skills distribution. The same skill is also contributed to [claude-code-templates](https://github.com/davila7/claude-code-templates/pull/918).

## Install (skills.sh)

```bash
npx skills add devjaime/pudu-task-telemetry
```

List without installing:

```bash
npx skills add devjaime/pudu-task-telemetry --list
```

After install, the skill lives under your agent's skills directory (for Claude Code: `.claude/skills/pudu-task-telemetry/`).

## Requirements

- Node.js >= 20.3
- [Pudu AI](https://github.com/devjaime/pudu-ai) on PATH
- A running **local** Ollama server (`OLLAMA_NO_CLOUD=1` on the server before confirming local-only)

Do not download models or change global settings as part of diagnosis.

## Usage

From a project root, after install:

```bash
node .claude/skills/pudu-task-telemetry/scripts/pudu-task.mjs doctor --repo . --json
```

See `skills/pudu-task-telemetry/SKILL.md` and `references/` for the full flow (recommend, start, run-local, finish, report).

## Packs

skills.sh packs are created in the UI ([Create pack](https://skills.sh/packs/create)), not via GitHub PR. After this repo is public, add `devjaime/pudu-task-telemetry` as a GitHub source.

## License

MIT
