# Workspace Structure Guide for Agents

## Directory Layout

```
workspace/
├── platform/
│   └── clawpanel/          # Core UI — DO NOT MODIFY
├── use-cases/              # Modular apps — CREATE HERE
│   └── <use-case-name>/
│       ├── manifest.json
│       ├── app/            # UI code
│       ├── docs/           # SPEC, README
│       └── workflows/      # Antfarm workflows
├── system/
│   ├── agents/             # Agent identities
│   ├── memory/             # Daily logs
│   ├── todo/               # Board, priorities
│   └── scripts/            # Automation
└── infra/                  # Deployment
```

## Rules

1. **Never modify `platform/`** — It's infrastructure
2. **Create use cases in `use-cases/`** — One folder per module
3. **Use `system/` for shared resources** — Agents, scripts
4. **Personal data** — Goes in `USER.md`, `system/memory/`

## Creating a Use Case

1. Create folder: `use-cases/{name}/`
2. Add `manifest.json` with use case config
3. Add `app/`, `docs/`, `workflows/` as needed
4. Update `system/todo/board.json` with new cards
