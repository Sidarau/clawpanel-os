# ClawPanel OS

Base template for ClawPanel user instances.

## Quick Start

```bash
# Create instance
gh repo create my-instance --template Sidarau/clawpanel-os

# Install use cases
./scripts/install-use-case.sh knowledge-base
./scripts/install-use-case.sh social-research
```

## Structure

- `platform/` — Core dashboard UI (read-only)
- `system/` — Agents, memory, todo, scripts
- `use-cases/` — Modular apps (populated during onboarding)
- `infra/` — Terraform for Lightsail provisioning

## License

MIT
